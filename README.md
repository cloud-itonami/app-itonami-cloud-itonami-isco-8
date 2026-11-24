# cloud-itonami-isco-8

Occupation reference: ISCO-08 (International Labour Organization, 2012), major group 8 (Plant and machine operators). This app is not produced, reviewed or endorsed by the ILO.
職業の参照: ISCO-08（国際労働機関 ILO、2012 年）の大分類 8（Plant and machine operators）。日本語の名称は当方の訳です。この app は ILO が作成・確認・推奨したものではありません。

**ISCO Major 8 — Plant and machine operators** — the ISCO-08 major group 8 series app (Tauri v3, `restricted-wasm-v1`).

Plant-operators sample: `physics.edn` carries two cases (`assembly-parts-handling`, `pallet-plant-transport`), and `docs/samples/operator-console.html` renders the plant-operators console sample.

- Source: `cloud-itonami-isco-8` (repo `app-itonami-cloud-itonami-isco-8`), slug `isco8`, identifier `network.itonami.isco8`.
- Bot profile: `hermes/profiles/itonami-isco-8` (source `cloud-itonami/app-itonami-isco@9d661bc593c28173e02ad5530e7b2832ea3b9830`).

**Safety and qualification model.** Scope is ISCO-08 major groups 81–83 (stationary plant and machine operators, assemblers, drivers and mobile plant operators). `:itonami.blueprint/adjudicating` is `false`: dangerous-work decisions are made by humans, and robots/automation assist only — they never instruct dangerous work. A worker's qualification is never asserted as "qualified"; it is one of four states — `unverified`, `applying`, `valid`, `not-required` — per `:itonami.blueprint/qualification-states`. Work, inspection and correction history is append-only (`:itonami.blueprint/append-only` `true`) and is never deleted. All samples in this repository are synthetic (no real persons or companies); licensed-work properties are held pack-side and are not in this repo.

AGPL-3.0-or-later, forkable by any qualified operator. Part of the
[cloud-itonami](https://itonami.cloud) open business fleet.
