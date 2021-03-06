## GitHub Enterprise Server (GHES) installation notes

✅ | This course is fully compatible with any versions 2.17 and above of GHES.
--- | ---

This course makes use of [security alerts for vulnerable dependencies](https://help.github.com/en/articles/about-security-alerts-for-vulnerable-dependencies), a feature that needs to be configured by GHES administrators.

### Course dependencies

The following are dependencies of the course. The course may continue to work without these dependencies, but learners won't experience the course as designed.

| Dependency                                                                                                                      | Required? | Reason                                                                                                                                           | Alternative                                                                                                                                                                                    |
|---------------------------------------------------------------------------------------------------------------------------------|-----------|--------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| GHES must be able to reach githubusercontent.com                                                                                | Yes       | Images used throughout the course are served from this domain. Learners will find broken images required to take the course without this access. | Manually download the images referenced in the `responses/` folder, upload them to an accessible domain, and replace the images in the `responses/` folder.                                    |
| Security alerts for vulnerable dependencies must be enabled on GHES | Yes | This course prompts users to interact with alerts triggered by intentionally vulnerable dependencies. | None |
| Learner must be able to reach github.com and outside web                                                                        | No        | Links are provided to resources that live on the outside web.                                                                                    | Without access to resources on the outside web, learners will reach blocked resources. You can change the links to these resources in the `responses/` folder, and in the template repository. |
| [GitHub Pages](https://help.github.com/en/enterprise/admin/installation/configuring-github-pages-on-your-appliance)             | No        | Used to let the learner work on a realistic, published web page.                                                                                 | Remove the first step in `config.yml`, and adjust responses in the `responses/` folder to remove any mentions of GitHub Pages. |