# Claude Code Configuration

This file contains configuration and instructions for Claude Code CLI.

## Project Setup

- **Language**: Multiple (Python, Go, JavaScript/TypeScript, Terraform)
- **Environment**: Linux development environment with Kubernetes and cloud tools

## Common Commands

### Kubernetes
- Set kubeconfig: `export KUBECONFIG=~/kubeconfigs/kubeconfig`

### Build & Test
- Run tests: `npm test` or `pytest` (depending on project)
- Build: `npm run build` or `go build` (depending on project)
- Lint: `npm run lint` or `golangci-lint run` (depending on project)

### Development
- Start dev server: `npm run dev` or `go run main.go` (depending on project)
- Format code: `npm run format` or `gofmt -w .` (depending on project)

## Notes

This configuration file helps Claude Code understand the development environment and common workflows.