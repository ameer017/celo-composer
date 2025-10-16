# Changelog

## [2.4.12] - 2025-10-16

### Changed
- Updated AI Chat template to use latest Gemini 2.5 models (gemini-2.5-flash and gemini-2.5-pro)
- Replaced deprecated Gemini 1.5 models with Gemini 2.5 versions for improved performance and capabilities

## [2.4.11] - 2024-10-16

### Fixed
- Fixed critical template path resolution bug when running CLI via npx
- Templates directory now correctly located whether running from dist/, dist/subdirectory/, or src/
- All template types (basic, farcaster-miniapp, minipay, ai-chat) now generate successfully when installed from npm
- Fixed development mode (pnpm dev) to correctly locate plopfile.ts instead of plopfile.js

## [2.3.5] - 2025-08-06

### Fixed
- Resolved file conflict issue during project generation by removing the base `connect-button.tsx.hbs` and ensuring wallet-specific templates are used.

## [2.3.4] - 2025-08-05

### Changed
- Updated docs config with SEO metadata and replaced favicon with new Celo logo.

## [2.3.3] - 2025-08-04

### Added
- Added wallet connection and miniapp installation UI to the Farcaster template.

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [2.2.4] - 2024-01-23

### Fixed
- Fixed runtime error "Cannot find module 'tsx/cjs'" when running published package
- Removed unnecessary tsx/cjs requirement from plop-generator
- CLI now works correctly when installed via npm/npx

## [2.2.3] - 2024-01-23

### Fixed
- Fixed GitHub Actions pnpm lockfile issues by removing --frozen-lockfile flag
- Improved CI/CD pipeline reliability for npm deployment

## [2.2.2] - 2024-01-23

### Internal
- Version bump for deployment testing

## [2.2.1] - 2024-01-23

### Fixed
- Fixed ESLint configuration for proper TypeScript support
- Resolved TypeScript linting errors and removed 'any' types
- Added proper type definitions for Plop.js data interfaces
- Updated test script to pass with no tests during development

### Added
- Complete GitHub Actions workflow for npm deployment
- CI/CD pipeline with automated testing and publishing
- Comprehensive deployment documentation
- Release automation script
- MIT License file

## [2.2.0] - 2024-01-XX

### Added
- Complete CLI tool for generating customizable Celo blockchain starter kits
- Support for multiple wallet providers (RainbowKit, Thirdweb)
- Hardhat smart contract development framework integration
- Modern UI with shadcn/ui components
- Monorepo structure with Turborepo
- Interactive prompts for project configuration
- Template-based project generation with Plop.js
- Support for Next.js 14+ with App Router
- TypeScript support throughout
- PNPM package manager integration

### Features
- **Wallet Integration**: Support for MetaMask, Trust Wallet, Valora, and in-app wallets
- **Smart Contracts**: Hardhat integration with Celo network configuration
- **Modern UI**: shadcn/ui components with responsive design
- **Monorepo**: Turborepo-based monorepo structure
- **Developer Experience**: Interactive CLI with progress indicators
- **Template System**: Modular template composition
- **Network Support**: Pre-configured for Celo mainnet and Alfajores testnet

### Technical Details
- Node.js 18+ support
- TypeScript strict mode
- ESLint configuration
- Jest testing framework
- Commander.js for CLI framework
- Inquirer.js for interactive prompts
- Plop.js for template generation

## [Unreleased]

### Planned
- Additional wallet provider integrations
- More smart contract templates
- Enhanced testing utilities
- Documentation improvements
- Performance optimizations

---

## Release Process

### Stable Releases
- Tagged as `v2.2.0`, `v2.3.0`, etc.
- Published to npm with `latest` tag
- Full GitHub releases with changelog

### Pre-releases
- Tagged as `v2.2.0-beta.1`, `v2.2.0-alpha.1`, etc.
- Published to npm with `beta`, `alpha`, or `rc` tags
- GitHub pre-releases for testing

### Installation
```bash
# Latest stable version
npm install -g @celo/celo-composer

# Beta version
npm install -g @celo/celo-composer@beta

# Specific version
npm install -g @celo/celo-composer@2.2.0
```
