# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Purpose

Backup repository for an OPML file containing RSS feed subscriptions for the "Don't Hype Me" RSS reader project. This is a data-only repo — no source code, build system, or tests.

## Structure

- `donthypeme-feeds.opml` — OPML 2.0 XML file with RSS feeds organized into categories: Tech, YouTube, Reddit, News, plus one uncategorized top-level feed

## OPML Format

When editing the feed list, follow the existing XML structure:
- Feeds use `<outline type="rss" text="Feed Name" xmlUrl="https://..." />`
- Categories are `<outline text="Category Name">` wrappers containing feed outlines
- Uncategorized feeds go directly under `<body>`
- Maintain XML encoding for special characters (`&amp;`, `&apos;`, `&quot;`)
