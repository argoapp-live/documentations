---
id: overview-domain
title: Overview
sidebar_label: Overview
slug: /domain-and-https/centralized-domain/overview
---

:::tip info

Domains allows user to access their site via one or more non-Spheron domain names. By default, the site is always accessible via arweave gateway based on transaction id.

:::

:::caution info

Domains use our domain resolver to serve deployed links. As it is a beta version and our system is not stable to handle a lot of traffic, we would like to inform you that if you are using it for the production app, please keep in mind that it may break due to unexpected heavy traffic. We are currently working on it to stabilize the system and we will inform everyone about it.

:::

## Domains

A domain name is the URL or web address where visitors find your site.

Custom domains allow you to make your sites accessible at your own, non-Spheron domain names (for example, `www.yourdomain.com`). Spheron supports all top-level domains.

## Multiple Domains

All the domains which selected the latest option when setting it up on the Spheron platform will point to the latest deployed transaction in Arweave. Otherwise, users can point to a single deployment and the domain site won't change with any new deployment.

## Definitions

- Domain name (or domain for short): full name used to access a site. For example, `yoursitename.spheron.app` or `www.yourdomain.com`

- Top-level domain: last part of the domain name. For example, the `.com` part in `www.yourdomain.com`.

- Apex domain (also known as a root, bare, or naked domain): the `youdomain.com` part in `www.yourdomain.com`.

- Subdomain: a domain that is part of a larger domain; the only domain that is not also a subdomain is the apex domain. For example, `www.yourdomain.com` and `app.yourdomain.com` are subdomains of `yourdomain.com`.

- Domain: a non-Spheron domain assigned to a site.

- Primary domain: Spheron term for the main domain assigned to a site.

- Domain alias: Spheron term for additional domains assigned to a site.

## Default Spheron Subdomain

We have added this new feature for providing a default subdomain for every project on our platform. Now every project created in an organization will have an Spheron subdomain attached to it.

The subdomain will be like - `{subdomain}.spheron.app`, where `subdomain` is `{project-name}-{random 8 digits}`

The default subdomain will always be pointed to the latest deployment that happened in that project. It also provides a better naming convention for sharing your project previews with others.

## Automated DNS Resolver

Earlier, when users attached their domain to a project, they had to add some records to their DNS provider. So, when users redeployed the project again, they had to again change these records which will point to a new deployment which is a great overhead for the users.

Now, Spheron users just have to attach their domains and add the records only once in their DNS provider. Upon successful verification, once the user redeploys any site, their domain will automatically point to the latest deployment or the user can opt for the domain to point a particular deployment.

To use this feature, when adding your domain to a project, you have to select the `latest` option. Choosing this option will link the latest deployed to the domain name and whenever there is any new deployment, it will be linked to the domain name.


## Domain got Environment

Spheron users can attach a deployment environment with a particular domain. Attaching a deployment environment to the domain will give users the flexibility to segregate their domains based on the environment of a project. That means, that if the deployment of a deployment environment is finished, the domain attached to the deployment environment will get updated with the new deployment link.

<img src={require('@site/static/img/3.0.0/dge.png').default} />

:::tip Note

This is only applicable to centralized and subdomains

:::
