# Bloodline — schema (stub, content authored on demand)

## Machine-readable definition

```yaml
entity: bloodline
spec_version: 1
fields:
  name:                {type: string, required: true}
  slug:                {type: string, required: true, pattern: "^[a-z0-9-]+$"}
  source:              {type: string, required: true}
  tier:                {type: enum, required: true, values: [minor, intermediate, major]}
  clan:                {type: string_or_null, required: false}
  primary_ability:     {type: enum, required: false, values: [str, dex, con, int, wis, cha, none]}
  level_progression:   {type: list_of_object, required: true}
  prerequisites:       {type: object_or_null, required: true}
  foundry_source:      {type: string_or_null, required: true}
  house_rules_applied: {type: list_of_string, required: true}
  created:             {type: date, required: true}
  updated:             {type: date, required: true}
```
