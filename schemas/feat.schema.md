# Feat — schema (stub, content authored on demand)

Per-feat structured data. No YAML files exist at ship time for this category; the schema lints any future authoring.

## Machine-readable definition

```yaml
entity: feat
spec_version: 1
fields:
  name:                {type: string, required: true}
  slug:                {type: string, required: true, pattern: "^[a-z0-9-]+$"}
  source:              {type: string, required: true}
  feat_type:           {type: enum, required: true, values: [general, combat, item-creation, metamagic, teamwork, racial, flaw, bloodline]}
  prerequisites:       {type: object_or_null, required: true}
  benefit:             {type: string, required: true}
  normal:              {type: string_or_null, required: false}
  special:             {type: string_or_null, required: false}
  foundry_source:      {type: string_or_null, required: true}
  house_rules_applied: {type: list_of_string, required: true}
  created:             {type: date, required: true}
  updated:             {type: date, required: true}
```
