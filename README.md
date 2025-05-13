# Django ToDo list

This is a to-do list web application with basic features of most web apps, i.e., accounts/login, API, and interactive UI. 
To complete this task, you will need:

- CSS | [Skeleton](http://getskeleton.com/)
- JS  | [jQuery](https://jquery.com/)

## Summary

In this project, I extended the GitHub Actions workflow by integrating Docker and Kubernetes deployment to a local kind cluster using Helm:

- Added DockerHub credentials (username and password) to the repository secrets.

- Updated the DockerImageName variable with my DockerHub repository.

- Created a reusable workflow to deploy to a kind Kubernetes cluster:

    - The workflow supports deploying to multiple environments via inputs.

    - Spins up a local cluster using cluster.yml.

    - Includes helm install --dry-run for validation.

    - Uses helm upgrade --install --atomic to ensure safe deployments.

    - All sensitive data is stored in environment secrets.

Also, utilized the reusable workflow to deploy to both development and staging environments.
