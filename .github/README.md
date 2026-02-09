Skip to main content
GitHub Docs
GitHub Copilot/Concepts/Billing/Copilot requests
Requests in GitHub Copilot
Learn about requests in Copilot, including premium requests, how they work, and how to manage your usage effectively.

In this article
Important

Premium requests for Spark and Copilot coding agent are tracked in dedicated SKUs from November 1, 2025. This provides better cost visibility and budget control for each AI product.
Billing for premium requests began on June 18, 2025, for all paid Copilot plans on GitHub.com, and on August 1, 2025, on GHE.com. The request counters were only set to zero for paid plans.
Premium request counters reset on the 1st of each month at 00:00:00 UTC. See Monitoring your GitHub Copilot usage and entitlements.
Certain requests may experience rate limits to accommodate high demand. Rate limits restrict the number of requests that can be made within a specific time period.
What is a request?
A request is any interaction where you ask Copilot to do something for you—whether it’s generating code, answering a question, or helping you through an extension. Each time you send a prompt in a chat window or trigger a response from Copilot, you’re making a request.

What are premium requests?
Some Copilot features use more advanced processing power and count as premium requests. The number of premium requests a feature consumes can vary depending on the feature and the AI model used.

Premium features
The following Copilot features can use premium requests.

Feature	Premium request consumption	SKU Attribution
Copilot Chat	Copilot Chat uses one premium request per user prompt, multiplied by the model's rate. This includes ask, edit, agent, and plan modes in Copilot Chat in an IDE.	Copilot premium requests
Copilot CLI	Each prompt to Copilot CLI uses one premium request with the default model. For other models, this is multiplied by the model's rate.	Copilot premium requests
Copilot code review	Each time Copilot reviews a pull request (when assigned as a reviewer) or reviews code in your IDE, one premium request is consumed.	Copilot premium requests
Copilot coding agent	Copilot coding agent uses one premium request per session, multiplied by the model's rate. A session begins when you ask Copilot to create a pull request or make one or more changes to an existing pull request. In addition, each real-time steering comment made during an active session uses one premium request per session, multiplied by the model's rate.	Copilot coding agent premium requests
Copilot Spaces	Copilot Spaces uses one premium request per user prompt, multiplied by the model's rate.	Copilot premium requests
Spark	Each prompt to Spark uses a fixed rate of four premium requests.	Spark premium requests
OpenAI Codex Visual Studio Code integration	While in preview, each prompt to OpenAI Codex uses one premium request multiplied by the model multiplier rates.	Copilot premium requests
Third-party coding agents	While in preview, each prompt to a third-party coding agent uses one premium request.	Copilot premium requests
Tip

For instructions on viewing how many premium requests you have used and advice on how to optimize usage, see Monitoring your GitHub Copilot usage and entitlements.

How do request allowances work per plan?
If you use Copilot Free, your plan comes with up to 2,000 inline suggestion requests and up to 50 premium requests per month. All chat interactions count as premium requests.

If you're on a paid plan, you get unlimited inline suggestions and unlimited chat interactions using the included models (GPT-5 mini, GPT-4.1 and GPT-4o). Rate limiting is in place to accommodate for high demand. See Rate limits for GitHub Copilot.

Paid plans also receive a monthly allowance of premium requests, which can be used for advanced chat interactions, inline suggestions using premium models, and other premium features. For an overview of the amount of premium requests included in each plan, see Plans for GitHub Copilot.

Note

If a user has licenses from multiple enterprises, or standalone organizations, they must make a selection using the "Usage billed to" drop down in order to utilize premium requests. The billing entity selected will be billed for any premium requests they make. If no billing entity is selected, premium requests will be blocked. See Monitoring your GitHub Copilot usage and entitlements.

What happens to unused requests at the end of the month?
Unused requests for the previous month do not carry over to the following month.

What if I run out of premium requests?
Note

Additional premium requests are not available to:

Users on Copilot Free. To access more premium requests, upgrade to a paid plan.
Users who subscribe, or have subscribed, to Copilot Pro or Copilot Pro+ through GitHub Mobile on iOS or Android.
If you're on a paid plan and use all of your premium requests, you can still use Copilot with one of the included models for the rest of the month. This is subject to change. Response times for the included models may vary during periods of high usage. Requests to the included models may be subject to rate limiting. See Rate limits for GitHub Copilot.

If you need more premium requests beyond your monthly allowance:

For an individual subscription, set a budget for additional premium requests or upgrade to a higher plan. See Setting up budgets to control spending on metered products.
If you're an enterprise or organization owner, ensure that the "Premium request paid usage" policy is enabled and that extra spending is not prevented by a budget. See Managing the premium request allowance for your organization or enterprise.
Accounts created before August 22, 2025 have a default $0 budget for Copilot premium requests. Premium requests over the allowance are rejected unless you edit or delete this budget.

