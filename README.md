
<!-- PROJECT LOGO -->
<div align="center">
  <h1 align="center">Devon: An open-source pair programmer</h1>
</div>
<div align="center">
  <a href="https://github.com/entropy-research/Devon/graphs/contributors"><img src="https://img.shields.io/github/contributors/entropy-research/devon?style=for-the-badge&color=lime" alt="Contributors"></a>
  <a href="https://github.com/entropy-research/Devon/network/members"><img src="https://img.shields.io/github/forks/entropy-research/devon?style=for-the-badge&color=orange" alt="Forks"></a>
  <a href="https://github.com/entropy-research/Devon/stargazers"><img src="https://img.shields.io/github/stars/entropy-research/devon?style=for-the-badge&color=yellow" alt="Stargazers"></a>
  <a href="https://github.com/entropy-research/Devon/issues"><img src="https://img.shields.io/github/issues/entropy-research/devon?style=for-the-badge&color=red" alt="Issues"></a>
  <br/>
  <a href="https://github.com/entropy-research/Devon/blob/main/LICENSE"><img src="https://img.shields.io/github/license/entropy-research/devon?style=for-the-badge&color=blue" alt="Apache 2.0 License"></a>
  <a href="https://discord.gg/p5YpZ5vjd9"><img src="https://img.shields.io/badge/Discord-Join%20Us-purple?logo=discord&logoColor=white&style=for-the-badge" alt="Join our Discord community"></a>
  <br/>
</div>


VIDEO/GIF HERE

# Installation

## Pre-requisites

1. `node.js` and `npm`
2. `pipx`
3. **Anthropic** api key

## Installation commands

To use simply run:

```bash
curl -sSL https://raw.githubusercontent.com/entropy-research/Devon/main/install.sh | bash
```


*Or to install using pipx + npm*

```bash
pipx install devon_agent
npm install -g devon-tui
```

### Thats it! Happy building :)


# Usage
Prior to running, set your Anthropic API key as an environment variable

```bash
export ANTHROPIC_API_KEY=sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
```

Then to *run*, the command is:
```bash
devon
```

It's as easy as that.

Don't worry, the agent will be able to only access files and folders in the directory you started it from. You can also correct it while it's performing actions.

# Features
- Multi file editing
- Code base exploration
- Config writing
- Test writing
- Bug fixing
- Architecture exploration

### Limitations
- Minimal functionality for non-python languages
- Sometimes have to specify the file where you want the change to happen

# Progress


### This project is still super early and we need your help to make it great!

### Current goals
- Multi-model support
- Launch plugin system for tool and agent builders
- Create self hostable electron app
- Set SOTA on swebench-lite

View our current thoughts on next steps [here](https://docs.google.com/document/d/e/2PACX-1vTjLCQcWE_n-uUHFhtBkxTCIJ4FFe5ftY_E4_q69SjXhuEZv_CYpLaQDh3HqrJlAxsgikUx0sTzf9le/pub)

### Star history
<p align="center">
  <a href="https://star-history.com/#entropy-research/Devon&Date">
    <img src="https://api.star-history.com/svg?repos=entropy-research/Devon&type=Date" width="500" alt="Star History Chart">
  </a>
</p>

### Past Milestones

- [x] May 10, 2024, Complete interactive agent v0.1.0
- [x] May 10, 2024, Add steerability features
- [x] May 8, 2024, Beat AutoCodeRover on SWE-Bench Lite
- [x] Mid April, 2024, Add repo level code search tooling
- [x] April 2, 2024, Begin development of v0.1.0 interactive agent
- [x] March 17, 2024 Launch non-interactive agent v0.0.1


## Current development priorities

1. Improve context gathering and code indexing abilities ex:
    - Adding memory modules
    - Improved code indexing
    - 
2. Add alternative models and agents to:
    - a) Reduce end user cost and
    - b) Reduce end user latency
3. Introduce electron app and new UI



# How can I contribute?

Devon and the entropy-research org are community-driven, and we welcome contributions from everyone!
From tackling issues to building features to creating datasets, there are many ways to get involved:

- **Core functionality:** Help us develop the core agents, user experience, tool integrations, plugins, etc.
- **Research:** Help us research agent performance (including benchmarks!), build data pipelines, and finetune models.
- **Feedback and Testing:** Use Devon, report bugs, suggest features, or provide feedback on usability.

For details, please check [CONTRIBUTING.md](./CONTRIBUTING.md).

If you would like to contribute to the project, please fill out our [contribution Form](https://forms.gle/VU7RN7mwNvqEYe3B9)


# Feedback

We would love feedback! Feel free to drop us a note on our [discord](https://discord.gg/p5YpZ5vjd9) in the feedback channel, or create issues!

We collect basic event type (i.e. "tool call") and failure telemetry to solve bugs and improve the user experience, but if you want to reach out, we would love to hear from you!

To disable telemtry, set the environment variable `DEVON_TELEMETRY_DISABLED` to `true` 
```bash
export DEVON_TELEMETRY_DISABLED=true
```

# Community

Join our discord server and say hi!
[discord](https://discord.gg/p5YpZ5vjd9)


# License

Distributed under the Apache 2.0 License. See [`LICENSE`](./LICENSE) for more information.
