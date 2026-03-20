---
title: Claude Code
subtitle: Setup instructions for Claude Code using AWS Bedrock
---

## Slide 1: Claude Code

  * **Title**: Claude Code
  * **Content**: (No content)

## Slide 2: Access keys: SSO start URL & SSO region

  * **Title**: Access keys: SSO start URL & SSO region
  * **Content**: (No content)

## Slide 3: aws configure sso

  * **Title**: aws configure sso
  * **Content**:
      * SSO session name (Recommended): `abeacock-sso`
      * SSO start URL: `https://ssoins-753561e08f8b016a.portal.eu-west-2.app.aws/#`
      * SSO region: `eu-west-2`
      * SSO registration scopes: `[sso:account:access]`
      * Processing…

## Slide 4: aws configure sso (continued)

  * **Title**: aws configure sso (continued)
  * **Content**:
      * Choose the Test environment account
      * Default client Region: `eu-west-2`
      * CLI default output format (json if not specified): (None specified)
      * Profile name: `abeacock-sso`

## Slide 5: aws sso login --profile=abeacock-sso

  * **Title**: aws sso login --profile=abeacock-sso
  * **Content**: (No content)

## Slide 6: Install Claude Code

  * **Title**: Install Claude Code
  * **Content**: <https://code.claude.com/docs/en/quickstart>

## Slide 7: Install Git for Windows

  * **Title**: Install Git for Windows
  * **Content**: <https://git-scm.com/install/windows>

## Slide 8

  * **Title**: (No title)
  * **Content**:
      * Windows PowerShell: `irm https://claude.ai/install.ps1 | iex`
      * Open a terminal window: `> claude`

## Slide 9: .claude/settings.json

  * **Title**: .claude/settings.json
  * **Content**:

<!-- end list -->

``` json
{
  "awsAuthRefresh": "aws sso login --profile abeacock-sso",
  "env": {
   "CLAUDE_CODE_USE_BEDROCK": "1",
   "AWS_PROFILE": "abeacock-sso",
   "AWS_REGION": "eu-west-2",
   "ANTHROPIC_DEFAULT_OPUS_MODEL": "eu.anthropic.claude-opus-4-6-v1",
   "ANTHROPIC_DEFAULT_SONNET_MODEL": "eu.anthropic.claude-sonnet-4-6",
   "ANTHROPIC_DEFAULT_HAIKU_MODEL": "eu.anthropic.claude-haiku-4-5-20251001-v1:0"
  },
  "model": "sonnet"
}

```

## Slide 10: VS Code Claude extension

  * **Title**: VS Code Claude extension
  * **Content**: (No content)

## Slide 11: VS Code - Claude Settings

  * **Title**: VS Code - Claude Settings
  * **Content**: (No content)

## Slide 12: VS Code - Disable login prompt

  * **Title**: VS Code - Disable login prompt
  * **Content**: (No content)
