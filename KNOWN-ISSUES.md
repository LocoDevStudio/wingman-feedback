# Known issues

Problems we know about and are working on, in plain words. The same list appears on the Updates page in the
Wingman panel. Status: **Workaround** (there's a way around it today), **Investigating** (we're finding the
cause), **Building** (the fix is in progress).

Last updated: 2026-11-17.

### Changing Blueprints during Play can crash Unreal
**Investigating.** Stop Play before asking Wingman to change a Blueprint.

### Adding input keys can remove the existing ones
**Workaround.** After adding keys, ask Wingman to list the input mappings. Fixed in the next update.

### A level save can fail without saying so
**Workaround.** Save the level yourself with Ctrl+S and check for an error message.

### A changed value on a placed actor can go back
**Investigating.** After a Blueprint compile, check the actor's value again.

### A failed Python script keeps its first changes
**Workaround.** Ask Wingman to check the result, or use Undo.

### A Play check doesn't save the level first
**Workaround.** Save the level before asking for a Play check.

### Motion matching can crash Play after removing animations
**Workaround.** Restart Unreal before pressing Play. Fixed in the next update.

### Screenshots can come out dark
**Workaround.** Keep the Unreal window visible while Wingman takes screenshots.
