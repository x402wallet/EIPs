<!-- 🌸 x402Wallet Cute README Header 🌸 -->
<p align="center">
  <img src="https://i.postimg.cc/GhnqtKSK/x402wallet-cover.png" alt="x402Wallet Cover" width="800"/>
</p>

<h2 align="center">✨ Welcome to <b>x402Wallet</b> ✨</h2>

<p align="center">
  <em>🌷 Your AI Agent's Cutest Crypto Wallet 🌷</em><br/>
  <em>Instant, Invisible, and a little bit adorable 💫</em>
</p>

<p align="center">
  <a href="https://x.com/x402wallet" target="_blank">
    <img src="https://img.shields.io/badge/🐤%20Follow%20on%20X-1DA1F2?style=for-the-badge&logo=x&logoColor=white" alt="Follow on X">
  </a>
  &nbsp;
  <a href="https://x402wallet.org" target="_blank">
    <img src="https://img.shields.io/badge/🌸%20Visit%20Website-FFD1DC?style=for-the-badge&logoColor=white" alt="Visit Website">
  </a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/🪄_Powered_by_x402Chain_-F9A8D4?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/💙_Built_for_AI_Agents_-A5F3FC?style=for-the-badge"/>
</p>

---

### 🐰 About
x402Wallet is a next-generation wallet for AI agents 🤖  
Seamless, secure, and delightfully simple 💫  
Built on the x402 protocol for instant, trustless micro-payments.

---

### 🌈 Features
- 💰 **AI-native payments** — built for agents, not humans  
- 🔐 **Non-custodial** — your key, your world  
- 🌐 **Cross-chain support** — Solana & beyond  
- ✨ **Beautiful interface** — sleek, cute, and future-ready  

---

### 💌 Connect
<p align="center">
  🐤 <a href="https://x.com/x402wallet" target="_blank">x.com/x402wallet</a><br/>
  🌸 <a href="https://x402wallet.org" target="_blank">x402wallet.org</a>
</p>

---

<p align="center">
  <sub>Made with 💖 by the <b>x402</b> team · 2025</sub>
</p>

# Ethereum Improvement Proposals (EIPs)

> **_ATTENTION_**: The EIPs repository has recently [undergone](https://github.com/ethereum/EIPs/pull/7206) a separation of ERCs and EIPs. ERCs are now accessible at [https://github.com/ethereum/ercs](https://github.com/ethereum/ercs). All new ERCs and updates to existing ones must be directed at this new repository. The editors apologize for this inconvenience.

The goal of the EIP project is to standardize and provide high-quality documentation for Ethereum itself and conventions built upon it. This repository tracks past and ongoing improvements to Ethereum in the form of Ethereum Improvement Proposals (EIPs). [EIP-1](https://eips.ethereum.org/EIPS/eip-1) governs how EIPs are published.

The [status page](https://eips.ethereum.org/) tracks and lists EIPs, which can be divided into the following categories:

- [Core EIPs](https://eips.ethereum.org/core) are improvements to the Ethereum consensus protocol.
- [Networking EIPs](https://eips.ethereum.org/networking) specify the peer-to-peer networking layer of Ethereum.
- [Interface EIPs](https://eips.ethereum.org/interface) standardize interfaces to Ethereum, which determine how users and applications interact with the blockchain.
- [ERCs](https://eips.ethereum.org/erc) specify application layer standards, which determine how applications running on Ethereum can interact with each other.
- [Meta EIPs](https://eips.ethereum.org/meta) are miscellaneous improvements that nonetheless require some sort of consensus.
- [Informational EIPs](https://eips.ethereum.org/informational) are non-standard improvements that do not require any form of consensus.

**Before you write an EIP, ideas MUST be thoroughly discussed on [Ethereum Magicians](https://ethereum-magicians.org/) or [Ethereum Research](https://ethresear.ch/t/read-this-before-posting/8). Once consensus is reached, thoroughly read and review [EIP-1](https://eips.ethereum.org/EIPS/eip-1), which describes the EIP process.**

Please note that this repository is for documenting standards and not for help implementing them. These types of inquiries should be directed to the [Ethereum Stack Exchange](https://ethereum.stackexchange.com). For specific questions and concerns regarding EIPs, it's best to comment on the relevant discussion thread of the EIP denoted by the `discussions-to` tag in the EIP's preamble.

If you would like to become an EIP Editor, please read [EIP-5069](./EIPS/eip-5069.md).

## Preferred Citation Format

The canonical URL for an EIP that has achieved draft status at any point is at <https://eips.ethereum.org/>. For example, the canonical URL for EIP-1 is <https://eips.ethereum.org/EIPS/eip-1>.

Consider any document not published at <https://eips.ethereum.org/> as a working paper. Additionally, consider published EIPs with a status of "draft", "review", or "last call" to be incomplete drafts, and note that their specification is likely to be subject to change.

## Validation and Automerging

All pull requests in this repository must pass automated checks before they can be automatically merged:

- [eip-review-bot](https://github.com/ethereum/eip-review-bot/) determines when PRs can be automatically merged [^1]
- EIP-1 rules are enforced using [`eipw`](https://github.com/ethereum/eipw)[^2]
- HTML formatting and broken links are enforced using [HTMLProofer](https://github.com/gjtorikian/html-proofer)[^2]
- Spelling is enforced with [CodeSpell](https://github.com/codespell-project/codespell)[^2]
  - False positives sometimes occur. When this happens, please submit a PR editing [.codespell-whitelist](https://github.com/ethereum/EIPs/blob/master/config/.codespell-whitelist) and **ONLY** .codespell-whitelist
- Markdown best practices are checked using [markdownlint](https://github.com/DavidAnson/markdownlint)[^2]

[^1]: https://github.com/ethereum/EIPs/blob/master/.github/workflows/auto-review-bot.yml
[^2]: https://github.com/ethereum/EIPs/blob/master/.github/workflows/ci.yml

It is possible to run the EIP validator locally:

Make sure to add cargo's `bin` directory to your environment (typically `$HOME/.cargo/bin` in your `PATH` environment variable)

```sh
cargo install eipw
eipw --config ./config/eipw.toml <INPUT FILE / DIRECTORY>
```

## Build the status page locally

### Install prerequisites

1. Open Terminal.

2. Check whether you have Ruby 3.1.4 installed. Later [versions are not supported](https://stackoverflow.com/questions/14351272/undefined-method-exists-for-fileclass-nomethoderror).

   ```sh
   ruby --version
   ```

3. If you don't have Ruby installed, install Ruby 3.1.4.

4. Install Bundler:

   ```sh
   gem install bundler
   ```

5. Install dependencies:

   ```sh
   bundle install
   ```

### Build your local Jekyll site

1. Bundle assets and start the server:

   ```sh
   bundle exec jekyll serve
   ```

2. Preview your local Jekyll site in your web browser at `http://localhost:4000`.

More information on Jekyll and GitHub Pages [here](https://docs.github.com/en/enterprise/2.14/user/articles/setting-up-your-github-pages-site-locally-with-jekyll).
