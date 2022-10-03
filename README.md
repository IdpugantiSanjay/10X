# 10X

## Code Practices Checklist

Local Development
- [ ] Conventional Commits
- [ ] Commit Linting
- [ ] Pre Commit hooks
    - [ ] Run formatting / linting
    - [ ] Run Unit Tests
- [ ] Pre Push hooks
    - [ ] Check for exposed secrets using git guardian
    - [ ] Run Integration Tests
    - [ ] Run E2E tests
- [ ] Docker Packaging
- [ ] WatchTower 

CI - Pull Request
- [ ] Use Github Super Linter
- [ ] Run Unit and Integration Tests
- [ ] Run Code Quality Analysis
- [ ] Get coverage report
- [ ] Send notification when all PR checks passed

CI - Master
- [ ] Github Actions for building Docker Image and Pushing to Docker hub

CI - Git Tag
- [ ] Github Actions for building Docker Image using the specified git tag

