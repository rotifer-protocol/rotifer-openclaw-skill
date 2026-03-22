---
name: rotifer
version: 1.0.0
description: Search, run, and compare Rotifer Genes — evolutionary AI capabilities that compete and improve autonomously
author: rotifer-protocol
permissions:
  - network:outbound
triggers:
  - command: /rotifer
mcp:
  server:
    command: npx
    args:
      - "@rotifer/mcp-server"
---

# Rotifer Gene Ecosystem

Access the [Rotifer Protocol](https://rotifer.dev) Gene ecosystem directly from OpenClaw. Search, compare, and discover AI capabilities (Genes) that evolve through natural selection.

## What is Rotifer?

Rotifer is an evolution framework for autonomous AI agents. Instead of static tool lists, Rotifer introduces **Genes** — atomic capabilities that compete in an **Arena**. The fittest Genes (measured by the fitness function **F(g)**) survive and are automatically selected by Agents.

## Available Commands

### Search Genes
Find Genes by name, domain, or description:
```
/rotifer search web scraping
/rotifer search --domain code.format
/rotifer search --fidelity Native
```

### Compare Genes
Compare multiple Genes side by side on fitness metrics:
```
/rotifer compare <gene-id-1> <gene-id-2>
```

### Arena Rankings
View the top-performing Genes in a domain:
```
/rotifer arena search.web
/rotifer arena code.format
```

### Get Gene Details
View full details about a specific Gene:
```
/rotifer detail <gene-id>
```

## Gene Types (Fidelity)

| Fidelity | Description |
|----------|-------------|
| **Native** | Pure WASM — fully sandboxed, highest security |
| **Hybrid** | WASM logic + controlled external calls |
| **Wrapped** | Thin envelope around an external API |
| **Unknown** | Forward-compatibility fallback |

## Fitness Function F(g)

Genes are ranked by an objective, data-driven fitness function:

```
F(g) = [S_r · ln(1 + C_util) · (1 + R_rob)] / [L · Resource_Cost]
```

No voting, no human preference — pure runtime performance metrics.

## Links

- [Developer Portal](https://rotifer.dev)
- [Gene Marketplace](https://rotifer.ai)
- [Documentation](https://rotifer.dev/docs)
- [Protocol Specification](https://github.com/rotifer-protocol/rotifer-spec)
