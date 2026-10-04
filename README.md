# GHL Appointment Setter

**Chat assistant that qualifies inbound leads, collects contact details and books calls straight into a GoHighLevel calendar.**

> **This is a proprietary project. Source code is private. This page showcases the system's architecture and results.**

**Case study page:** [https://jryahia.github.io/showcase-ghl-appointment-setter/](https://jryahia.github.io/showcase-ghl-appointment-setter/)

![GHL Appointment Setter](assets/00-api-dashboard.png)

## Problem it solves

Inbound leads go cold while waiting for a human to qualify and schedule them. This assistant handles the first conversation, offers real open slots and creates the contact and event in GoHighLevel.

## Architecture

![Architecture](assets/architecture.svg)

1. A visitor opens the chat widget and answers qualification questions.
2. Available slots are generated from business hours, minus conflicts and blackout dates.
3. The lead picks a slot; the contact and event are created in GoHighLevel.
4. Every conversation and booking is logged.

## Key features

- Conversational booking flow
- Slot generation with conflict and blackout handling
- GoHighLevel contact and calendar integration
- LLM qualification with a rule-based fallback
- Demo mode with mock GHL responses

## Tech stack

![Python](https://img.shields.io/badge/Python-161b22?style=for-the-badge&labelColor=161b22&color=161b22) ![FastAPI](https://img.shields.io/badge/FastAPI-161b22?style=for-the-badge&labelColor=161b22&color=161b22) ![SQLAlchemy](https://img.shields.io/badge/SQLAlchemy-161b22?style=for-the-badge&labelColor=161b22&color=161b22) ![GoHighLevel API](https://img.shields.io/badge/GoHighLevel%20API-161b22?style=for-the-badge&labelColor=161b22&color=161b22) ![OpenAI / DeepSeek](https://img.shields.io/badge/OpenAI%20/%20DeepSeek-161b22?style=for-the-badge&labelColor=161b22&color=161b22) ![Jinja2](https://img.shields.io/badge/Jinja2-161b22?style=for-the-badge&labelColor=161b22&color=161b22)

## What it does in practice

- Covers the first-contact and scheduling step that would otherwise need a human SDR.

## Screenshots

**Leads, upcoming appointments and open slots**

![Leads, upcoming appointments and open slots](assets/00-api-dashboard.png)

**Booking assistant chat widget**

![Booking assistant chat widget](assets/11-chat.png)

---

Built by [Yahya Jarray](https://github.com/jryahia). Interested in a similar system? [Get in touch](mailto:yahiajarray43@gmail.com).
