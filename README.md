# MVP-SONGWRITER

Music prompt generator for AI music platforms. Fill out a form describing the sound you want, and get tailored prompts for **Suno**, **Udio**, and **ElevenLabs Music**.

## Files

### `index.html`

The entire application — a single-page static HTML file with no dependencies. Contains:

- **Form UI** — inputs for genre, mood, energy, tempo/BPM, key, instruments, vocals, production style, era, song structure, duration, reference artists, and elements to avoid. Uses a tag system with quick-pick buttons for multi-value fields.
- **Prompt generators** — three functions (`buildSuno`, `buildUdio`, `buildElevenLabs`) that take the form data and produce platform-specific prompts. Each follows the conventions and field formats that work best on its respective platform (comma-separated tags for Suno, descriptive tags for Udio, natural-language sentences for ElevenLabs).
- **Tabbed output** — generated prompts are displayed in a tabbed panel with copy-to-clipboard buttons.
- **Email option** — after generating, a "Send prompts via email" button opens the user's email client with all three prompts addressed to info@aitheria.io.

## Usage

Open `index.html` in a browser. No build step or server required.
