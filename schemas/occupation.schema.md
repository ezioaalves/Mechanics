# Occupation Schema

Canonical occupation data lives in `Mechanics/Character_Options/Occupations/occupations.yaml`.
It is generated from every occupation markdown file under `Mechanics/Character_Options/Occupations/`,
excluding `Homebrew/Occupation Formula.md`.

## Machine-readable definition

```yaml
entity: occupation
spec_version: 1
collection:
  occupations: {type: list_of_occupation, required: true}
fields:
  name:                  {type: string, required: true}
  slug:                  {type: string, required: true, pattern: "^[a-z0-9-]+$"}
  status:                {type: string, required: true, allowed: [active, draft, deprecated]}
  source_md:             {type: string, required: true}
  source_category:       {type: string, required: true}
  source_subcategory:    {type: string_or_null, required: true}
  description:           {type: string, required: true}
  prerequisite:          {type: string, required: false}
  skill_select_count:    {type: integer, required: true}
  fixed_class_skills:    {type: list_of_skill_option, required: true}
  class_skill_options:   {type: list_of_skill_option, required: true}
  raw_skills:            {type: string, required: false}
  feat_select_count:     {type: integer, required: true}
  feat_options:          {type: list_of_named_option, required: true}
  technique_options:     {type: list_of_named_option, required: true}
  wealth_bonus:          {type: integer, required: true}
  reputation_bonus:      {type: integer, required: true}
  affiliation:           {type: string, required: false}
  expertise:             {type: string, required: false}
  tags:                  {type: list_of_string, required: true}
  foundry_source:        {type: string_or_null, required: true}
  house_rules_applied:   {type: list_of_string, required: true}
  created:               {type: date, required: true}
  updated:               {type: date, required: true}
```

## Nested Types

```yaml
skill_option:
  label: {type: string, required: true}
  slug:  {type: string, required: true}
  key:   {type: string, required: true}

named_option:
  name:        {type: string, required: true}
  source_uuid: {type: string_or_null, required: true}
```

## Foundry Mapping

Generated compendium items are PF1e `feat` items with `system.subType: trait`.
Initial `system.classSkills` and `system.links.supplements` are empty. The module
fills them when an occupation is applied: fixed and selected class skills go to
Details, while selected feats and occupation technique references go to Links.
