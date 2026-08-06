# Archive data guide

Each item in `_data/photos.yml` supports:

```yaml
- id: unique-id
  file: /assets/images/crew/groups/example.jpg
  title: Short title
  description: Full historical caption
  section: crew
  people:
    - virgil-wayne-reed
    - don-peterson
  topics:
    - life-aboard
  identified: true
```

Valid primary sections currently used by the site are `crew`, `marines`, `ship`, `damage`, `life-aboard`, `documents`, and `unidentified`.
