# Race — schema (stub)

## Machine-readable definition

```yaml
entity: race
spec_version: 1
fields:
  name:                {type: string, required: true}
  slug:                {type: string, required: true, pattern: "^[a-z0-9-]+$"}
  source:              {type: string, required: true}
  size:                {type: enum, required: true, values: [fine, diminutive, tiny, small, medium, large, huge, gargantuan, colossal]}
  ability_modifiers:   {type: object, required: true}
  base_speed:          {type: integer, required: true}
  racial_features:     {type: list_of_object, required: true}
  foundry_source:      {type: string_or_null, required: true}
  house_rules_applied: {type: list_of_string, required: true}
  created:             {type: date, required: true}
  updated:             {type: date, required: true}
```
