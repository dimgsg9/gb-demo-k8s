## This is README for demo Gitlab CI/CD + Helm

At this stage I assume you already have:
* GitLab and Docker hub accounts.
* Setup Kubernetes integration with GitLab repository

Just push this repo into GitLab repo and configure Kubernetes integration in the context of this repository within GitLab.

The following env variables will be expdected by CI/CD pipeline in GitLab project settings:

`REGISTRY_USERNAME` - your docker hub user name
`REGISTRY_PASSWORD` - your docker hub user password

*Don't forget to point any application sample domain name to a public IP of the GCP load balancer created by ingress controller (you can find it in GCP console). I've just added a temporary record into my `hosts` file and pointed test domain like demo-guestbook.net to that public IP.*
