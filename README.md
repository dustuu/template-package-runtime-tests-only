* [template-package-runtime-tests-only](https://github.com/dustuu/template-package-runtime-tests-only) shows the same scenario as [template-package-runtime-tests-only-fail](https://github.com/dustuu/template-package-runtime-tests-only-fail), but this time has `REQUIRED_COVERAGE` set to `0`.
  * The `Build Release` workflow will pass on all three jobs. even without Editor Tests. This is because the new configuration no longer requires full code coverage:
  * ![image](https://github.com/vrchat-community/template-package/assets/101824882/9d54b24d-08e2-49a0-b4a7-e86b7bce55b2)
  * The `Build Repo Listing` workflow will be trigged to run and will succeed.
  * Both badges will be configured properly:
    * [![VPM Package Version](https://img.shields.io/vpm/v/com.vrchat.demo-template?repository_url=https%3A%2F%2Fdustuu.github.io%2Ftemplate-package-runtime-tests-only%2Findex.json)](https://dustuu.github.io/template-package-runtime-tests-only)
    * [![Code Coverage](https://dustuu.github.io/template-package-runtime-tests-only/coverage/badge_linecoverage.svg)](https://dustuu.github.io/template-package-runtime-tests-only/coverage)
