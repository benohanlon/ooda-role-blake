# Run the first Emissary review in Hermes

1. Select the Blake profile and connect the operator's private role application. Add this checkout's absolute `skills/` path to `skills.external_dirs` in that profile. Verify which copy Hermes resolves for `/emissary`. An existing local or project skill can take precedence.
2. Install [Hermes Teammates](https://hermes-agent.nousresearch.com/marketplace/hermes-teammates) for Blake and [Pixel HQ](https://hermes-agent.nousresearch.com/marketplace/pixel-hq) for the Hermes Desktop backend that will observe the run. Check each listing against the installed Hermes version and record the plugin revisions actually tested.
3. Copy [the roster example](teammates.example.yaml) into Blake's Hermes profile home as `teammates.yaml`. Merge these keys into the existing profile config. Check the effective worker toolsets and confirm the roster before sharing private evidence.

```yaml
delegation:
  inherit_mcp_toolsets: false
plugins:
  entries:
    hermes-teammates:
      settings:
        roster_file: teammates.yaml
```

The example reviewer needs only the evidence Blake includes in the assignment. The roster limits the reviewer to the built-in `todo` toolset. Keep that toolset available to Blake and check the effective restriction during the trial.

4. In Blake's session, use `/emissary` on one existing priority report or the [synthetic example](../examples/private-context.example.md). Have Blake dispatch one review, record its run ID, reconcile the response and return the shortlist. In Pixel HQ, check whether the teammate appears under Blake while running, whether the activity is attributable and whether the operator can tell when intervention is needed. Confirm the result in Teammates even if Pixel HQ misses a short run.

Keep the working roster, installed profile config and runtime files outside the public checkout. The Teammates SQLite ledger lives in the profile's plugin data on the Hermes host. Pixel HQ reads Hermes activity and Kanban data available to its backend. The trial establishes what it can see on this installation.

[Hermes external skill directories](https://hermes-agent.nousresearch.com/docs/user-guide/features/skills#external-skill-directories) · [Teammates roster and toolsets](https://hermes-agent.nousresearch.com/marketplace/hermes-teammates) · [Pixel HQ data and runtime requirements](https://hermes-agent.nousresearch.com/marketplace/pixel-hq)
