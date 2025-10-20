# LinkUp API Documentation

This repository contains the documentation for LinkUp API with support for multiple versions.

## 📁 Structure

```
mintlify-docs/
├── mint.json              # Main configuration (points to v2 by default)
├── v1/                    # Version 1.0 documentation
│   ├── mint.json         # v1.0 specific configuration
│   └── api-reference/    # v1.0 API documentation
├── v2/                    # Version 2.0 documentation
│   ├── mint.json         # v2.0 specific configuration
│   └── api-reference/    # v2.0 API documentation
├── logo/                  # Shared assets
├── images/               # Shared images
└── package.json          # Build scripts
```

## 🚀 Development

### Run All Versions
```bash
# Main documentation (v2 by default)
npm run dev

# Preview all versions simultaneously
npm run preview        # Main docs on :3000
npm run preview:v1     # v1.0 docs on :3001
npm run preview:v2     # v2.0 docs on :3002
```

### Run Specific Version
```bash
# Version 1.0
npm run dev:v1

# Version 2.0  
npm run dev:v2
```

## 🏗️ Building

```bash
# Build all versions
npm run build

# Build specific version
npm run build:v1
npm run build:v2
```

## 📚 Version Management

### Current Versions
- **v2.0** (Latest): Full-featured API with enhanced capabilities
- **v1.0** (Legacy): Original API, deprecated December 2024

### Adding a New Version

1. Create a new version directory (e.g., `v3/`)
2. Copy the latest version as a starting point
3. Update the `mint.json` configuration
4. Add the new version to the main `mint.json` versions array
5. Update navigation paths in the main configuration

### Version Configuration

Each version has its own `mint.json` with:
- Version-specific navigation
- API base URLs
- Version-specific content

## 🔄 Migration Between Versions

Users can switch between versions using the version selector in the documentation interface. Each version maintains its own:
- API endpoints and base URLs
- Documentation structure
- Examples and code snippets
- Migration guides

## 📖 Content Guidelines

### Version-Specific Content
- Keep breaking changes and new features in version-specific sections
- Maintain migration guides between versions
- Update examples to reflect version-specific syntax

### Shared Content
- Logo and branding assets
- General company information
- Contact and support information

## 🚀 Deployment

The documentation supports Mintlify's native versioning system:
- Main domain shows the latest version (v2.0)
- Previous versions accessible via `/v1/` path
- Version selector allows easy switching

## 📞 Support

For questions about the documentation:
- Technical issues: [GitHub Issues](https://github.com/linkupapi/docs)
- API questions: [Support Portal](https://app.linkupapi.com/support)
- Community: [Discord](https://discord.gg/linkupapi)