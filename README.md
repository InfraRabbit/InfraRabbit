# InfraRabbit

**Every published compute price, archived daily.**

InfraRabbit keeps a daily archive of published list prices for compute, with history, price indices and a free MCP server. Data is CC BY 4.0.

## What we publish

- GPU instance hours, VPS plans and LLM API tokens, taken from each provider's own price page or API
- Price history with dated change points, plus a feed of price changes, new SKUs and delistings
- Daily price indices (H100/H200/B200 GPU hour, EU VPS, frontier and open LLM tokens)
- A read-only JSON API and a remote MCP server, no key needed
- CSV downloads and a Hugging Face dataset

## Links

- Site: [infrarabbit.com](https://infrarabbit.com)
- API docs: [infrarabbit.com/api](https://infrarabbit.com/api) · [llms.txt](https://infrarabbit.com/llms.txt)
- MCP server: [`InfraRabbit/mcp`](https://github.com/InfraRabbit/mcp)
- Indices: [infrarabbit.com/prices/indices](https://infrarabbit.com/prices/indices)
- Data: [`InfraRabbit/data`](https://github.com/InfraRabbit/data) · [CSVs](https://infrarabbit.com/prices/data) · [Hugging Face](https://huggingface.co/datasets/InfraRabbit/compute-prices)
- SDKs (Python, JavaScript): [`InfraRabbit/sdk`](https://github.com/InfraRabbit/sdk)
- Licensing: [infrarabbit.com/licensing](https://infrarabbit.com/licensing)

## Connect the MCP server

Remote streamable HTTP, no authentication:

```
https://infrarabbit.com/mcp
```

Claude Code:

```bash
claude mcp add --transport http infrarabbit https://infrarabbit.com/mcp
```
