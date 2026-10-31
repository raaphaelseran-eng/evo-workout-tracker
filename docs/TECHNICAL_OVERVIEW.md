# evo — Technology overview (non-sensitive)

This public note deliberately describes the **technology categories and responsibilities**, not implementation details.

| Layer | Technologies / responsibilities |
| --- | --- |
| Presentation | Flutter / Dart screens and user interactions |
| Application state | BLoC / Cubit architecture |
| Session domain | Workout interpretation, normalized exercises, editable sessions, exercise matching |
| Data services | Firebase Authentication, Cloud Firestore, client-side domain services |
| Insights | Training history, exercise trends, personal records and charting with `fl_chart` |
| Quality assurance | Local Dart test coverage for parser behavior, domain models, statistics and service interactions |

## Key engineering considerations

**Text interpretation:** accept flexible notations for sets, reps, load and comments, with user-visible reconciliation when meaning is unclear. No proprietary grammar or matching rules are included.

**Domain consistency:** modifications to past sessions need to be reflected in history and derived statistics.

**State and persistence:** keep the UI, domain transformations and storage responsibilities separated. This is a conceptual description of the codebase's responsibilities, not a promise of a formally verified architecture.

**Platform:** this is an **iOS-first Flutter app**, not proof of deployed Android/macOS/web builds.

## What is intentionally not public

No Dart code, unit tests, Firebase settings, Firestore rules/indexes, cloud-project identifiers, assets beyond carefully selected screenshots, parser algorithms, product secrets, training or user data, credentials or distribution artifacts.

**Do not upload the previous source-containing portfolio ZIP to a public GitHub repo.** This revised repository is the public-safe alternative for the project.
