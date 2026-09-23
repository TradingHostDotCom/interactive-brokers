# TradingHost + Interactive Brokers

Build and deploy professional multi-asset trading bots (stocks, options, futures, forex) via IB Gateway using [TradingHost](https://tradinghost.com).

## What is this?

This repository is an AI-powered development scaffold. Use it as a template (click "Use this template" on GitHub), open your new repo in your AI coding tool (Cursor, Claude, Codex), and tell the AI what you want to build. The rules in `.cursor/rules/` teach the AI everything it needs to know about Interactive Brokers and TradingHost to help you create a production-quality trading bot.

Interactive Brokers provides access to 150+ markets in 34 countries — stocks, options, futures, forex, bonds, funds, and more. The `ib_insync` library gives you a clean async Python API on top of IB's TWS/Gateway API.

## Getting Started

1. **Click "Use this template"** → Create a new repository (you can make it private)
2. **Open in Cursor** (or your preferred AI coding tool)
3. **Tell the AI what to build** — e.g. "Build me an options wheel strategy for AAPL and MSFT"
4. **Configure** — set your IB Gateway address (`ib_host`, `ib_port`, `ib_client_id`) in `config.json`. These are non-secret connection tunables; IB authentication happens at your Gateway, so no API secret is stored on TradingHost.
5. **Deploy on TradingHost** — link this repo as a strategy, create a deployment, and you're live

## Important: IB Gateway

IB Gateway (or TWS) must run somewhere your TradingHost deployment can reach — your own VPS, home machine with port forwarding, or a separate cloud instance. TradingHost runs your strategy code; your IB Gateway provides the broker connection.

## TradingHost Deployment

1. Create an account at [tradinghost.com](https://tradinghost.com)
2. Link this GitHub repository as a strategy
3. Create a deployment (choose region closest to your IB Gateway)
4. Your bot runs 24/7 with persistent storage, monitoring, and real-time logs

## Documentation

- [TradingHost Docs](https://tradinghost.com/docs)
- [ib_insync Documentation](https://ib-insync.readthedocs.io)
- [Interactive Brokers API](https://interactivebrokers.github.io)

## Risk Warning

Trading stocks, options, futures, and forex involves significant risk of loss. Options sellers face theoretically unlimited risk. This software is provided as-is with no guarantees. Always test with IB's paper trading account before going live.
