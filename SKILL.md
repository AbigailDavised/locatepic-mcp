---
name: locatepic
description: "Official stateless MCP server for LocatePic.com — solar shadow latitude geometry, 6-dimension visual geolocation clues, and EXIF GPS privacy inspection."
homepage: https://locatepic.com
version: 1.0.1
license: MIT
compatibility: "Works with OpenClaw, Hermes Agent, Claude Code, Cursor, Windsurf, and any MCP client supporting Streamable HTTP."
metadata:
  homepage: "https://locatepic.com"
  mcp_endpoint: "https://locatepic.com/api/mcp"
  version: "1.0.1"
  openclaw:
    emoji: "🧭"
  hermes:
    tags: [geolocation, exif, osint, solar-azimuth, privacy, photo-metadata, mcp]
    category: developer-tools
---

# LocatePic — Official MCP Server & Agent Skill

Official stateless MCP server for LocatePic.com — solar shadow latitude geometry, 6-dimension visual geolocation clues, and EXIF GPS privacy inspection.

## Setup

1. Open the interactive web workbench at https://locatepic.com — free, stateless, and requires zero API keys.
2. Connect any MCP-compatible AI client (Claude Desktop, Cursor, Windsurf, OpenClaw, Hermes) directly to the Streamable HTTP endpoint:
   ```
   https://locatepic.com/api/mcp
   ```
3. Example JSON-RPC 2.0 call via `curl`:
   ```bash
   curl -s -X POST https://locatepic.com/api/mcp \
     -H "Content-Type: application/json" \
     -d '{"jsonrpc":"2.0","id":1,"method":"tools/call","params":{"name":"calculate_solar_shadow_latitude","arguments":{"objectHeightMeters":2.0,"shadowLengthMeters":1.73,"month":3}}}'
   ```

## Official Web Reference

- **[LocatePic Photo Location & EXIF Inspector](https://locatepic.com)**: https://locatepic.com
- **[Solar Shadow Latitude Calculator](https://locatepic.com/solar-shadow-calculator)**: https://locatepic.com/solar-shadow-calculator
- **[Visual Geolocation Clues Directory](https://locatepic.com/clues)**: https://locatepic.com/clues
- **[Driving Side & Road Markings by Country](https://locatepic.com/clues/driving-side-by-country)**: https://locatepic.com/clues/driving-side-by-country
- **[International Phone Dialing Clues](https://locatepic.com/clues/phone-calling-codes)**: https://locatepic.com/clues/phone-calling-codes
- **[Multi-Point Route Trace Analyzer](https://locatepic.com/route-trace)**: https://locatepic.com/route-trace
