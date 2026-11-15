# Day 0 — Wed 11 Nov: setting the table (no game yet)

**The rule we're working under.** Nothing of the game may exist before the jam opens (Thursday 07:00 our time). Tools, agent settings and prompts may. So today is plumbing.

**The team.**
- PC: the only human. Picks the idea, plays every build on a PS5 controller, records the video, presses submit.
- Fable (Claude, in the Claude app): design, briefs, this log.
- Console (Claude Code in a terminal): builds inside Unreal through Unreal MCP.
- Codex: art and sound through the generation tools, and build checks.
- Cursor: on the bench as a reserve builder.

**The experiment.** No asset packs. Everything the player sees and hears is either generated with the jam partners' tools (Tripo, Rodin, Meshy, PBRgen, fal) or built by the agents in the engine. We want to find out how far that gets one person in four days, and where it falls over.

**How the agents don't trip over each other.** They can't talk to each other and none of them can wake another, so they share three files:
- a **board** (`Board\BOARD.md`): who owns which task and which assets;
- a **journal** (`Board\JOURNAL.md`): what was just done, what's half-done, what's next, so the next agent can carry on when one runs out of usage;
- a **baton**: only the agent holding it may change the editor. Unreal's MCP server runs one call at a time, and two agents editing at once wreck each other's work.

**What was set up today.**
- A blank Unreal Engine 5.8.3 project, Blueprint-only.
- Unreal MCP switched on (two plugins, auto-start, port 8000), with client settings for Claude Code and Cursor.
- Hardware ray tracing switched off. The dev machine is a laptop with an RTX 2050 and 4 GB of video memory; if it doesn't run here, it doesn't ship.
- A ledger for every prompt and generated file, so we can show exactly what was made by which tool.
- The rules read end to end (all 16 pages), and a one-page design template with only three "must ship" slots.

**Later that day.**
- MCP worked on the first open: 52 toolsets. The Claude app couldn't reach the editor at first, because the app had started before the editor did. Fix: editor first, then restart the app.
- The partner email with the tool codes never arrived. Tripo, Meshy and WeLoveIndies don't need it; the rest wait.

**21:00, the theme: "Director's Cut".** The chat's verdict was "so, anything". We read it as a test: when a thousand teams can generate a game in a prompt, what does a directed one look like?

**How we picked.** Six ideas in forty minutes. The first, a film set where you replay one scene as actor, effects rigger and camera operator alongside your own earlier takes, was the most exciting and too big for one person. We chose *Final Cut*: you get a game with everything in it and cut it down, and each cut removes the ability and its half of the world. PC asked the right question: how many other teams will an AI hand this same idea to? Probably dozens. So the twist carries it: **everything you cut comes back as the final boss.**

**The look, chosen for the tools:** a tabletop diorama of painted wind-up toys. Rigid figures that hop and wobble need no skeletal rigging, which is exactly where generated 3D models are weakest.

**What we're nervous about:** scope, a 4 GB video card, and five different AI tools that each export a slightly different idea of what a metre is.

**22:10, a correction from PC.** The first draft leaned on film: a boss called The Outtake, scissors, strips of film. PC called it on the nose, and he was right. "Director's Cut" in game terms means a game director cutting scope. So the world is now a toy prototype on a developer's desk, the cuts are sticky notes crumpled into the bin, and the boss that climbs out of the bin is **Feature Creep**.
