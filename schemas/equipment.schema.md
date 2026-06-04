# Equipment — schema (stub)

## Machine-readable definition

```yaml
entity: equipment
spec_version: 1
fields:
  name:                {type: string, required: true}
  slug:                {type: string, required: true, pattern: "^[a-z0-9-]+$"}
  source:              {type: string, required: true}
  item_type:           {type: enum, required: true, values: [weapon, armor, shield, consumable, tool, vehicle, artifact, general]}
  purchase_dc:         {type: integer_or_null, required: true}
  weight:              {type: number_or_null, required: false}
  properties:          {type: object_or_null, required: false}
  foundry_source:      {type: string_or_null, required: true}
  house_rules_applied: {type: list_of_string, required: true}
  created:             {type: date, required: true}
  updated:             {type: date, required: true}
```
