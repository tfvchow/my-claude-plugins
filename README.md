# My Claude Plugins

Personal collection of Claude Code plugins.

## Installation

1. Clone this repo:
   ```bash
   git clone https://github.com/tfvchow/my-claude-plugins.git
   ```

2. Add to your `.claude/settings.json`:
   ```json
   {
     "extraKnownMarketplaces": {
       "my-plugins": {
         "source": {
           "source": "directory",
           "path": "/path/to/my-claude-plugins"
         }
       }
     },
     "enabledPlugins": {
       "frugal-output@my-plugins": true
     }
   }
   ```

3. Restart Claude Code session.

## Plugins

### frugal-output

Minimal output style for terminal responses.

**Features**:
- Absolute minimum words in chat responses
- No pleasantries or verbose explanations
- Code/written output remains complete and self-contained
- No placeholders or incomplete implementations

**When to use**: Fast-paced coding sessions where brevity matters.

**Example**:
```
User: Add validation to the function
Claude: Adding validation.
[provides complete implementation]
```

## License

MIT
