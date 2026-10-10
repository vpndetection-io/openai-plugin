# [<img src="https://s3.vpndetection.io/vpndetection-public/brand/mark.svg" alt="VPNDetection" height="28"/>](https://vpndetection.io/) VPNDetection Plugin for ChatGPT and Codex

[![version](https://img.shields.io/github/package-json/v/vpndetection-io/openai-plugin?filename=plugin.json)](CHANGELOG.md)
[![license](https://img.shields.io/github/license/vpndetection-io/openai-plugin)](LICENSE)

The official [VPNDetection](https://vpndetection.io) plugin for [ChatGPT](https://chatgpt.com) and [Codex](https://developers.openai.com/codex).

## Getting Started

In Codex:

```console
codex plugin marketplace add vpndetection-io/openai-plugin
codex plugin add vpndetection@vpndetection
codex mcp login vpndetection
```

The last line signs you in with your VPNDetection account, where you pick the API key Codex should use. Codex never sees the key: our MCP server uses it on your behalf. The Codex CLI, its IDE extension and Codex in the ChatGPT desktop app read the same configuration, so one install covers all three.

To disconnect Codex, run `codex mcp logout vpndetection`, or remove it under Connected applications at https://app.vpndetection.io/settings/account/sessions. Access ends within about a minute.

## What's in it

- The VPNDetection MCP server at `https://mcp.vpndetection.io/mcp`.

## What it sends

The plugin runs nothing on your machine. Codex sends what you ask about to `https://mcp.vpndetection.io/mcp`, which calls the VPNDetection API with the key you picked and returns the answer. Each request is logged against that key as any API call is. Our privacy policy is at https://vpndetection.io/privacy, and questions go to support@vpndetection.io.

## Other Libraries

There are official VPNDetection client libraries available for many languages including PHP, Python, Go, Java, and Ruby. See our GitHub at https://github.com/vpndetection-io for more.

## About VPNDetection

VPN Detection API: Accurate anonymity detection identifying VPNs, residential proxies, hosting servers, Tor nodes, CDNs, relays and more.

[<img src="https://s3.vpndetection.io/vpndetection-public/brand/mark.svg" alt="VPNDetection" height="64"/>](https://vpndetection.io/)

## License

This project is licensed under the [MIT License](LICENSE).
