# Pomodoros

Shared pomodoro timer for [Delta Chat](https://delta.chat), built as a [webxdc](https://webxdc.org) app.

Two-phase focus + break timer with pie chart visualization. Choose 25 or 50 minute sessions. Tap the pie to reveal remaining time. Chat members are notified when time is up.

Multilingual symbol-based UI — no text labels to translate.

## Screenshots

| Chat preview | Idle | Running |
|:---:|:---:|:---:|
| ![Chat preview](screenshots/01.png) | ![Idle](screenshots/02.png) | ![Running](screenshots/03.png) |
| Live timer status in chat | Ready to start 25 or 50 min | Tap the pie for remaining time |

## Install

Download `pomodoros.xdc` from the [latest release](https://github.com/maphouse/pomodoros/releases/latest) and send it as a file in any Delta Chat conversation.

## Development

Requires [webxdc-dev](https://github.com/niclas/webxdc-dev) for local testing.

```bash
npx webxdc-dev app/
```

Package for Delta Chat:

```bash
(cd app/ && zip -9 --recurse-paths - *) > pomodoros.xdc
```