Important

Beginning December 2, 2025:

Account-level $0 Copilot premium request budgets for GitHub Enterprise and GitHub Team will be removed. See Upcoming removal of Copilot premium request $0 budgets for enterprise and team accounts in the GitHub changelog.

Model multipliers
The available models vary depending on your Copilot plan. See Plans for GitHub Copilot.

Note

The models included with Copilot plans are subject to change.
Discounted multipliers are available for using Copilot auto model selection in Copilot Chat in VS Code. See About Copilot auto model selection.
If you are on a paid Copilot plan and use auto model selection, models qualify for a 10% multiplier discount. For example, Sonnet 4 would be billed at .9x rather than 1x when using auto model selection.
Discounted multipliers are not available for Copilot Free.
Promotional pricing for Claude Opus 4.6 (fast mode) (preview) is available from February 7, 2026 through February 16, 2026. During this period, Claude Opus 4.6 (fast mode) (preview) uses a 9x premium request multiplier.
Each model has a premium request multiplier, based on its complexity and resource usage. If you are on a paid Copilot plan, your premium request allowance is deducted according to this multiplier.

GPT-5 mini, GPT-4.1 and GPT-4o are the included models, and do not consume any premium requests if you are on a paid plan.

If you use Copilot Free, you have access to a limited number of models, and each model will consume one premium request when used.

Model	Multiplier for paid plans	Multiplier for Copilot Free
Claude Haiku 4.5	0.33	1
Claude Opus 4.1	10	Not applicable
Claude Opus 4.5	3	Not applicable
Claude Opus 4.6	3	Not applicable
Claude Opus 4.6 (fast mode) (preview)	9 during promotional period	Not applicable
Claude Sonnet 4	1	Not applicable
Claude Sonnet 4.5	1	Not applicable
Gemini 2.5 Pro	1	Not applicable
Gemini 3 Flash	0.33	Not applicable
Gemini 3 Pro	1	Not applicable
GPT-4.1	0	1
GPT-4o	0	1
GPT-5	1	Not applicable
GPT-5 mini	0	1
GPT-5-Codex	1	Not applicable
GPT-5.1	1	Not applicable
GPT-5.1-Codex	1	Not applicable
GPT-5.1-Codex-Mini	0.33	Not applicable
GPT-5.1-Codex-Max	1	Not applicable
GPT-5.2	1	Not applicable
GPT-5.2-Codex	1	Not applicable
Grok Code Fast 1	0.25	Not applicable
Raptor mini	0	1
Examples of premium request usage
Premium request usage is based on the model’s multiplier and the feature you’re using. For example:

Using Claude Opus 4.5 in Copilot Chat: With a 3× multiplier, one interaction counts as 3 premium requests.
Using GPT-5 mini on Copilot Free: Each interaction counts as 1 premium request.
Using GPT-5 mini on a paid plan: No premium requests are consumed.
Help and support
Did you find what you needed?

Privacy policy
Help us make these docs great!
All GitHub docs are open source. See something that's wrong or unclear? Submit a pull request.

Learn how to contribute

Still need help?
Ask the GitHub community
Contact support
Legal
© 2026 GitHub, Inc.
Terms
Privacy
Status
Pricing
Expert services
Bloghttps://github.com/khanin2529-dot/expert-garbanzo<!-- > [!IMPORTANT] -->
<!-- > Wagmi is participating in Gitcoin Grants round 21. Consider <a href="https://explorer.gitcoin.co/#/round/42161/389/74">supporting the project</a>. Thank you. 🙏 -->

<br>

<p align="center">
  <a href="https://wagmi.sh">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/wevm/wagmi/main/.github/logo-dark.svg">
      <img alt="wagmi logo" src="https://raw.githubusercontent.com/wevm/wagmi/main/.github/logo-light.svg" width="auto" height="60">
    </picture>
  </a>
</p>

<p align="center">
  Reactive primitives for Ethereum apps
<p>

