# School — schema

Static school packages for character-background choices. The canonical catalog
lives at `Mechanics/Character_Options/Schools/schools.yaml`; legacy `.md`
files in the same tree are source notes, not generator input.

## Machine-readable definition

```yaml
entity: school_catalog
spec_version: 1
fields:
  schools: {type: list_of_object, required: true}
  schools[].name: {type: string, required: true}
  schools[].slug: {type: string, required: true, pattern: "^[a-z0-9-]+$"}
  schools[].status: {type: enum, required: true, values: [active, draft, retired]}
  schools[].village: {type: string_or_null, required: true}
  schools[].clan: {type: string_or_null, required: true}
  schools[].legacy_name: {type: string_or_null, required: false}
  schools[].source_md: {type: string, required: true}
  schools[].focus: {type: string, required: true}
  schools[].description: {type: string, required: true}
  schools[].bonus_feat: {type: object, required: true}
  schools[].bonus_feat.name: {type: string, required: true}
  schools[].bonus_feat.source_uuid: {type: string_or_null, required: true}
  schools[].starting_techniques: {type: list_of_object, required: true, count: 3}
  schools[].starting_techniques[].name: {type: string, required: true}
  schools[].starting_techniques[].source_uuid: {type: string_or_null, required: true}
  schools[].starting_outfit: {type: string, required: true}
  schools[].tags: {type: list_of_string, required: true}
  schools[].foundry_source: {type: string_or_null, required: true}
  schools[].house_rules_applied: {type: list_of_string, required: true}
  schools[].created: {type: date, required: true}
  schools[].updated: {type: date, required: true}
```
