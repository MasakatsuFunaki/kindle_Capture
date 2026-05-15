# Kindle Capture

Captures pages.

## 1. Configure

Open the book in Kindle for PC, look at the footer (`Page X of N`), then
edit `config.json`:

```json
{
  "total_pages": 241
}
```

## 2. Run

Open the book in Kindle for PC, then:

```powershell
capture.exe
```

Pages land in `output\<book title>\`.
