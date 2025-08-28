# Claude Code Configuration

This file contains configuration and instructions for Claude Code CLI.

## Project Setup

- **Language**: Multiple (Python, Go, JavaScript/TypeScript, Terraform)
- **Environment**: Linux development environment with Kubernetes and cloud tools

## Common Commands

### Kubernetes Commands
- Set kubeconfig: `export KUBECONFIG=~/kubeconfigs/kubeconfig`
- Check cluster status: `kubectl get nodes`
- View pods: `kubectl get pods -A`

### Build & Test
- Run tests: `npm test` or `pytest` (depending on project)
- Build: `npm run build` or `go build` (depending on project)
- Lint: `npm run lint` or `golangci-lint run` (depending on project)

### Home Cluster Management
- READ operations with kubectl are fine for troubleshooting
- NO manual WRITE operations to cluster (no `kubectl apply`, `kubectl create`, etc.)
- All changes must go through GitFlow: push to home-cluster repo and ArgoCD picks up changes
- Cluster manifests located in `~/home-cluster/`

### Development Preferences
- Use 2-space indentation for YAML
- Prefer `kubectl` over `k` alias for clarity
- Always check git status before commits

### Development
- Start dev server: `npm run dev` or `go run main.go` (depending on project)
- Format code: `npm run format` or `gofmt -w .` (depending on project)

## Notes

This configuration file helps Claude Code understand the development environment and common workflows.