<p align="center">
  <a href="https://www.npmjs.com/package/wagmi">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://img.shields.io/npm/v/wagmi?colorA=21262d&colorB=21262d">
      <img src="https://img.shields.io/npm/v/wagmi?colorA=f6f8fa&colorB=f6f8fa" alt="Version">
    </picture>
  </a>
  <a href="https://scorecard.dev/viewer/?uri=github.com/ossf/scorecard">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://img.shields.io/ossf-scorecard/github.com/wevm/wagmi?label=openssf+scorecard&style=flat&color=21262d&labelColor=21262d">
      <img src="https://img.shields.io/ossf-scorecard/github.com/wevm/wagmi?label=openssf+scorecard&style=flat&color=f6f8fa&labelColor=f6f8fa" alt="OpenSSF Best Practices">
    </picture>
  </a>
  <a href="https://www.bestpractices.dev/en/projects/11233">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://img.shields.io/badge/openssf_best_practices-passing-21262d?labelColor=21262d">
      <img src="https://img.shields.io/badge/openssf_best_practices-passing-f6f8fa?labelColor=f6f8fa" alt="OpenSSF Best Practices">
    </picture>
  </a>
  <br />
  <a href="https://github.com/wevm/wagmi/blob/main/LICENSE">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://img.shields.io/npm/l/wagmi?colorA=21262d&colorB=21262d">
      <img src="https://img.shields.io/npm/l/wagmi?colorA=f6f8fa&colorB=f6f8fa" alt="MIT License">
    </picture>
  </a>
  <a href="https://www.npmjs.com/package/wagmi">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://img.shields.io/npm/dm/@wagmi/core?colorA=21262d&colorB=21262d">
      <img src="https://img.shields.io/npm/dm/@wagmi/core?colorA=f6f8fa&colorB=f6f8fa" alt="Downloads per month">
    </picture>
  </a>
  <a href="https://bestofjs.org/projects/wagmi">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://img.shields.io/endpoint?colorA=21262d&colorB=21262d&url=https://bestofjs-serverless.now.sh/api/project-badge?fullName=wevm%2Fviem%26since=daily">
      <img src="https://img.shields.io/endpoint?colorA=f6f8fa&colorB=f6f8fa&url=https://bestofjs-serverless.now.sh/api/project-badge?fullName=wevm%2Fviem%26since=daily" alt="Best of JS">
    </picture>
  </a>
  <a href="https://app.codecov.io/gh/wevm/wagmi">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://img.shields.io/codecov/c/github/wevm/wagmi?colorA=21262d&colorB=21262d">
      <img src="https://img.shields.io/codecov/c/github/wevm/wagmi?colorA=f6f8fa&colorB=f6f8fa" alt="Code coverage">
    </picture>
  </a>
</p>

---

## Documentation

