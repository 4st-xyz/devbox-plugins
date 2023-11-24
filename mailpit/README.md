# Mailpit

Plugin for the [`mailpit`](https://www.nixhub.io/packages/mailpit) package. This plugin sets the `MAILPIT_ARGS` environment variable to run an instance of Mailpit in your local project.

## How to Activate

To install Mailpit, run `devbox add mailpit@latest`

To activate this plugin, add the following reference to the `include` section of your `devbox.json` file.

```json

"include": [
    "github:4st-xyz/devbox-plugins?dir=mailpit"
],
```

## Services

* rabbitmq

Use `devbox services up mailpit` to start Mailpit

## Files

This plugin creates the following helper files:

* **.devbox/virtenv/mailpit/process-compose.yaml** - Defines the process to start Mailpit

## Environment Variables

This plugin sets the following environment variables:

* **MAILPIT_ARGS** = // see https://mailpit.axllent.org/docs/configuration/runtime-options/
