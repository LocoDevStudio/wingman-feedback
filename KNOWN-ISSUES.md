# Known issues

Problems we know about and are working on, in plain words. The same list appears on the Updates page in the
Wingman panel. Status: **Workaround** (there's a way around it today), **Investigating** (we're finding the
cause), **Building** (the fix is in progress), **Fixed** (fixed in the version named).

Last updated: 2026-11-16.

### Motion matching: Play can crash after removing animations from a database
**Workaround.** Rebuilding an existing Pose Search database with fewer animations in the same editor session can
keep the old search index, and pressing Play then crashes Unreal. Restart the editor before pressing Play after
changing an existing database's animations. From 0.22.7, Wingman reports it instead of saying it worked.

### A Play check does not save the level first
**Workaround.** Actors placed just before a Play check are lost if the editor crashes during it. Save the level
before asking for a Play check.

### A failed Python script keeps the edits it already made
**Workaround.** When a script stops with an error halfway, the changes it made before the error stay. Ask Wingman
to check the result, or use Undo in Unreal.

### A placed actor's new value can be lost on the next compile
**Investigating.** Changing a property on an actor in the level can report success, then the value goes back after
the next Blueprint compile. Check the actor's value after compiling.

### Wingman's AI tools can disappear in the middle of a session
**Workaround.** If the AI suddenly says it has no Unreal tools, reopen the Wingman panel.

### Viewport screenshots can fail or come out dark
**Workaround.** When Unreal is in the background, Wingman may get no rendered frame or a dark image. Keep the
Unreal window visible while Wingman takes screenshots.

### Clicking editor buttons and changing Project Settings rarely work
**Building.** Clicking buttons in Unreal's own interface and finding Project Settings sections fail most of the
time. Do these two by hand for now.

### Control Rigs made on UE 5.8 cannot be read or edited
**Workaround.** Edit those Control Rig assets in Unreal's Control Rig editor.
