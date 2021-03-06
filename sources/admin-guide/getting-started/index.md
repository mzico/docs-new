# Getting Started

This document will show you how to get up and running with the Gluu Server. It is broken down into the following sections:

1. [What is the Gluu Server](#what-is-the-gluu-server)  
2. [Deployment](#deployment)  
3. [Dashboard](#dashboard)
4. [Authentication](#authentication)   
    a. [Customer Authentication](#customer-authentication)  
    b. [Multi-Factor Authentication](#multi-factor-authentication)  
5. [Identity Management](#identity-management)   
6. [Single Sign-On (SSO)](#single-sign-on-sso)  
7. [Web & API Access Management](#web--api-access-management)  

## What is the Gluu Server

The Gluu Server is an identity and access management suite comprised of free open source software (FOSS) components. Some of the software was written by Gluu (all OX products), and some of the software we forked from existing open source projects (Shibboleth, OpenDJ, Asimba, and CAS). Learn more about each of the open source licenses [here](../introduction/index.md#licenses).

The full suite of software is distributed as easy to install linux packages that support either single server or clustered deployments. In order to gain access to the clustered packages, a commercial license needs to be purchased. More about that below in [Deployment Models](#deployment-models).


## Deployment
The Gluu Server is very flexible, and can be deployed on any physical or virtual server. Depending on the size of your data, and the number of concurrent authentications you want to be able to support, you may need more or less memory or CPU capacity.        

##### Server Requirements:    
We recommend at least 2 CPU units, 4 GB of RAM, and around 30GB of disk space. From there, you may need to adjust the resources based on the requirements.
 
##### OS Support:     
We currently support and maintain package repositories for Ubuntu, CentOS, and Red Hat.   

##### Deployment Models:  
*Single Server:* You can find deployment instructions for a single instance of the Gluu Server by following one of the links above to your preferred operating system. All single server deployments of the Gluu Server can be deployed in production with an unlimited number of users for free.   

*Clusters:*  To deploy a cluster of Gluu Servers, your best option is to purchase one or more of our commercial cluster licenses. You can purchase a single license which supports a two server cluster via our ecommerce system for $1,995 per license. To deploy a more robust environment, you may want to purchase an enterprise license, which will enable you to cluster your Gluu Servers across as many servers and in as many environements (i.e. QA, Production, Development, Staging, etc.) as desired. 

## Dashboard
The dashboard shows you metrics on the health and activity of your Gluu Server. 

## Authentication
The Gluu Server provides an interface to centrally configure authentication logic for your organization. 

### Customer Authentication
### Multi-Factor Authentication

## Identity Management
To keep the Gluu Server up-to-date with the latest user claims, your organization can either "push" or "pull" identity data. In the "pull" mode, otherwise known as LDAP Syncronization or Cache Refresh, the Gluu Server can use an existing LDAP identity source like Microsoft Active Directory as the authoritative source of identity information. If you "push" identities to the Gluu Server, you can use the JSON/REST SCIM API. Local user management can also be performed inside oxTrust.


## Single Sign-On (SSO)
The Gluu Server stack includes both a SAML and OpenID Connect Identity Provider which can be configured for single sign-on to any SAML 2.0 or OpenID Connect protected application.


## Web & API Access Management
The Gluu Server includes an UMA Authorization Server (AS) that can be used to enforce policies for access to any API or web resource. UMA is a profile of OAuth2 that is complimentary to OpenID Connect. UMA defines RESTful, JSON-based, standardized flows and constructs for access management. 
