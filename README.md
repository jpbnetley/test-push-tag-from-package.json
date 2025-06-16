# test-push-tag-from-package.json

A minimal project demonstrating how to automatically create and push a git tag based on the version in `package.json` using GitHub Actions.

## Project Structure

- `package.json` – Project metadata and scripts.
- `.github/workflows/release.yml` – GitHub Actions workflow for tagging releases.

## Release Workflow

This project uses a GitHub Actions workflow to:

1. Extract the version from `package.json`.
2. Check if a git tag for that version already exists.
3. If not, create and push a new tag.

The workflow runs on pushes to the `main` branch or via manual dispatch.

## Usage

1. Update the `version` field in `package.json` as needed.
2. Push changes to the `main` branch.
3. The workflow will automatically create and push a tag if one does not already exist for that version.

## Example of composite action being consumed
- https://github.com/jpbnetley/push-tag-from-package.json-action