For documentation and guides, visit [wagmi.sh](https://wagmi.sh).

## Community

For help, discussion about best practices, or any other conversation that would benefit from being searchable:

[Discuss Wagmi on GitHub](https://github.com/wevm/wagmi/discussions)

For casual chit-chat with others using the framework:

[Join the Wagmi Discord](https://discord.gg/SghfWBKexF)

## Contributing

Contributions to Wagmi are greatly appreciated! If you're interested in contributing to Wagmi, please read the [Contributing Guide](https://wagmi.sh/dev/contributing) **before submitting a pull request**.

## Sponsors

If you find Wagmi useful or use it for work, please consider [sponsoring Wagmi](https://github.com/sponsors/wevm?metadata_campaign=gh_readme_support). Thank you 🙏

<p>
  <a href="https://paradigm.xyz">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/wevm/.github/main/content/sponsors/paradigm-dark.svg">
      <img alt="paradigm logo" src="https://raw.githubusercontent.com/wevm/.github/main/content/sponsors/paradigm-light.svg" width="auto" height="70">
    </picture>
  </a>
  <a href="https://tempo.xyz">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/wevm/.github/main/content/sponsors/tempo-dark.svg">
      <img alt="tempo logo" src="https://raw.githubusercontent.com/wevm/.github/main/content/sponsors/tempo-light.svg" width="auto" height="70">
    </picture>
  </a>
</p>

<p>
  <a href="https://twitter.com/family">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/wevm/.github/main/content/sponsors/family-dark.svg">
      <img alt="family logo" src="https://raw.githubusercontent.com/wevm/.github/main/content/sponsors/family-light.svg" width="auto" height="50">
    </picture>
  </a>
  <a href="https://twitter.com/context">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/wevm/.github/main/content/sponsors/context-dark.svg">
      <img alt="context logo" src="https://raw.githubusercontent.com/wevm/.github/main/content/sponsors/context-light.svg" width="auto" height="50">
    </picture>
  </a>
  <a href="https://twitter.com/prtyDAO">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/wevm/.github/main/content/sponsors/partydao-dark.svg">
      <img alt="PartyDAO logo" src="https://raw.githubusercontent.com/wevm/.github/main/content/sponsors/partydao-light.svg" width="auto" height="50">
    </picture>
  </a>
  <a href="https://dynamic.xyz">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/wevm/.github/main/content/sponsors/dynamic-dark.svg">
      <img alt="Dynamic logo" src="https://raw.githubusercontent.com/wevm/.github/main/content/sponsors/dynamic-light.svg" width="auto" height="50">
    </picture>
  </a>
  <a href="https://sushi.com">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/wevm/.github/main/content/sponsors/sushi-dark.svg">
      <img alt="Sushi logo" src="https://raw.githubusercontent.com/wevm/.github/main/content/sponsors/sushi-light.svg" width="auto" height="50">
    </picture>
  </a>
  <a href="https://stripe.com">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/wevm/.github/main/content/sponsors/stripe-dark.svg">
      <img alt="Stripe logo" src="https://raw.githubusercontent.com/wevm/.github/main/content/sponsors/stripe-light.svg" width="auto" height="50">
    </picture>
  </a>
  <a href="https://www.privy.io">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/wevm/.github/main/content/sponsors/privy-dark.svg">
      <img alt="Privy logo" src="https://raw.githubusercontent.com/wevm/.github/main/content/sponsors/privy-light.svg" width="auto" height="50">
    </picture>
  </a>
  <a href="https://pancakeswap.finance/">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/wevm/.github/main/content/sponsors/pancake-dark.svg">
      <img alt="pancake logo" src="https://raw.githubusercontent.com/wevm/.github/main/content/sponsors/pancake-light.svg" width="auto" height="50">
    </picture>
  </a>
  <a href="https://pimlico.io">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/wevm/.github/main/content/sponsors/pimlico-dark.svg">
      <img alt="pimlico logo" src="https://raw.githubusercontent.com/wevm/.github/main/content/sponsors/pimlico-light.svg" width="auto" height="50">
    </picture>
  </a>
  <a href="https://zora.co">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/wevm/.github/main/content/sponsors/zora-dark.svg">
      <img alt="zora logo" src="https://raw.githubusercontent.com/wevm/.github/main/content/sponsors/zora-light.svg" width="auto" height="50">
    </picture>
  </a>
  <a href="https://syndicate.io">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/wevm/.github/main/content/sponsors/syndicate-dark.svg">
      <img alt="syndicate logo" src="https://raw.githubusercontent.com/wevm/.github/main/content/sponsors/syndicate-light.svg" width="auto" height="50">
    </picture>
  </a>
  <a href="https://relay.link">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/wevm/.github/main/content/sponsors/relay-dark.svg">
      <img alt="relay logo" src="https://raw.githubusercontent.com/wevm/.github/main/content/sponsors/relay-light.svg" width="auto" height="50">
    </picture>
  </a>
  <a href="https://polymarket.com">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/wevm/.github/main/content/sponsors/polymarket-dark.svg">
      <img alt="polymarket logo" src="https://raw.githubusercontent.com/wevm/.github/main/content/sponsors/polymarket-light.svg" width="auto" height="50">
    </picture>
  </a>
  <a href="https://routescan.io">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/wevm/.github/main/content/sponsors/routescan-dark.svg">
      <img alt="routescan logo" src="https://raw.githubusercontent.com/wevm/.github/main/content/sponsors/routescan-light.svg" width="auto" height="50">
    </picture>
  </a>
  <a href="https://sequence.xyz">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/wevm/.github/main/content/sponsors/sequence-dark.svg">
      <img alt="sequence logo" src="https://raw.githubusercontent.com/wevm/.github/main/content/sponsors/sequence-light.svg" width="auto" height="50">
    </picture>
  </a>
  <a href="https://gemini.com">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/wevm/.github/main/content/sponsors/gemini-dark.svg">
      <img alt="gemini logo" src="https://raw.githubusercontent.com/wevm/.github/main/content/sponsors/gemini-light.svg" width="auto" height="50">
    </picture>
  </a>
  <a href="https://web3auth.io">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/wevm/.github/main/content/sponsors/web3auth-dark.svg">
      <img alt="web3auth logo" src="https://raw.githubusercontent.com/wevm/.github/main/content/sponsors/web3auth-light.svg" width="auto" height="50">
    </picture>
  </a>
</p>

[Sponsor Wagmi](https://github.com/sponsors/wevm?metadata_campaign=gh_readme_support_bottom)

<br />
<br />

<a href="https://vercel.com/?utm_source=wevm&utm_campaign=oss">
  <img src="https://www.datocms-assets.com/31049/1618983297-powered-by-vercel.svg" alt="Powered by Vercel" height="35">
</a>
<br />
<a href="https://quicknode.com/?utm_source=wevm&utm_campaign=oss">
  <img src="https://raw.githubusercontent.com/wevm/.github/refs/heads/main/content/quicknode-badge.svg" alt="Powered by QuickNode" height="35">
</a>

