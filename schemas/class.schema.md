# Class — schema

Per-class structured data for the `naruto-d20-character-builder` skill. Sidecar `.yaml` lives next to the prose `.md` under `Mechanics/Character_Options/Classes/<subcategory>/`.

| Field | Type | Required | Notes |
|---|---|---|---|
| name | string | yes | Display name, e.g. "Fast Ninja" |
| slug | string | yes | kebab-case, unique across all classes |
| category | enum | yes | basic / advanced / paragon / prestige / npc |
| source | string | yes | Sourcebook citation, e.g. "NarutoD20 Redux v1.3 p.45" |
| ability | enum | yes | str / dex / con / int / wis / cha / none |
| hit_die | enum | yes | d4 / d6 / d8 / d10 / d12 |
| action_points | string | yes | Formula, e.g. "5 + level/2" |
| bab | enum | yes | low (1/2) / mid (3/4) / high (1/1) |
| saves.fort | enum | yes | low / mid / high |
| saves.ref | enum | yes | low / mid / high |
| saves.will | enum | yes | low / mid / high |
| defense_progression | enum | yes | low / mid / high |
| reputation_progression | enum | yes | low / mid / high |
| class_skills | list[skill_slug] | yes | Each must be in active_skills |
| skill_points_first_level | string | yes | Formula, e.g. "(5 + Int) × 4" |
| skill_points_per_level | string | yes | Formula, e.g. "5 + Int" |
| prerequisites | object \| null | yes | null for basic; required for advanced/paragon/prestige |
| talents | list[object] | no | `[{tree, talents: [name, ...]}, ...]` |
| bonus_feats | list[feat_slug] | no | Each must not be in removed_feats; not be a merged_feats key |
| special_features | list[object] | no | `[{level, name, description}, ...]` |
| foundry_source | string \| null | yes | "Compendium.…" / "bespoke" / null |
| house_rules_applied | list[string] | yes | e.g. `[eitr-feat-overhaul, kaihou-skill-list]` |
| notes | string \| null | no | Free-form |
| created | date | yes | ISO date |
| updated | date | yes | ISO date |

## Machine-readable definition

```yaml
entity: class
spec_version: 1
fields:
  name:        {type: string, required: true}
  slug:        {type: string, required: true, pattern: "^[a-z0-9-]+$"}
  category:    {type: enum, required: true, values: [basic, advanced, paragon, prestige, npc]}
  source:      {type: string, required: true}
  ability:     {type: enum, required: true, values: [str, dex, con, int, wis, cha, none]}
  hit_die:     {type: enum, required: true, values: [d4, d6, d8, d10, d12]}
  action_points: {type: string, required: true}
  bab:         {type: enum, required: true, values: [low, mid, high]}
  saves.fort:  {type: enum, required: true, values: [low, mid, high]}
  saves.ref:   {type: enum, required: true, values: [low, mid, high]}
  saves.will:  {type: enum, required: true, values: [low, mid, high]}
  defense_progression:    {type: enum, required: true, values: [low, mid, high]}
  reputation_progression: {type: enum, required: true, values: [low, mid, high]}
  class_skills:           {type: list_of_skill_slug, required: true}
  skill_points_first_level: {type: string, required: true}
  skill_points_per_level:   {type: string, required: true}
  prerequisites:          {type: object_or_null, required: true}
  talents:                {type: list_of_object, required: false}
  bonus_feats:            {type: list_of_feat_slug, required: false}
  special_features:       {type: list_of_object, required: false}
  foundry_source:         {type: string_or_null, required: true}
  house_rules_applied:    {type: list_of_string, required: true}
  notes:                  {type: string_or_null, required: false}
  created:                {type: date, required: true}
  updated:                {type: date, required: true}
```
