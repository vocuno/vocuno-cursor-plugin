# Vocuno for Cursor

Create original music and work with audio directly from Cursor through Vocuno's hosted Model Context Protocol server.

## What it can do

- Generate complete songs from a prompt or supplied lyrics
- Retrieve permanent Vocuno share pages for generated tracks
- Trim, concatenate, loop, fade, filter, mix, and master audio
- Detect BPM and analyze audio metadata
- Change tempo, pitch, volume, and file format
- Separate vocals, drums, bass, and other stems
- Remove reverb, noise, or echo
- Browse AI voices and convert vocals with explicit consent
- Create covers, extensions, mashups, and section replacements

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

## Usage examples

- "Create an upbeat synth-pop song about starting over in Lisbon."
- "Separate the vocals and instrumental from this audio file."
- "Detect this track's BPM, then retime it to 120 BPM."
- "Master this mix and return the finished track."
- "Extend this song with a final chorus and polished outro."

Some generation and processing tools consume credits from the connected Vocuno account. Cursor should obtain confirmation before unusually expensive multi-provider operations. Vocuno preserves source media and creates separate processed results; the MCP plugin does not expose deletion or overwrite tools.

## Links

- [Vocuno](https://vocuno.com)
- [Support](https://support.vocuno.com)
- [Privacy policy](https://vocuno.com/privacy)
- [Terms of service](https://vocuno.com/terms)

## License

The plugin package in this repository is licensed under the MIT License. Vocuno's hosted service remains governed by its Terms of Service.
