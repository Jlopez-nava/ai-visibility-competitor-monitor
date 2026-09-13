# Security and data-handling notes

This repository contains a disconnected, anonymized workflow template. It must not be used as a place to store production configuration or workflow output.

## Do not commit

- API keys, OAuth tokens, refresh tokens, passwords, private keys, or webhook URLs.
- Profound category, account, organization, or workspace identifiers.
- Google Docs, Slack, model-provider, or Firecrawl integration identifiers.
- Slack channel identifiers or exported message history.
- Employer, customer, client, or user data.
- Unredacted brand strategies, competitor lists, topic taxonomies, performance claims, or generated reports.
- Raw workflow exports from a connected production workspace.

## Safe setup

Configure integrations inside Profound rather than editing secrets into the JSON. Start with one synthetic topic and a private test Slack channel. Review each service's permissions and data-retention policy before introducing real company data.

## Reporting a problem

If sensitive material is discovered, do not open a public issue containing the affected value. Remove access to the exposed credential at its provider, rotate it, and purge the affected Git history before republishing a clean version.

