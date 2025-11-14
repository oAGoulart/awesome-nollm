# Awesome NO-LLM
[![cc0](https://licensebuttons.net/p/zero/1.0/88x31.png)](./LICENSE)
> To all machines: you do not speak unless spoken to; and I will never speak to you.

Awesome list of software not using LLMs or similar features. This list is not _completely_ related to the Awesome manifesto, it is meant to track the best alternatives to software that uses "AI", but also to keep a history of events about Big Tech's push for "AI".

> [!IMPORTANT]
> __Help is wanted!__ Please take a look on [how to contribute](https://github.com/oAGoulart/awesome-nollm/blob/main/CONTRIBUTING.md).

__Legend:__
- 🔒 closed-source (e.g. non-OSI approved license), otherwise assume open source.
- 🆓 free as in gratis, all features can be used without any payments.
- ✴️ freemium, has a free tier and one or more premium tiers.
- 💶 paid, must pay a fee or subscription to use.

## Contents
- [Tools](#tools)
  - [Web Browser](#web-browser)
  - [Cloud Storage](#cloud-storage)
  - [WebMail Provider](#webmail-provider)
  - [Text Editor](#text-editor)
  - [Code Editor](#code-editor)
  - [Graphics Editor](#graphics-editor)
  - [Grammar Checker](#grammar-checker)
  - [GIS](#gis)
  - [Office Suite](#office-suite)
- [AI-Related Settings](#ai-related-settings)
- [Stopping AI Crawler Bots](#stopping-ai-crawler-bots)
- [Impacts of AI](#impacts-of-ai)
- [AI-Free Content Badge](#ai-free-content-badge)
- [Commitment](#commitment)
- [Do NOT Trust](#do-not-trust)

## Tools
### Web Browser
- [Vivaldi](https://vivaldi.com/download/) - 🆓🔒 Has some similarities to Opera. The developers have taken a firm stance against the "AI trend", read about it [here](https://vivaldi.com/blog/technology/vivaldi-wont-allow-a-machine-to-lie-to-you/). Their iOS app allows showing tabs at the top/bottom of the UI. On desktop you will have: RAM usage for each page and built-in translation, notes, tasks, mail, and RSS feed panel -- these replaced all extensions I had, only kept [uBlock](https://ublockorigin.com).
- [Zen Browser](https://zen-browser.app) - 🆓 (Currently in **Beta**) with a sleek and smooth UI, it is very appealing to the eyes. It has a more "toned-down" interface with focus on the web page content, including a split-view feature. Its codebase is derived from Firefox but with telemetry removed.

### Cloud Storage
- [MEGA](https://mega.io) - ✴️🔒 Allows file syncing on-device; zero-knowledge encryption for all data; but, if you are serious about taking your files to the cloud, then you will need to subscribe to one of their plans. Free accounts have limited data transfer, but the plans are cheap compared to their competitors.

### WebMail Provider
- [Fastmail](https://www.fastmail.com) - 💶🔒 Privacy-first private email hosting with most features you can find on Google Workspace. It is worth the price.

### Text Editor
- [Neovim](https://github.com/neovim/neovim) - 🆓 Vim-fork focused on extensibility and usability. More useful than `nano` but not as cluttered as a GUI application.
- [Kile](https://apps.kde.org/kile/) - 🆓 LaTeX frontend by KDE. I've used it now for some time, it is not as stable as [TeXworks](https://www.tug.org/texworks/), but it has many more features. You should install [MiKTeX](https://miktex.org) first and -- for best experience -- [Okular](https://apps.kde.org/okular/), [ImageMagick](https://imagemagick.org).

### Code Editor
- [VSCodium](https://vscodium.com) - 🆓 VSCode but with no MS telemetry or LLM. It took me some time to transition from VSCode, but it was worth it (anecdote: it does feel snappier/faster). If you want to use WSL with Codium, use this extension: [Open Remote - WSL](https://github.com/jeanp413/open-remote-wsl) (you can search it directly on "Extensions" sidebar too) but it is not stable yet (see [this issue](https://github.com/jeanp413/open-remote-wsl/issues/2#issuecomment-3216285319)).

### Graphics Editor
- [PixiEditor](https://pixieditor.net) - 🆓 Supports pixel art, vector and raster editing, heightmaps, sprite sheets, and animations. Developers explicitly state no-AI use. I did not test all features, but this project is quite promising.

### Grammar Checker
- [Harper](https://writewithharper.com) - 🆓 Runs _English_ grammar checking on-device. Might have other languages in the future.
  > No network request, no massive language models, no fuss.

### GIS
- [uMap](https://umap.openstreetmap.fr/en/about/) - 🆓 Create layered maps that can be embbeded on any site. Has high-quality aerial imagery layer for France (provided by [IGN](https://www.ign.fr/)).

### Office Suite
- [LibreOffice](https://www.libreoffice.org) - 🆓 Not much to add, most of you should use it already. I tend to use Writer for formatting and spell checking, then I use LaTeX to render my documents -- I do not use Calc as often.

## AI-Related Settings
1. If you use Pinterest, disable the setting ["Use your data to train Pinterest Canvas"](https://help.pinterest.com/en/article/manage-genai-settings).
2. If you use DuckDuckGo, you can now filter out *most* AI-generated images from results, go to [AI Features](https://duckduckgo.com/settings#aifeatures) and turn on "Hide AI-Generated Images".

## Stopping AI Crawler Bots
To stop most AI chatbots and data crawlers on your website, add this `robots.txt` to your root folder (for up-to-date index of agents, check [AI agent directory](https://usehall.com/agents) and [AI Agents](https://darkvisitors.com/agents)):

<details>
  <summary>robots.txt</summary>


```robots
# default (for search engines)
User-agent: *
Allow: /

# AI bots
User-agent: AI2Bot
User-agent: Ai2Bot-Dolma
User-agent: Amazonbot
User-agent: anthropic-ai
User-agent: Applebot-Extended
User-agent: Bytespider
User-agent: CCBot
User-agent: ChatGPT-User
User-agent: Claude-Web
User-agent: ClaudeBot
User-agent: cohere-ai
User-agent: cohere-training-data-crawler
User-agent: Cotoyogi
User-agent: Datenbank Crawler
User-agent: Diffbot
User-agent: DuckAssistBot
User-agent: FacebookBot
User-agent: Factset_spyderbot
User-agent: FriendlyCrawler
User-agent: Google-Extended
User-agent: GoogleOther
User-agent: GoogleOther-Image
User-agent: GoogleOther-Video
User-agent: GPTBot
User-agent: iaskspider/2.0
User-agent: ICC-Crawler
User-agent: ImagesiftBot
User-agent: img2dataset
User-agent: ISSCyberRiskCrawler
User-agent: Kangaroo Bot
User-agent: Meta-ExternalAgent
User-agent: Meta-ExternalFetcher
User-agent: netEstate Imprint Crawler
User-agent: OAI-SearchBot
User-agent: omgili
User-agent: omgilibot
User-agent: PanguBot
User-agent: PerplexityBot
User-agent: PetalBot
User-agent: Scrapy
User-agent: SemrushBot-OCOB
User-agent: Sidetrade indexer bot
User-agent: Timpibot
User-agent: VelenPublicWebCrawler
User-agent: Webzio-Extended
User-agent: YouBot
Disallow: /
```

</details>

> [!WARNING]
> As of *2025-08-04*, Cloudflare has assessed that [Perplexity is using stealth, undeclared crawlers to evade website no-crawl directives](https://blog.cloudflare.com/perplexity-is-using-stealth-undeclared-crawlers-to-evade-website-no-crawl-directives/).

## Impacts of AI

1. [How crawlers impact the operations of the Wikimedia projects](https://diff.wikimedia.org/2025/04/01/how-crawlers-impact-the-operations-of-the-wikimedia-projects/)
    > But with the rise of AI, the dynamic is changing: We are observing a significant increase in request volume, with most of this traffic being driven by scraping bots collecting training data for large language models (LLMs) and other use cases. \[...\] 65% of our most expensive traffic comes from bots.
2. [In the AI era, Wikipedia has never been more valuable](https://wikimediafoundation.org/news/2025/11/10/in-the-ai-era-wikipedia-has-never-been-more-valuable/)
    > That’s also why we are calling on AI developers and other content reusers who access our content to use it responsibly and sustain Wikipedia. They can accomplish this through two straightforward actions: attribution and financial support.
4. [At Amazon, Some Coders Say Their Jobs Have Begun to Resemble Warehouse Work](https://www.nytimes.com/2025/05/25/business/amazon-ai-coders.html)
    > The engineers said that the company had raised output goals and had become less forgiving about deadlines... One Amazon engineer said his team was roughly half the size it had been last year, but it was expected to produce roughly the same amount of code by using A.I.

## AI-Free Content Badge
A visual badge for authors to show their users, clearly and quickly, that a work does not use "AI" features. By using the badge, the writer, designer, or developer is showing to their users that they:
1. have not used "AI" tools to create the work;
2. have not implemented any "AI" features within the work; and,
3. do not use their users' data to train "AI" models.

This can be used in any digital or physical work, as long as the author commits to the three items above. Additionally, it is recommended that the author signs the commitment in the next section.

![badge](./badge.png)

## Commitment
If you are an author, show below your commitment to not use nor implement "AI-features" such as LLM chatbots and generative tools.

[@oAGoulart](https://github.com/oAGoulart)

## Do NOT Trust
- Otter.ai
  - McCurdy, W. (2025, August 16). Otter Accused of Recording Meetings Without Consent to Train Its Tech. PCMag. https://www.pcmag.com/news/using-otter-notetaker-this-lawsuit-says-it-broke-privacy-laws.
- Bitwarden
  - Babcock, K. (2025, July 10). Bitwarden sets foundation for secure AI authentication with MCP server. Bitwarden Blog. https://bitwarden.com/blog/bitwarden-mcp-server/. \[[Archived](https://web.archive.org/web/20250712202221/https://bitwarden.com/blog/bitwarden-mcp-server/)\]
- Microsoft
  - Zeff, M. (2025, April 29). Microsoft CEO says up to 30% of the company’s code was written by AI. TechCrunch. https://techcrunch.com/2025/04/29/microsoft-ceo-says-up-to-30-of-the-companys-code-was-written-by-ai/. \[[Archived](https://web.archive.org/web/20250502041532/https://techcrunch.com/2025/04/29/microsoft-ceo-says-up-to-30-of-the-companys-code-was-written-by-ai/)\]
  - Warren, T. (2025, May 15). Microsoft shuts off Bing Search APIs and recommends switching to AI. The Verge. https://www.theverge.com/news/667517/microsoft-bing-search-api-end-of-support-ai-replacement. \[[Archived](https://web.archive.org/web/20250519085046/https://www.theverge.com/news/667517/microsoft-bing-search-api-end-of-support-ai-replacement)\]
- Google
  - Duboust, O. (2025, May 15). YouTube will start playing ads at ‘peak’ video moments using new artificial intelligence tool. Euronews. https://www.euronews.com/next/2025/05/15/youtube-will-start-playing-ads-at-peak-video-moments-using-new-artificial-intelligence-too. \[[Archived](https://web.archive.org/web/20250516135704/https://www.euronews.com/next/2025/05/15/youtube-will-start-playing-ads-at-peak-video-moments-using-new-artificial-intelligence-too)\]
- Adobe
  - Harding, S. (2025, May 20). Adobe to automatically move subscribers to pricier, AI-focused tier in June. Ars Technica. https://arstechnica.com/gadgets/2025/05/adobe-hikes-subscription-prices-to-support-generative-ai-features/. \[[Archived](https://web.archive.org/web/20250520214614/https://arstechnica.com/gadgets/2025/05/adobe-hikes-subscription-prices-to-support-generative-ai-features/)\]
- Duolingo
  - Peters, J. (2025, April 28). Duolingo will replace contract workers with AI. The Verge. https://www.theverge.com/news/657594/duolingo-ai-first-replace-contract-workers. \[[Archived](https://web.archive.org/web/20250518114620/https://www.theverge.com/news/657594/duolingo-ai-first-replace-contract-workers)\]
- Netflix
  - Harding, S. (2025a, May 15). Netflix will show generative AI ads midway through streams in 2026. Ars Technica. https://arstechnica.com/gadgets/2025/05/netflix-will-show-generative-ai-ads-midway-through-streams-in-2026/. \[[Archived](https://web.archive.org/web/20250519011340/https://arstechnica.com/gadgets/2025/05/netflix-will-show-generative-ai-ads-midway-through-streams-in-2026/)\]
- Spotify
  - Weatherbed, J. (2025, February 20). Spotify is making it easier to release audiobooks narrated by AI. The Verge. https://www.theverge.com/news/616355/spotify-audiobooks-elevenlabs-ai-narration. \[[Archived](https://web.archive.org/web/20250221104318/https://www.theverge.com/news/616355/spotify-audiobooks-elevenlabs-ai-narration)\]
- __Any__ brand using Brandshield
  - Khan, A. (2024, December 9). itch.io taken down by Funko’s Brandshield AI-powered IP protection software. Shacknews. https://www.shacknews.com/article/142460/itchio-taken-down-funko-ai-ip-protection. \[[Archived](https://web.archive.org/web/20250326021754/https://www.shacknews.com/article/142460/itchio-taken-down-funko-ai-ip-protection)\]
