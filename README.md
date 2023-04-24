> This file was generated by [README.tpl](README.tpl) via [yaml-readme](https://github.com/LinuxSuRen/yaml-readme), please don't edit it directly!

## 实用的流水线模板

这里包含一些比较实用的流水线模板。在 KubeSphere Console 编辑一个新的流水线时，我们可以选择合适的模板来填充流水线脚本。

These are offical Pipeline templates:
Template Type: ClusterStepTemplate

| Name | Description |
|---|---|
| [Archive artifacts](featured/steps/archive-artifacts.yaml) | Archive artifacts of the build records |
| [buildkit](featured/steps/buildkit.yaml) | buildkit |
| [CD](featured/steps/cd.yaml) | Update image information using continuous deployment |
| [Checkout](featured/steps/checkout.yaml) | check out source code, often used for non-git repository, such as svn |
| [Specify Container](featured/steps/container.yaml) | Specify a container to add nested tasks to execute inside the container |
| [Docker build &amp; push](featured/steps/docker-build-push.yaml) | Build and push an image from a Dockerfile |
| [Docker login](featured/steps/docker-login.yaml) | Docker login |
| [Echo](featured/steps/echo.yaml) | Print a message in the build |
| [Exit With Error](featured/steps/error.yaml) | Signals an error, exit the Pipeline and mark it as failed |
| [Git Clone](featured/steps/git-clone.yaml) | Pull code from Git-Repo |
| [Fast linters Runner for Go](featured/steps/golangci.yaml) | Fast linters Runner for Go |
| [Groovy Script](featured/steps/groovy-script.yaml) | Execute groovy script |
| [input](featured/steps/input.yaml) | When the pipeline runs here, this task will be suspended, and you can choose to continue or terminate after the review |
| [JUnit Report](featured/steps/junit.yaml) | Archive JUnit-formatted test results |
| [Setup k3s cluster](featured/steps/k3d.yaml) | Setup k3s cluster |
| [Mail](featured/steps/mail.yaml) | Send message by email |
| [Pipeline trigger](featured/steps/pipeline-trigger.yaml) | Trigger a new build for a given job |
| [Retry](featured/steps/retry.yaml) | Repeatedly run given steps |
| [Shell](featured/steps/shell.yaml) | Execute shell commands or windows batch commands in the build |
| [Check license with skywalking-eyes](featured/steps/skywalking-eyes.yaml) | Check license with skywalking-eyes |
| [Sleep](featured/steps/sleep.yaml) | Pause the process for specific time |
| [Code Scan with Snyk](featured/steps/snyk-scan.yaml) | Code Scan with Snyk |
| [Timeout](featured/steps/timeout.yaml) | Executes the code inside the block with a determined time out limit |
| [WaitForQualityGate](featured/steps/waitfor-qauality-gate.yaml) | Execute code analysis(SonarQube) |
| [WithCredential](featured/steps/with-credential.yaml) | Bind credentials to the environment variables |
| [WithSonarQubeEnv](featured/steps/with-sonarqube-env.yaml) | Load a code block with sonarqube configuration environments(run code-review in it) |

Template Type: ClusterTemplate

| Name | Description |
|---|---|
| [Golang](featured/pipelines/golang.yaml) | Designed for the continuous integration of most Golang projects, including dependency downloading, testing, building, and artifact archiving. |
| [Maven](featured/pipelines/maven.yaml) | Designed for the continuous integration of most Maven projects, including dependency downloading, testing, building, and artifact archiving. |
| [Node.js](featured/pipelines/nodejs.yaml) | Designed for the continuous integration of most Node.js projects, including dependency downloading, testing, building, and artifact archiving. |

Template Type: PodTemplate

| Name | Description |
|---|---|
| [buildkit](featured/jenkins-agents/buildkit.yaml) | buildkit |
| [go 1.17](featured/jenkins-agents/go-1.17.yaml) | This is a PodTemplate for the Jenkins agent with go 1.17 |
| [go 1.18](featured/jenkins-agents/go-1.18.yaml) | This is a PodTemplate for the Jenkins agent with go 1.18 |
| [go 1.19](featured/jenkins-agents/go-1.19.yaml) | This is a PodTemplate for the Jenkins agent with go 1.19 |
| [Golang builder](featured/jenkins-agents/go-builder.yaml) | Golang builder |
| [Fast linters Runner for Go](featured/jenkins-agents/golangci-lint.yaml) | Fast linters Runner for Go |
| [k3d 5.3.0](featured/jenkins-agents/k3d-5.3.yaml) | k3d 5.3.0 |
| [A full-featured license tool](featured/jenkins-agents/skywalking-eyes.yaml) | A full-featured license tool |
| [Snyk Go 1.17](featured/jenkins-agents/snyk-go-1.17.yaml) | Snyk Go 1.17 |


## Contribution

想要了解更多关于流水线模板如何工作，请参考：

- https://github.com/kubesphere/ks-devops/blob/master/docs/pipeline-template.md
- [Contribution guide](CONTRIBUTION.md)
