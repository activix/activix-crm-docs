# Introduction

This documentation will help you understand how third-party services can interact with Activix CRM and vice-versa.

This documentation is constantly updated to reflect the latest changes and features in Activix CRM. Breaking changes will only be introduced in new versions of the API.

When a new version is introduced, a new section of the documentation will be added with a release date, an upgrade guide from the previous version as well as any changes between it and the previous version

API users will be notified of the new version and of the deprecation date of the previous version\(s\). It is our intent to provide support for previous versions for at least 6 months.   
  
Users that have access to a version will automatically gain access to the most recent one but will not have access to previous one \(unless specifically granted for special circumstances\). This means that if a user was added when v3 is the main version, the user will have access to v4, v5 etc, but will never have access to v2.

## API

The Activix CRM API is based on the [REST](https://en.wikipedia.org/wiki/Representational_state_transfer) standard. We try to follow the common standards for API communication as much as possible.

To get started quickly, we suggest reading the Resources documentation here:

{% page-ref page="api-1/resources/" %}

## Objects

Every piece of data in the CRM is represented as an object \(also called `entity`\).  
The `OBJECTS` section explains what each object in the CRM consists of.

### Blank fields

Blank fields will always be included with the value `null` \(they are never omitted\).

### Dates

Unless otherwise specified, all timestamps are in [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) format.

```text
YYYY-MM-DDTHH:MM:SSZ
```

We use the UTC timezone for all timestamps.

## Webhooks

The Activix CRM has the ability to send data to third-party services in a variety of ways. The `WEBHOOKS` section explains how data can pushed to a web service in real time.

{% page-ref page="webhooks-1/webhooks/" %}



