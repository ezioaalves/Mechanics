# Technique — schema (stub; existing all_jutsus.json unaffected)

## Machine-readable definition

```yaml
entity: technique
spec_version: 1
fields:
  name:                {type: string, required: true}
  slug:                {type: string, required: true, pattern: "^[a-z0-9-]+$"}
  source:              {type: string, required: true}
  discipline:          {type: enum, required: true, values: [ninjutsu, taijutsu, genjutsu, fuinjutsu, chakra-control]}
  rank:                {type: integer, required: true}
  chakra_cost:         {type: string, required: true}
  learn_dc:            {type: integer, required: true}
  perform_dc:          {type: integer, required: true}
  save_dc:             {type: string_or_null, required: false}
  is_hijutsu:          {type: boolean, required: true}
  is_kinjutsu:         {type: boolean, required: true}
  drawbacks:           {type: list_of_object, required: false}
  foundry_source:      {type: string_or_null, required: true}
  house_rules_applied: {type: list_of_string, required: true}
  created:             {type: date, required: true}
  updated:             {type: date, required: true}
```
