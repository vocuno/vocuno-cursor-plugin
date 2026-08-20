# Vocuno for Cursor

Official Cursor plugin for [Vocuno](https://vocuno.com), the AI music studio. It connects Cursor to Vocuno's hosted Model Context Protocol server so Cursor can create and edit music directly in your Vocuno account.

## What it can do

- **Generate songs:** Create complete songs with vocals from a prompt or your own lyrics, across multiple music models.
- **Covers and remixes:** Reimagine a song in a new style or build mashups from two tracks.
- **Stems:** Separate vocals, drums, bass, and instruments; remove reverb; extract MIDI from stems.
- **Voice:** Browse voices, convert vocals with explicit consent, or clone a voice for future generations.
- **Song tools:** Extend songs, replace sections, mix, master, detect BPM and chords, and convert audio formats.
- **Audio editing:** Trim, concatenate, loop, fade, filter, and adjust speed, pitch, or volume with free FFmpeg-based tools.
- **Account:** Check remaining credits and retrieve the status and shareable links of your generations.

Everything runs in your Vocuno library. Songs created through Cursor appear at [vocuno.com/app](https://vocuno.com/app) like anything you make on the site, with shareable streaming links returned as results.

## Installation

After marketplace approval, install **Vocuno** from Cursor's Marketplace or run:

```text
/add-plugin vocuno
```

For local testing, clone this repository into Cursor's local plugin directory and reload Cursor:

```bash
git clone https://github.com/vocuno/vocuno-cursor-plugin.git ~/.cursor/plugins/local/vocuno
```

## Authentication

The plugin connects to `https://vocuno.com/mcp` using OAuth. Cursor opens Vocuno's authorization page when you first enable the MCP server. Sign in with an existing Vocuno account and approve access; no API key is stored in this repository.

## Requirements

- A Vocuno account ([sign up free](https://vocuno.com)). New accounts include free credits.
- Generation tools consume Vocuno credits exactly as on the website. Editing and analysis tools marked free consume none.

## Usage examples

- "Create an upbeat synth-pop song about starting over in Lisbon."
- "Separate the vocals and instrumental from this audio file."
- "Detect this track's BPM, then retime it to 120 BPM."
- "Master this mix and return the finished track."
- "Extend this song with a final chorus and polished outro."

Cursor should obtain confirmation before unusually expensive multi-provider operations. Vocuno preserves source media and creates separate processed results; the MCP plugin does not expose deletion or overwrite tools.

## Links

- [Vocuno](https://vocuno.com)
- [Support](https://support.vocuno.com)
- [Privacy policy](https://vocuno.com/privacy)
- [Terms of service](https://vocuno.com/terms)

## License

The plugin package in this repository is licensed under the MIT License. Vocuno's hosted service remains governed by its Terms of Service.
