# Black Duck CoPilot Gradle/GitHub CI Example

[![Actions](https://github.com/BlackDuckCoPilot/example-gradle-githubactions/workflows/Java%20CI/badge.svg)](https://github.com/BlackDuckCoPilot/example-gradle-githubactions/actions?workflow=Java+CI) [![Black Duck Security Risk](https://copilot.blackducksoftware.com/github/repos/BlackDuckCoPilot/example-gradle-githubactions/branches/master/badge-risk.svg)](https://copilot.blackducksoftware.com/github/repos/BlackDuckCoPilot/example-gradle-githubactions/branches/master)

Shows a working setup for using the Synopsys CoPilot GitHub App to analyze the risk of project dependencies

## GitHub CI/CD Setup

The `.github/workflows/workflow.yml` file has been modified to upload generated dependency data to Black Duck CoPilot:

```yaml
- name: Upload to CoPilot
      run: bash <(curl -s https://copilot.blackducksoftware.com/ci/githubactions/scripts/upload)
```
