# feed
A GH page for rss feed of meetup times and community messages.

## Community Message Format

```json
   {
        "id": "1",
        "title": "Anmelden für Versammlung",
        "content": "Heute ist die letzte Möglichkeit dich für die kommende Versammlung anzumelden um dein Gemeinschaftseinkommen abzuholen. Diese findet schon übermorgen Mittag statt.",
        "showAt": "2022-12-07T11:30:00.00+00:00"
    }
```

### Hints
Some JSON libraries do not allow dangling commas after the last entry in the list, or map. So this should be prevented.
