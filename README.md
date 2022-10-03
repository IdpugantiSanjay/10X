# 10X

### Code Practices Checklist

#### Local Development
    - [ ] Conventional Commits
    - [ ] Commit Linting
    - [ ] Pre Commit hooks
        - [ ] Run formatting / linting
        - [ ] Run Unit Tests
    - [ ] Pre Push hooks
        - [ ] Check for exposed secrets using git guardian
        - [ ] Run Integration Tests
        - [ ] Run E2E tests
    - [ ] Use Dockerfile and docker-compose
    - [ ] WatchTower to monitor new docker images

    ##### CI - Pull Request
    - [ ] Use Github Super Linter
    - [ ] Run Unit and Integration Tests
    - [ ] Run Code Quality Analysis
    - [ ] Get coverage report
    - [ ] Send notification when all PR checks passed
    - [ ] Run Sonar Qube

    ##### CI - Master
    - [ ] Github Actions for building Docker Image and Pushing to Docker hub

    ##### CI - Git Tag
    - [ ] Github Actions for building Docker Image using the specified git tag
    - [ ] Use Github Release / Packages for every git tag push

#### Continous Deployment
- [ ] Use Github Actions to deploy to AWS/Azure
- [ ] Use Terraform for provisioning cloud infrastructure
- [ ] Use Ansible for provisioning VM softwares


#### Observability Best Practices
- [ ] Use an APM library (ElasticSearch / Cloudwatch / Application Insights) to log every request's duration
- [ ] Log Request Body if the Response Code is >500
- [ ] Use WatchDog library for simple request response loggin (maybe even only for Local Dev)
- [ ] Use Alarms for alerting on 500 error
- [ ] Use a library to Track core web vitals
