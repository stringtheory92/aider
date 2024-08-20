<!-- Edit README.md, not index.md -->

Build image: run from root: $ docker build -f docker/Dockerfile -t aider-image .

Run container: $ docker run -it --rm aider-image

# Aider is AI pair programming in your terminal

Aider lets you pair program with LLMs,
to edit code in your local git repository.
Start a new project or work with an existing git repo.
Aider works best with GPT-4o & Claude 3.5 Sonnet and can
[connect to almost any LLM](https://aider.chat/docs/llms.html).

<p align="center">
  <img
    src="https://aider.chat/assets/screencast.svg"
    alt="aider screencast"
  >
</p>

<p align="center">
  <a href="https://discord.gg/Tv2uQnR88V">
    <img src="https://img.shields.io/badge/Join-Discord-blue.svg"/>
  </a>
  <a href="https://aider.chat/docs/install.html">
    <img src="https://img.shields.io/badge/Read-Docs-green.svg"/>
  </a>
</p>

## Getting started

<!--[[[cog
# We can't "include" here.
# Because this page is rendered by GitHub as the repo README
cog.out(open("aider/website/_includes/get-started.md").read())
]]]-->

You can get started quickly like this:

```
python -m pip install aider-chat

# Change directory into a git repo
cd /to/your/git/repo

# Work with Claude 3.5 Sonnet on your repo
export ANTHROPIC_API_KEY=your-key-goes-here
aider

# Work with GPT-4o on your repo
export OPENAI_API_KEY=your-key-goes-here
aider
```

<!--[[[end]]]-->

See the
[installation instructions](https://aider.chat/docs/install.html)
and other
[documentation](https://aider.chat/docs/usage.html)
for more details.

## Features

- Run aider with the files you want to edit: `aider <file1> <file2> ...`
- Ask for changes:
  - Add new features or test cases.
  - Describe a bug.
  - Paste in an error message or or GitHub issue URL.
  - Refactor code.
  - Update docs.
- Aider will edit your files to complete your request.
- Aider [automatically git commits](https://aider.chat/docs/git.html) changes with a sensible commit message.
- Aider works with [most popular languages](https://aider.chat/docs/languages.html): python, javascript, typescript, php, html, css, and more...
- Aider works best with GPT-4o & Claude 3.5 Sonnet and can [connect to almost any LLM](https://aider.chat/docs/llms.html).
- Aider can edit multiple files at once for complex requests.
- Aider uses a [map of your entire git repo](https://aider.chat/docs/repomap.html), which helps it work well in larger codebases.
- Edit files in your editor while chatting with aider,
  and it will always use the latest version.
  Pair program with AI.
- [Add images to the chat](https://aider.chat/docs/usage/images-urls.html) (GPT-4o, Claude 3.5 Sonnet, etc).
- [Add URLs to the chat](https://aider.chat/docs/usage/images-urls.html) and aider will read their content.
- [Code with your voice](https://aider.chat/docs/usage/voice.html).

## Top tier performance

[Aider has one of the top scores on SWE Bench](https://aider.chat/2024/06/02/main-swe-bench.html).
SWE Bench is a challenging software engineering benchmark where aider
solved _real_ GitHub issues from popular open source
projects like django, scikitlearn, matplotlib, etc.

## More info

- [Documentation](https://aider.chat/)
- [Installation](https://aider.chat/docs/install.html)
- [Usage](https://aider.chat/docs/usage.html)
- [Tutorial videos](https://aider.chat/docs/usage/tutorials.html)
- [Connecting to LLMs](https://aider.chat/docs/llms.html)
- [Configuration](https://aider.chat/docs/config.html)
- [Troubleshooting](https://aider.chat/docs/troubleshooting.html)
- [LLM Leaderboards](https://aider.chat/docs/leaderboards/)
- [GitHub](https://github.com/paul-gauthier/aider)
- [Discord](https://discord.gg/Tv2uQnR88V)
- [Blog](https://aider.chat/blog/)

## Kind words from users

- _The best free open source AI coding assistant._ -- [IndyDevDan](https://youtu.be/YALpX8oOn78)
- _The best AI coding assistant so far._ -- [Matthew Berman](https://www.youtube.com/watch?v=df8afeb1FY8)
- _Aider ... has easily quadrupled my coding productivity._ -- [SOLAR_FIELDS](https://news.ycombinator.com/item?id=36212100)
- _It's a cool workflow... Aider's ergonomics are perfect for me._ -- [qup](https://news.ycombinator.com/item?id=38185326)
- _It's really like having your senior developer live right in your Git repo - truly amazing!_ -- [rappster](https://github.com/paul-gauthier/aider/issues/124)
- _What an amazing tool. It's incredible._ -- [valyagolev](https://github.com/paul-gauthier/aider/issues/6#issue-1722897858)
- _Aider is such an astounding thing!_ -- [cgrothaus](https://github.com/paul-gauthier/aider/issues/82#issuecomment-1631876700)
- _It was WAY faster than I would be getting off the ground and making the first few working versions._ -- [Daniel Feldman](https://twitter.com/d_feldman/status/1662295077387923456)
- _THANK YOU for Aider! It really feels like a glimpse into the future of coding._ -- [derwiki](https://news.ycombinator.com/item?id=38205643)
- _It's just amazing. It is freeing me to do things I felt were out my comfort zone before._ -- [Dougie](https://discord.com/channels/1131200896827654144/1174002618058678323/1174084556257775656)
- _This project is stellar._ -- [funkytaco](https://github.com/paul-gauthier/aider/issues/112#issuecomment-1637429008)
- _Amazing project, definitely the best AI coding assistant I've used._ -- [joshuavial](https://github.com/paul-gauthier/aider/issues/84)
- _I absolutely love using Aider ... It makes software development feel so much lighter as an experience._ -- [principalideal0](https://discord.com/channels/1131200896827654144/1133421607499595858/1229689636012691468)
- _I have been recovering from multiple shoulder surgeries ... and have used aider extensively. It has allowed me to continue productivity._ -- [codeninja](https://www.reddit.com/r/OpenAI/s/nmNwkHy1zG)
- _I am an aider addict. I'm getting so much more work done, but in less time._ -- [dandandan](https://discord.com/channels/1131200896827654144/1131200896827654149/1135913253483069470)
- _After wasting $100 on tokens trying to find something better, I'm back to Aider. It blows everything else out of the water hands down, there's no competition whatsoever._ -- [SystemSculpt](https://discord.com/channels/1131200896827654144/1131200896827654149/1178736602797846548)
- _Aider is amazing, coupled with Sonnet 3.5 it’s quite mind blowing._ -- [Josh Dingus](https://discord.com/channels/1131200896827654144/1133060684540813372/1262374225298198548)
- _Hands down, this is the best AI coding assistant tool so far._ -- [IndyDevDan](https://www.youtube.com/watch?v=MPYFPvxfGZs)
- _[Aider] changed my daily coding workflows. It's mind-blowing how a single Python application can change your life._ -- [maledorak](https://discord.com/channels/1131200896827654144/1131200896827654149/1258453375620747264)
- _Best agent for actual dev work in existing codebases._ -- [Nick Dobos](https://twitter.com/NickADobos/status/1690408967963652097?s=20)
