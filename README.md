# DiscordMCP

**Manage your Discord server by telling Claude or ChatGPT what you want.**

Create channels, hand out roles, set permissions, post announcements — in the
assistant you already use, in plain language. No console, no bot programming,
no second dashboard to learn.

### → **[discordmcp.com](https://discordmcp.com)**

---

## What it actually is

A hosted [Model Context Protocol](https://modelcontextprotocol.io) server for
Discord. You paste your bot token once, click once, and get an address to add
to Claude or ChatGPT as a custom connector. From then on you type *"make a
channel for the tournament and let only the Verified role in"* and it happens.

**One server, one bot, one process.** Your instance is yours: its own
subdomain, its own bot token, its own log channel. It is not a shared service
with your server as a row in somebody's table.

## What it can do

**Read** — the server at a glance, channels, roles, members, messages,
permissions, reactions, emoji, pins, bans, threads, invites, events, the audit
log.

**Change** — create and edit channels and roles, move roles, hand them out and
take them back, post and edit messages, polls, reactions, pins, threads,
invites and scheduled events.

**Ask first** — deleting a channel, a message or a role, kicking, timing out,
banning, clearing reactions, revoking an invite, cancelling an event. Every
one of these is **off until you switch it on**, per server, with the exact
wording you agreed to recorded.

The dividing line is not how alarming a word sounds. It is whether the thing
can be put back.

## What it deliberately does not do

Mass removal, bulk deletion, anything that empties a server in one call. Not
"not yet" — those tools do not exist, so nothing anybody writes in a channel
topic can reach them.

That matters more than it sounds: what decides to call a tool is a language
model reading text other people wrote. A tool that is not there cannot be
talked into running, however the request is phrased.

## How it is built, in four lines

- **No dependencies.** Not a short list — none. The machine that holds
  customers' bot tokens installs nobody else's code.
- **No gateway connection.** REST only. Your bot gets no second presence.
- **The portal does not keep your token.** It passes through on its way to
  your instance and is erased the moment the instance confirms it started.
  What remains is a fingerprint — enough to notice it changed, not enough to
  use it.
- **Everything is written into your own log channel.** Refusals too. An
  attempt that Discord rejected is the more interesting line of the two.

## Price

**$6 a month or $60 a year**, up to 2 Discord servers, every tool included.
Cancel anytime.

There is an open beta running: finish the setup during it and you get a free
month, and it runs its full length even past the end of the beta.

## Where to go

- **[discordmcp.com](https://discordmcp.com)** — what it does, what it costs,
  and the setup
- **[discordmcp.com/faq](https://discordmcp.com/faq)** — the questions people
  actually ask
- **[discordmcp.com/guide/claude](https://discordmcp.com/guide/claude)** —
  adding it as a connector in Claude, step by step
- **[discordmcp.com/guide/chatgpt](https://discordmcp.com/guide/chatgpt)** —
  the same for ChatGPT

## About this repository

It holds no source code and is not meant to. DiscordMCP is a hosted service,
not something you run yourself, and this is here so that somebody searching
for a Discord MCP server can find it.

Questions, problems and feature requests are welcome as
[issues](https://github.com/Nicras/discord-mcp-public/issues) — or through the
support server linked on the site, which is usually faster.
