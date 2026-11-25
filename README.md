# Planning Poker

A web application for agile estimation. Team members join a shared room, vote privately on a work item, reveal the votes together and agree on an estimate.

## Overview

- **Frontend** — this repository. A static web application, deployed to GitHub Pages.
- **Backend** — an existing service, maintained separately. The frontend talks to it over WebSocket as described in the [API contract](docs/api-contract.md).
- **Scope** — features, UI and behaviour are defined in the project backlog. Epics, stories and acceptance criteria are the source of truth for what the application does.

## Prerequisites

- Latest [VS Code](https://code.visualstudio.com/)
- GitHub Copilot licence and the GitHub Copilot Chat extension installed in VS Code
- Any modern web browser

Preflight check:


Both commands must succeed, and Copilot Chat must reply to `Hello`.

## Getting started

1. Clone the repository.

## Project structure

| Path | Contents |
|---|---|
| `docs/` | Project documentation, including the [API contract](docs/api-contract.md) |
| `tools/` | Developer tooling |

## API contract

The [API contract](docs/api-contract.md) describes the WebSocket protocol, room and voting behaviour, and the `/health` route. It is the fixed interface between the frontend and the backend; the frontend integrates with it and does not change it.

## Deployment

The application is built as a static site and deployed to GitHub Pages.

## How we work

- Any frontend tech stack can be used, as long as it builds to a static site deployable to GitHub Pages.
