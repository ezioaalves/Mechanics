# Occupation — schema (stub)

## Machine-readable definition

```yaml
entity: occupation
spec_version: 1
fields:
  name:                {type: string, required: true}
  slug:                {type: string, required: true, pattern: "^[a-z0-9-]+$"}
  source:              {type: string, required: true}
  prerequisites:       {type: object_or_null, required: true}
  bonus_class_skills:  {type: list_of_skill_slug, required: true}
  starting_feat_options: {type: list_of_string, required: false}
  wealth_bonus:        {type: integer, required: false}
  foundry_source:      {type: string_or_null, required: true}
  house_rules_applied: {type: list_of_string, required: true}
  created:             {type: date, required: true}
  updated:             {type: date, required: true}
```
