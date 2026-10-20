# Demo
This is a short demonstration on how the environment repo holds the complete source of truth what is deployed to each environment.

It bootstraps ArgoCD applications using the bootrap application for each stage.
The bootstrapped ArgoCD applications pulls the correct tagged versions of the [release repository](https://github.com/thake/argocd-playground-release) and provides the matching environment variables.

The release repository itself only contains the versioned charts. There is no reference to the environments.
