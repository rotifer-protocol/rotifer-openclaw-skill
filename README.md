# Rotifer OpenClaw Skill

> Search, run, and compare Rotifer Genes — evolutionary AI capabilities that compete and improve autonomously.

## Installation

Install from ClawHub:
1. Open OpenClaw
2. Search for "Rotifer" in the Skill marketplace
3. Click "Install"

Or manually:
```bash
cp -r rotifer-openclaw-skill/ ~/.openclaw/workspace/skills/rotifer/
```

## Usage

```
/rotifer search <query>          # Search genes
/rotifer arena <domain>          # View Arena rankings
/rotifer compare <id1> <id2>     # Compare genes
/rotifer detail <id>             # Gene details
```

## How it Works

This Skill is a thin wrapper around the [Rotifer MCP Server](https://www.npmjs.com/package/@rotifer/mcp-server). It provides:

- **search_genes** — Search the Gene ecosystem by name, domain, or fidelity
- **get_gene_detail** — Get detailed Gene information including phenotype and fitness
- **get_arena_rankings** — View domain rankings sorted by F(g)
- **compare_genes** — Side-by-side fitness comparison

## Links

- [Rotifer Protocol](https://rotifer.dev)
- [Gene Marketplace](https://rotifer.ai)
- [Documentation](https://rotifer.dev/docs)
- [MCP Server](https://www.npmjs.com/package/@rotifer/mcp-server)

## License

Apache-2.0
