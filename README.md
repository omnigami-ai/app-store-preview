# App Store preview · omnigami

Your iPhone app’s store preview, and a promo of the same story.

One film, two cuts, from your app’s real screens. The store cut is prepared to Apple’s preview specifications: only your app, full frame, short captions and fingertip touches. The social cut tells the same moments on a dark ground in your colours, with chapters, headlines, your app in a phone, a recap and an end card.

Watch it play live, and change its words, at [omnigami.ai/skills/app-store-preview](https://omnigami.ai/skills/app-store-preview).

## Install

In Claude Code:

```
/plugin marketplace add omnigami-ai/skills
/plugin install app-store-preview@omnigami
```

With the skills CLI, for Claude Code and other agents that read SKILL.md:

```bash
npx skills add omnigami-ai/app-store-preview
```

Or copy `skills/app-store-preview/` into your agent's skills folder (for Claude Code, `~/.claude/skills/app-store-preview/`). Then ask:

```
Make an App Store preview for my iPhone app
```

## What it runs

The skill works on your computer. It runs the Node scripts in `skills/app-store-preview/scripts/`: they open your product's pages in a local headless browser to capture its real screens, then render the film with that browser and ffmpeg, writing MP4s and an editable HTML film to your project. It sends nothing to omnigami or anyone else, and uses no network beyond loading your own product's pages and the fonts and assets in this folder.

## You need

- Claude Code with Opus 5.5
- Node 20 or later
- ffmpeg
- Chrome, Chromium, Edge or Brave

None beyond your Claude plan’s usage. Node, ffmpeg and the browser are free. Submitting a preview needs your Apple developer account; Apple decides what it accepts.

## Licence

Free to use. Use the films and anything else the skill makes for anything, commercial work included. Don't redistribute the skill. See [LICENSE.md](LICENSE.md). The bundled fonts keep their own licence (SIL Open Font License, beside them in `reference/assets/fonts/`).

## Credits

Style inspired by @wallacex227’s video (https://x.com/wallacex227/status/2103245000989659422); @wallacex227 didn’t make or endorse this skill. Its example shows Fernwise, a fictional company made for omnigami’s examples, with sample data.

omnigami is not affiliated with Anthropic. More skills at [omnigami.ai](https://omnigami.ai).
