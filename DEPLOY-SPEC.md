# GitHub Pages Deployment Task

## Context
The cafeteria menu for 203 Sports Academy is ready to deploy. Files are already pushed to `CortexTechnologies-AI/203Menu`.

## Your Task

1. **Test the github-pages MCP** by calling:
   ```
   route("enable github pages")
   ```
   Then use the tools found to enable GitHub Pages on the repo.

2. **If MCP doesn't work**, fall back to gh CLI:
   ```bash
   gh api repos/CortexTechnologies-AI/203Menu/pages -X POST -f build_type=workflow -f source='{"branch":"main","path":"/"}'
   ```
   Or if pages already enabled, just get the URL:
   ```bash
   gh api repos/CortexTechnologies-AI/203Menu/pages --jq '.html_url'
   ```

3. **Report the Pages URL** - It should be something like:
   `https://cortextechnologies-ai.github.io/203Menu/`

## Success Criteria
- GitHub Pages is enabled on the repo
- You have the live URL where the menu is accessible
- Report the URL back

## Files Location
- Menu files: `C:\CORTEX\projects\chef-tony\cafeteria-menu\`
- Repo: `CortexTechnologies-AI/203Menu`
