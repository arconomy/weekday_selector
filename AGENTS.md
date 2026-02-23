# Weekday Selector

## Purpose

Weekday Selector provides a Dart widget for selecting specific days of the week. Used in strategy scheduling and backtest configuration.

## Type

UI Widget (Dart/Flutter)

## Consumed By

- Strategy configuration screens
- Backtest setup UIs
- Scheduling interfaces

## Exposed Interface

**WeekdaySelector Widget**:
- Properties: `onChanged`, `selectedDays`, `enabled`
- Returns: `List<int>` (0=Monday, 6=Sunday)

## Usage Example

```dart
import 'package:weekday_selector/weekday_selector.dart';

WeekdaySelector(
  onChanged: (List<int> selected) {
    setState(() => selectedDays = selected);
  },
  selectedDays: selectedDays,
)
```

---

**Last Updated**: 2026-02-22



After ANY change to this service that affects:
- API surface (new/modified endpoints or gRPC methods)
- NATS subjects (new publish/subscribe calls)
- Data models (schema/migration changes)
- Config vars (new env vars)
- Inter-service dependencies (new gRPC clients or NATS consumers)

You MUST update this service's AGENTS.md to reflect the change before committing.
Update the root ./AGENTS.md if the change affects the architecture graph,
NATS subject registry, or gRPC relationship table.

---

**Last Updated**: 2026-02-23
