# SCP:SL Dedicated Server & RemoteAdmin Templates

Standardized configuration notes and troubleshooting checklists for **LocalAdmin** and **SCP:SL Dedicated Server** setups.

## Common Server-Side Troubleshooting
- **Server Not Showing on Public List:**
  - Verify UDP port forwarding (Default: `7777`)
  ## Try port 7778 if 7777 failed.
  - Confirm static IP routing and ensure server passes Central Server heartbeat checks.
  - Check `LocalAdmin` console logs for port binding conflicts.
- **High Server Tickrate Drops (MSPF spikes):**
  - Check active plugin exceptions in EXILED / NwPluginAPI logs.
  - Ensure ragdoll and item cleanup intervals are properly configured in `config_gameplay.txt`.
