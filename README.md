# Password Generator v1

A secure, client-side **password generator** built as a reusable React component. Pick a length and character-set options (uppercase, lowercase, digits, symbols), generate a random password in one click, and copy it to the clipboard.

Everything runs **100% in the browser** — no servers, no network calls, no tracking. Generated passwords never leave your machine.

## Features

- **Random password generation** — random character selection across configurable character pools
- **Customizable options** — toggle uppercase letters, lowercase letters, numbers, and symbols
- **Adjustable length** — control to set password length
- **One-click copy** — copy the generated password to the clipboard with visual confirmation
- **Strength feedback** — UI indicates relative password strength
- **No login, no backend** — pure client-side React; drop it into any app

## Tech Stack

- **React** (hooks: `useState`, `useCallback`)
- **shadcn/ui** components (`Button`, `Card`, `Slider`, `Switch`)
- **lucide-react** icons (`Copy`, `RefreshCw`)
- **Tailwind CSS** for styling

## Quick Start

This repository contains a single drop-in component file (`password-generator v1`).

1. Copy the component into your React project's components directory.
2. Install the dependencies it needs:

```bash
npm install lucide-react
# plus shadcn/ui + Tailwind CSS per your project setup
```

3. Import and render:

```jsx
import PasswordGenerator from "./components/password-generator"

export default function App() {
  return <PasswordGenerator />
}
```

## Project Structure

```
.
├── README.md                  # This file
├── LICENSE                    # MIT license
└── password-generator v1      # The React component (rename to .jsx/.tsx as needed)
```

## Security Notes

- Generation happens entirely in the browser's JS runtime; nothing is sent anywhere.
- For production use, prefer `crypto.getRandomValues()` over `Math.random()` for entropy.
- Do not display generated passwords on shared screens.

## License

[MIT](LICENSE) — free to use, modify, and ship.

---

## Author

Built by **Girish Lade** — [ladestack.in](https://ladestack.in)
