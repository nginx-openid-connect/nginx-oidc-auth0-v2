# nginx-oidc-auth0

Reference implementation of NGINX Plus as relying party for OpenID Connect authentication w/ Auth0.

This repo provides the information of how to set up Auth0, integrate with NGINX Plus, and test using a containerized NGINX Plus app, a frontend OIDC simulation tool, and a NGINX Dev Portal.

![](./docs/img/nginx-oidc-workflow.png)

- [Getting Started](#🏠-getting-started)
- [Troubleshooting](#🔧-troubleshooting)
- [References](#📚-references)

<br>

## 🏠 Getting Started

### Set up an identity provider (IdP)

- [Create and configure an app in Auth0](./docs/01-Auth0-Setup.md)

### Option 1. Directly set up a SSO application via NGINX Plus

- [Configure NGINX Plus OIDC](./docs/02-NGINX-Plus-Setup.md)
- [Test an SSO app in a container ](./docs/03-Container-Test.md)

### Option 2. Set up a SSO application via NGINX ACM

- [Configure and test NGINX Dev Portal OIDC](./docs/04-NGINX-DevPortal-Test.md)

<br>

## 🔧 Troubleshooting

- How to ensure that Auth0 correctly set up before configuring your app or NGINX Dev Portal?

  > Take the step of [Option 1. Set up your application via NGINX Plus](#option-1-set-up-your-application-via-nginx-plus) once you set up Auth0.

- How to troubleshoot when PKCE is not working with Auth0?
- How to troubleshoot when none-PKCE is not working with Auth0?
- How to troubleshoot when logout is not working with Auth0?
- How to troubleshoot when dns server is not responding?
- How to troubleshoot when a frontend OIDC simulation tool is not working with `X-Client-Id should be in cookie`. when signing-in after signed-out?
- [Additional troubleshooting information](https://github.com/nginxinc/nginx-openid-connect#troubleshooting)

<br>

## 📚 References

- [NGINX OIDC Core v1.0: Forked from NGINX GitHub](https://github.com/nginx-openid-connect/nginx-oidc-core-v1)
- [NGINX Plus: Single Sign-On With Auth0](https://docs.nginx.com/nginx/deployment-guides/single-sign-on/auth0/)
- [NGINX Management Suite](https://docs.nginx.com/nginx-management-suite/)
- [NGINX API Connectivity Manager](https://docs.nginx.com/nginx-management-suite/acm/)
