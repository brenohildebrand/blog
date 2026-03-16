+++
date = '2026-03-16T12:39:52-04:00'
draft = false
title = 'How Claude Code Created This Blog (And Why That Is Amazing)'
tags = ['claude', 'ai', 'hugo', 'meta']
description = 'I asked an AI to build my blog from scratch. Here is exactly what happened.'
+++

I have been meaning to start a blog for years. The usual excuses: too busy, not sure which platform to use, don't want to deal with the setup. Then I tried Claude Code, and the blog you're reading right now went from zero to running in under five minutes.

Here's exactly what happened.

## "Create a Hugo blog for me"

That was essentially the whole prompt. I opened my terminal, navigated to an empty folder, and told Claude Code to set up a Hugo blog with the PaperMod theme and explain how to publish it.

What followed was genuinely impressive. Without any further input from me, it:

- Detected that Hugo wasn't installed and ran `brew install hugo`
- Initialized a new Hugo site in my project folder
- Initialized a git repository and added PaperMod as a proper git submodule
- Wrote a complete `hugo.toml` config with sensible defaults — dark/light mode, reading time, table of contents, navigation menus, social icons
- Created a sample blog post and an About page
- Ran `hugo --minify` to verify the build succeeded
- Explained three different ways to publish the site

No errors. No back-and-forth. It just worked.

## What makes this different

I've used AI assistants to help with code before. Usually it means copying a snippet, pasting it somewhere, watching it fail, and then asking follow-up questions for the next twenty minutes.

Claude Code is different because it operates directly in your terminal with access to your filesystem and shell. It doesn't just suggest commands — it runs them. It doesn't just generate files — it creates them in the right place with the right content. It sees the output of every command it runs and adjusts if something goes wrong.

It's less like asking a chatbot for help and more like pairing with a developer who can type faster than you.

## The moment that stuck with me

After setting everything up, I said: "change the title of the blog to Breno Hildebrand."

One edit, done, no explanation needed. It knew exactly which file, which line, and what to change. That kind of contextual awareness — remembering what it just built, knowing where everything lives — is what separates this from a generic AI assistant.

## What I actually had to do

Honestly? Very little. I updated a few things in `hugo.toml`:

- My name and description
- My actual domain instead of `example.com`
- My GitHub link

That's it. The structure, the theme configuration, the git setup — all handled.

## Should you try it?

If you've been putting off starting a blog, a project, or any kind of setup task because the initial friction felt too high — yes, try it. Claude Code is available as a CLI tool and the barrier to entry is low.

The best part isn't that it saved me time (though it did). It's that it removed the excuse. There's no more "I'll set it up someday." Someday is now five minutes away.

And now I have a blog.
