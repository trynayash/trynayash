# GitHub Permissions

This document outlines the required GitHub permissions and repository settings for the workflows in this profile to function correctly.

## Workflow Permissions

### snake.yml
**Required permissions:**
- `contents: write` - To commit generated snake SVG files

**Current configuration:**
```yaml
permissions:
  contents: write
```

### metrics.yml
**Required permissions:**
- `contents: read` - To read repository information for metrics generation

**Current configuration:**
```yaml
permissions:
  contents: read
```

### readme-validation.yml
**Required permissions:**
- `contents: read` - To read README.md for validation

**Current configuration:**
```yaml
permissions:
  contents: read
```

## Repository Settings

### Actions Settings

Navigate to: Repository → Settings → Actions → General

**Required settings:**
- ✅ **Allow all actions and reusable workflows** - Required for using third-party actions
- ✅ **Workflow permissions** - Set to "Read and write permissions"
- ✅ **Allow GitHub Actions to create and approve pull requests** - Enable if you want automated PRs

### Secrets Settings

Navigate to: Repository → Settings → Secrets and variables → Actions

**Required secrets:**

#### METRICS_TOKEN
- **Name**: `METRICS_TOKEN`
- **Description**: Personal access token for GitHub metrics generation
- **Required scopes**:
  - `public_repo` - Read public repository information
  - `read:org` - Read organization information (if applicable)
- **How to create**:
  1. Go to GitHub Settings → Developer settings → Personal access tokens → Tokens (classic)
  2. Click "Generate new token (classic)"
  3. Select expiration period (recommended: 90 days or no expiration)
  4. Check required scopes
  5. Generate and copy token
  6. Paste in repository secrets

## Branch Protection Rules (Optional but Recommended)

Navigate to: Repository → Settings → Branches

**Recommended rules for main branch:**
- ✅ **Require a pull request before merging**
- ✅ **Require approvals** - 1 approval required
- ✅ **Require status checks to pass before merging**
  - Add: `Validate links`
  - Add: `Lint Markdown`
- ✅ **Require branches to be up to date before merging**
- ✅ **Do not allow bypassing the above settings**

## Workflow-Specific Requirements

### Snake Workflow
- **Write access**: Required to commit `.github/assets/github-snake.svg`
- **Schedule**: Runs daily at 00:00 UTC
- **Manual trigger**: Available via workflow_dispatch

### Metrics Workflow
- **Read access**: Required to fetch repository statistics
- **Secret**: Requires `METRICS_TOKEN` for API access
- **Schedule**: Runs daily at 00:00 UTC
- **Manual trigger**: Available via workflow_dispatch

### Validation Workflow
- **Read access**: Required to validate README.md
- **Triggers**: 
  - Pull requests modifying README.md
  - Pushes modifying README.md
- **No secrets required**

## Security Best Practices

### Token Management
- ✅ Use the minimum required scopes for tokens
- ✅ Set expiration dates on tokens
- ✅ Rotate tokens regularly
- ✅ Never commit tokens to repository
- ✅ Use GitHub Secrets for sensitive data

### Workflow Permissions
- ✅ Use the principle of least privilege
- ✅ Only grant write permissions when necessary
- ✅ Review third-party actions before use
- ✅ Pin actions to specific versions (e.g., `@v4` instead of `@main`)

### Repository Visibility
- This profile repository should be **public** for:
  - GitHub profile display
  - External service access
  - Workflow execution

## Troubleshooting

### Workflow Fails with "Resource not accessible"
**Cause**: Insufficient permissions
**Solution**: 
1. Check workflow permissions in repository settings
2. Ensure "Read and write permissions" is enabled
3. Verify token has required scopes

### Metrics Workflow Fails
**Cause**: Missing or invalid `METRICS_TOKEN`
**Solution**:
1. Verify secret exists in repository settings
2. Check token has not expired
3. Verify token has required scopes
4. Regenerate token if necessary

### Snake Workflow Doesn't Commit
**Cause**: Write permissions not granted
**Solution**:
1. Check workflow has `contents: write` permission
2. Verify repository settings allow workflow write access
3. Check workflow logs for specific error

### Validation Workflow Skips
**Cause**: README.md not modified
**Solution**: This is expected behavior. Workflow only runs when README.md changes.

## Updating Permissions

If you need to modify workflow permissions:

1. Edit the workflow file in `.github/workflows/`
2. Add or modify the `permissions` section
3. Commit and push changes
4. Verify workflow runs successfully

Example:
```yaml
permissions:
  contents: write
  pull-requests: write
```

## Third-Party Action Permissions

The following third-party actions are used:

| Action | Required Permissions | Purpose |
|--------|---------------------|---------|
| actions/checkout@v4 | contents: read | Checkout repository code |
| Platane/snk@v3 | contents: write | Generate snake SVG |
| lowlighter/metrics@latest | contents: read | Generate metrics |
| gaurav-nelson/github-action-markdown-link-check@v1 | contents: read | Validate links |
| avto-dev/markdown-lint@v1 | contents: read | Lint markdown |

All actions are pinned to specific versions for security and stability.

## Support

For permission-related issues:
1. Check GitHub Actions logs for specific error messages
2. Review this documentation
3. Consult GitHub Actions documentation: https://docs.github.com/en/actions
