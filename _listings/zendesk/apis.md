---
name: Zendesk
x-slug: zendesk
description: Customer service software and support ticketing system by Zendesk. Cloud-based
  help desk solution used by more than 200,000 organizations worldwide. Free 30-day
  trial.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/283-zendesk.jpg
x-kinRank: "8"
x-alexaRank: "402"
tags: Users
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/zendesk/apis.md
specificationVersion: "0.14"
apis:
- name: Sales Force Desk API Get Users
  x-api-slug: sales-force-desk-api
  description: Get users.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/283-zendesk.jpg
  humanURL: http://www.zendesk.com/
  baseURL: https://yoursite.desk.com//api/v2//users.{format}
  tags: Users,Format
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/zendesk/users-format-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/zendesk/users-format-get-openapi.md
- name: Sales Force Desk API Get User
  x-api-slug: sales-force-desk-api
  description: Get user.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/283-zendesk.jpg
  humanURL: http://www.zendesk.com/
  baseURL: https://yoursite.desk.com//api/v2//users/{id}.{format}
  tags: Users,Format
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/zendesk/usersid-format-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/zendesk/usersid-format-get-openapi.md
- name: Sales Force Desk API
  x-api-slug: sales-force-desk-api
  description: Customer service software and support ticketing system by Zendesk.
    Cloud-based help desk solution used by more than 200,000 organizations worldwide.
    Free 30-day trial.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/283-zendesk.jpg
  humanURL: http://www.zendesk.com/
  baseURL: https://yoursite.desk.com//api/v2
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/zendesk/openapi.md
x-common:
- type: x-base
  url: https://zendesk.com/api/
- type: x-blog
  url: http://www.zendesk.com/blog
- type: x-blog-rss
  url: http://www.zendesk.com/feed
- type: x-crunchbase
  url: http://www.crunchbase.com/company/zendesk
- type: x-crunchbase
  url: https://crunchbase.com/organization/zendesk
- type: x-developer
  url: https://developer.zendesk.com/
- type: x-email
  url: support@zendesk.com
- type: x-email
  url: legal@zendesk.com
- type: x-email
  url: ip@zendesk.com
- type: x-email
  url: privacy@zendesk.com
- type: x-email
  url: press@zendesk.com
- type: x-faq
  url: https://gemini24.zendesk.com/hc/en-us
- type: x-github
  url: https://github.com/zendesk
- type: x-pricing
  url: https://www.zendesk.com/product/pricing/
- type: x-support
  url: https://genexus.zendesk.com/hc/en-us
- type: x-support
  url: https://gemini24.zendesk.com/hc/en-us/requests/new
- type: x-twitter
  url: https://twitter.com/zendesk
- type: x-website
  url: http://www.zendesk.com/
- type: x-website
  url: http://desk.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---