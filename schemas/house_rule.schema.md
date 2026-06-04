# House Rule — schema (stub; House_Rules/*.md are authoritative prose)

This schema describes how a future per-house-rule YAML projection would be shaped. Not used this ship — the canonical projection is `house_rules_active.yaml`, not per-rule sidecars.

## Machine-readable definition

```yaml
entity: house_rule
spec_version: 1
fields:
  name:                {type: string, required: true}
  slug:                {type: string, required: true, pattern: "^[a-z0-9-]+$"}
  source:              {type: string, required: true}
  status:              {type: enum, required: true, values: [active, retired, experimental]}
  affects:             {type: list_of_string, required: true}
  summary:             {type: string, required: true}
  created:             {type: date, required: true}
  updated:             {type: date, required: true}
```
