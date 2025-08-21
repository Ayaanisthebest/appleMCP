# Apple MCP - Enhanced Edition

> **Enhanced by [@Ayaanisthebest](https://github.com/Ayaanisthebest)**  
> Based on the original work by [supermemoryai/apple-mcp](https://github.com/supermemoryai/apple-mcp)

## Overview

This enhanced version of Apple MCP extends the original [supermemoryai/apple-mcp](https://github.com/supermemoryai/apple-mcp) repository with additional features and improvements. The original project provides a comprehensive Model Context Protocol server for Apple ecosystem integration, enabling AI assistants to interact with native Apple applications.

## Enhanced Features

### Smart Contact Resolution
- Automatic contact name to phone number resolution in the Messages tool
- Eliminates manual contact lookup requirements before messaging
- Intelligent phone number parsing with international format preference

### Enhanced Notes Management
- Priority-based search algorithm prioritizing title matches over content
- Visual indicators for search result types (Title Match vs Content Match)
- Full support for Apple Notes rich text formatting and structure
- Advanced note editing capabilities with format preservation

### Improved Error Handling
- Enhanced validation and user-friendly error messaging
- Comprehensive error guidance and troubleshooting
- Advanced debugging and logging capabilities

### Developer Experience Improvements
- Enhanced TypeScript interfaces and type validation
- Improved code organization and maintainability
- Comprehensive debugging and development tools

## Core Functionality

### Messages
- Send messages using contact names with automatic phone number resolution
- Access message history and conversation threads
- Schedule messages for future delivery
- Enhanced error handling and validation

### Notes
- Advanced search with priority-based result ranking
- Rich text creation and editing with full formatting support
- Note organization and folder management
- Content modification while preserving formatting

### Contacts
- Comprehensive contact search and retrieval
- Phone number and email address management
- Required integration step for messaging operations

### Mail
- Email composition with attachment, CC, and BCC support
- Advanced email search and filtering
- Scheduled email delivery
- Unread message monitoring

### Reminders
- Task creation with due date management
- Advanced reminder search and organization
- Comprehensive reminder listing and management
- Direct reminder access and modification

### Calendar
- Event creation and management
- Advanced calendar search capabilities
- Meeting and appointment scheduling
- Direct calendar event access

### Maps
- Location search and discovery
- Favorite location management
- Route planning and navigation
- Location guide creation and pin management

## Installation

### Option 1: Smithery Integration
```bash
npx -y install-mcp apple-mcp --client claude
```

For Cursor IDE users:
```bash
npx -y install-mcp apple-mcp --client cursor
```

### Option 2: Manual Configuration
```bash
brew install oven-sh/bun/bun
```

Add to your `claude_desktop_config.json`:
```json
{
  "mcpServers": {
    "apple-mcp": {
      "command": "bunx",
      "args": ["--no-cache", "apple-mcp@latest"]
    }
  }
}
```

## Usage Examples

```
"Send a message to John regarding the delayed dinner arrival"
"Search notes for 'AI research' and display results"
"Create a reminder for dental appointment tomorrow at 2:00 PM"
"Display calendar events for next week"
"Locate nearest coffee establishment and add to favorites"
```

## Development Setup

```bash
git clone https://github.com/Ayaanisthebest/appleMCP.git
cd appleMCP
bun install
bun run index.ts
```

## Acknowledgments

### Original Development Team
This project builds upon the foundation established by the [supermemoryai/apple-mcp](https://github.com/supermemoryai/apple-mcp) development team:
- [@Dhravya](https://github.com/Dhravya) - Project founder and principal developer
- [@jxnl](https://github.com/jxnl) - Core architecture and development
- [@calclavia](https://github.com/calclavia) - Development and testing
- The complete supermemory team for ongoing project support

### Enhancement Development
Additional features and improvements developed by [@Ayaanisthebest](https://github.com/Ayaanisthebest)

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for complete license terms.

---

For additional information about the original project, visit: https://mcp.supermemory.ai
