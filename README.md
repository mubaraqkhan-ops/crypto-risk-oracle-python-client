# Crypto Risk Oracle: Python API Client

A lightweight Python client for interacting with the **Mindcare Institutional Risk Oracle**. 

This tool is designed for quantitative developers and algorithmic traders who need to integrate real-time technical risk controls—such as Order Book Imbalance (OBI) and Liquidity Wall detection—directly into their trading daemons.

## Overview
Automated trading requires strict risk management to survive high-volatility liquidation events. Instead of building complex WebSocket aggregators from scratch to monitor order book depth across multiple exchanges, this API provides a unified, cryptographically verified risk verdict in milliseconds.

Use this API to confidently manage position sizing and dynamic trailing stop-loss mechanisms based on institutional-grade market data.

## Features
* **Multi-Exchange Aggregation:** Automatically pools liquidity data from Binance and Bybit.
* **Key Control Indicators (KCIs):** Audits real-time Funding Rates, Volatility, and Volume.
* **OBI Scoring:** Detects Buy/Sell walls before you execute a market order.
* **Cryptographic Proof:** Every API response is ECDSA-signed for immutable audit trails.

## 📖 Complete Documentation
**[Read the full API Reference and Integration Guide Here](https://doc.mindcare.agency)**

## Quick Start

This API utilizes the `x402` machine-to-machine payment protocol on the Base network. No traditional API keys or monthly subscriptions are required—you only pay $0.05 per successful audit via smart contract.

### Installation
```bash
pip install httpx pydantic
