# Stylus to Firemonkey repository template
Here's how to set up your repository for using the [Stylus to Firemonkey](https://github.com/NinoMaruszewski/stylus-to-firemonkey) Github action. For additional configuration info see the repository.

1. Click on "Use this template" in the top right. **Make sure to select the checkbox to keep all branches.**
2. Add style URLs to [styles.txt](./.github/styles.txt).
3. Change your Firemonkey scripts to point to this repository.

### Reviewing PRs before merging
If you want to review the PR before merging, see the [Create Pull Request Action](https://github.com/marketplace/actions/create-pull-request). A possible config is:
```yaml
- name: Create Pull Request
  uses: peter-evans/create-pull-request@v3
  with:
    commit-message: "Sync styles"
    branch: upstream-sync
    title: Sync Styles
```
