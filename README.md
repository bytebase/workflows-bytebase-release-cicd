# About
This repository contains example workflows demonstrating a GitOps database CI/CD workflow via GitHub Actions and Bytebase.

When a new pull request is opened, the [check-release](./.github/workflows/bytebase-check-release.yml) workflow checks the new migration files against the target databases.

On push to the main branch, the [release](./.github/workflows/bytebase-release-cicd.yml) workflow creates a release on Bytebase and rollout the changes to your target databases.
