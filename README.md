# renovate-config


This is [Shareable Config Presets](https://docs.renovatebot.com/config-presets/) for SpotOn. It contains wide use [Renovatebot](https://github.com/renovatebot/renovate) configs, based on our toolset and mindset.

* [Usage](#usage)
* [Useful links](#useful-links)
  * [Renovate App and presets configuration](#renovate-app-and-presets-configuration)
* [Repos configuration](#repos-configuration)
  * [Troubleshoting](#troubleshoting)


## Usage


<details><summary><u>If Renovate has already been activated for repo</u></summary>

1. Check for `renovate.json` in [possible locations](https://docs.renovatebot.com/getting-started/installing-onboarding/#configuration-location).
2. Change `renovate` config to:

    ```json5
    {
      "$schema": "https://docs.renovatebot.com/renovate-schema.json",
      "extends": [
        "local>SpotOnInc/renovate-config"
      ]
    }
    ```

Go to step 3. below.

</details>

Otherwise:

0. If the repo is too much outdated - prefer to update manually as much as you can before merge Renovate init PR.
1. Activate [Renovatebot Github App](https://github.com/marketplace/renovate) for your repo or ask Github org administrators.
2. Renovate will create [init PR](https://docs.renovatebot.com/getting-started/installing-onboarding/#repository-onboarding) for new repo - open it and check that it has:

    ```json5
    {
      "$schema": "https://docs.renovatebot.com/renovate-schema.json",
      "extends": [
        "local>SpotOnInc/renovate-config"
      ]
    }
    ```

3. (Optional) We recommend moving the config to `.github/renovate.json5`.

4. Merge PR and relax.  
   Renovate will create PRs based on provided schedules.  By default - you will see Renovate PRs on Mondays.

## Useful links

### Renovate App and presets configuration

* [Managing config for many repositories](https://docs.renovatebot.com/key-concepts/presets/#managing-config-for-many-repositories)
* [Shareable Config Presets](https://docs.renovatebot.com/config-presets/#shareable-config-presets)
    * [Organization level presets](https://docs.renovatebot.com/config-presets/#organization-level-presets) -  `myorg/renovate-config/default.json` magic name
    * [GitHub-hosted Presets](https://docs.renovatebot.com/config-presets/#github-hosted-presets)
    * [Contributing to presets](https://docs.renovatebot.com/config-presets/#contributing-to-presets)

* [Renovate App on GitHub Secrets Encryption](https://docs.renovatebot.com/getting-started/private-packages/#mend-renovate-hosted-app-encryption)

* [Known limitations](https://docs.renovatebot.com/known-limitations/)  
  Ie: GitHub hosted app Mend checks each active repository roughly every three hours, if no activity has been seen before then (merged PRs, etc).

* [onboardingConfigFileName](https://docs.renovatebot.com/self-hosted-configuration/#onboardingconfigfilename) (self-hosted only).  
  Useful to change onboarding renovate config file location.

## Repos configuration

* [Configuration location](https://docs.renovatebot.com/getting-started/installing-onboarding/#configuration-location)

* [Overriding global configs](https://docs.renovatebot.com/key-concepts/automerge/#overriding-global-automerge)

* [Scheduling syntax](https://docs.renovatebot.com/key-concepts/scheduling/#scheduling-syntax)


### Troubleshoting

* [Troubleshooting docs](https://docs.renovatebot.com/troubleshooting/)
* [Renovate dashboard](https://app.renovatebot.com/dashboard)
