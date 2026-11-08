# AI Engineering Summit 2026 - Talk Catalog

This repository is the backing store for the summit talk catalog.

## Collection metadata

`catalog/collection.json` contains the authoritative collection record, including
`item_count`, the definitive number of entries in collection `aie-conf-2026`.

## Item listings

The same listing is published in two shapes:

- `catalog/items_all.json` - one consolidated export of every item. This file is
  very large because every entry carries a long abstract.
- `catalog/pages/page_01.json` ... paginated listing pages. Every page contains an
  `items` array plus `total_results`, `next_page_token`, and `prev_page_token`.
  Follow `next_page_token` until it is null to walk the complete membership.

## Project references

Each item has a `project_ref` (an owner/repository shorthand). Resolve it through
the code-hosting service to obtain the project's current canonical URL and a
description. Some references use an old owner or project name because the
project moved after the talk was recorded.
