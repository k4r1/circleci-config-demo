# README

This repo is created to demonstrate an issue with CircleCI validation to their support team.

When attempting to use [certain Pipeline Values](https://circleci.com/docs/2.0/pipeline-variables/#pipeline-values), CircleCI remotely is happy with the config, but the command `circleci config validate` reports that the config is invalid.

Jobs:

- `build-<< pipeline.number >>`
- `check`

The `check` job failing whilst `build-<< pipeline.number >>` passes demonstrates this issue.
