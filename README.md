# GitHub Copilot Home Assistant Setup Helper

This agent helps you discover and create tailored solutions to your specific home assistant setup.

I use it primarily to create and update automations whenever I need a new one or don't have the care to fix a automation issue myself.

You'll need `RickyKleinhempel.homeassistant-mcp` extension to use this agent. This extensions allows Copilot to discover your entities.

## Customization

The agent is configured in [`.github/agents/home-assistant-config.agent.md`](.github/agents/home-assistant-config.agent.md). You can customize it to match your own preferences:

- **Language preferences** — Change entity ID and display name languages to match your HA setup
- **Naming conventions** — Adjust the entity naming patterns and emoji usage
- **Workflow preferences** — Modify how the agent discovers, designs, and archives configurations

Make a copy of the agent file and adjust the settings to suit your own Home Assistant environment.