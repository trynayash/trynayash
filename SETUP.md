# Setup Instructions

This repository contains the GitHub profile configuration for trynayash. Follow these instructions to set up the profile after cloning.

## Required GitHub Secrets

### METRICS_TOKEN

The metrics workflow requires a personal access token with the following permissions:

1. Go to GitHub Settings → Developer settings → Personal access tokens → Tokens (classic)
2. Generate a new token (classic)
3. Select the following scopes:
   - `public_repo` (required for reading public repository information)
   - `read:org` (required if you want to show organization information)
4. Copy the token
5. Go to your profile repository → Settings → Secrets and variables → Actions
6. Add a new secret named `METRICS_TOKEN` with the token value

## Workflow Configuration

### Snake Contribution Graph

The snake workflow (`.github/workflows/snake.yml`) runs daily at 00:00 UTC to generate contribution snake animations.

**No configuration required.** The workflow automatically:
- Generates light and dark theme snake SVGs
- Commits them to `.github/assets/`
- Pushes to the repository

### GitHub Metrics

The metrics workflow (`.github/workflows/metrics.yml`) generates comprehensive GitHub statistics and activity visualizations.

**Configuration:**
- Requires `METRICS_TOKEN` secret (see above)
- Runs daily at 00:00 UTC
- Generates metrics including:
  - Calendar heat map
  - Language usage
  - Commit lines
  - Coding habits
  - Notable repositories
  - People (followers/following)
  - Repository traffic

### README Validation

The validation workflow (`.github/workflows/readme-validation.yml`) runs on:
- Pull requests that modify README.md
- Pushes that modify README.md

It validates:
- Markdown link integrity
- Markdown linting

## External Services

This profile uses the following external services:

### Badge Services
- **Shields.io** (`img.shields.io`) - Status and technology badges
  - Status: Active and maintained
  - Documentation: https://shields.io

### Stats Services
- **GitHub Readme Stats (Shion.dev)** (`github-readme-stats.shion.dev`) - Profile statistics
  - Status: Community-maintained alternative
  - Note: Original `github-readme-stats.vercel.app` is paused
  - Documentation: https://github.com/Shion1305/github-readme-stats

- **Streak Stats (DemoLab)** (`streak-stats.demolab.com`) - Contribution streak
  - Status: Official endpoint
  - Note: Old `github-readme-streak-stats.herokuapp.com` is deprecated
  - Documentation: https://github.com/DenverCoder1/github-readme-streak-stats

### Icon Services
- **SkillIcons** (`skillicons.dev`) - Technology icons
  - Status: Active
  - Documentation: https://skillicons.dev

## Customization

### Updating Profile Information

Edit `README.md` to update:
- About section
- Engineering principles
- Tech stack
- Featured projects
- Experience
- Education
- Current focus

### Updating Project Links

Ensure all project repository links point to actual repositories:
- Check repository names match exactly
- Verify repositories are public
- Test repository URLs in browser

### Adding Snake to README

To display the contribution snake in your README, add:

```markdown
![GitHub Snake](.github/assets/github-snake-dark.svg)
```

Place it in the desired section (typically near GitHub Metrics).

## Troubleshooting

### Metrics Workflow Fails

If the metrics workflow fails:
1. Verify `METRICS_TOKEN` secret is set
2. Check token has required scopes
3. Regenerate token if expired

### Snake Workflow Fails

If the snake workflow fails:
1. Check workflow logs for specific error
2. Verify `.github/assets/` directory exists
3. Ensure workflow has write permissions

### Broken Images

If images appear broken:
1. Check external service status
2. Verify URLs are correct
3. Test URLs in browser
4. Check for rate limiting on external services

### Link Validation Fails

If link validation fails:
1. Check `.github/.mlc_config.json` for ignore patterns
2. Verify all links are accessible
3. Update ignore patterns for dynamic content

## Maintenance

### Regular Tasks

- Review and update project links quarterly
- Check external service status annually
- Update tech stack as skills evolve
- Refresh experience section annually

### Updating External Services

If an external service becomes deprecated:
1. Research alternatives
2. Update URLs in README.md
3. Test new URLs
4. Update this documentation

## Support

For issues with:
- **GitHub Actions**: Check Actions tab logs
- **External services**: Check respective service status pages
- **Profile content**: Edit README.md directly

## License

This profile configuration is provided as-is for personal use.
