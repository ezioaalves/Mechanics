# Skill — schema (stub, descriptive only this ship)

The 43 active skill files already exist as prose under `Character_Options/Skills/`. This stub schema declares the shape a future per-skill YAML sidecar would take if/when one is authored.

## Machine-readable definition

```yaml
entity: skill
spec_version: 1
fields:
  name:                {type: string, required: true}
  slug:                {type: string, required: true, pattern: "^[a-z0-9-]+$"}
  source:              {type: string, required: true}
  key_ability:         {type: enum, required: true, values: [str, dex, con, int, wis, cha, none]}
  trained_only:        {type: boolean, required: true}
  armor_check_penalty: {type: boolean, required: true}
  retry:               {type: boolean, required: true}
  foundry_source:      {type: string_or_null, required: true}
  house_rules_applied: {type: list_of_string, required: true}
  created:             {type: date, required: true}
  updated:             {type: date, required: true}
```
