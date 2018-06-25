---
name: Google Stackdriver Monitoring
x-slug: google-stackdriver-monitoring
description: Google Stackdriver provides powerful monitoring, logging, and diagnostics.
  It equips you with insight into the health, performance, and availability of cloud-powered
  applications, enabling you to find and fix issues faster. It is natively integrated
  with Google Cloud Platform, Amazon Web Services, and popular open source packages.
  Stackdriver provides a wide variety of metrics, dashboards, alerting, log management,
  reporting, and tracing capabilities.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-stackdriver.png
x-kinRank: "8"
x-alexaRank: "0"
tags: Monitoring
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/monitoring/master/_listings/google-stackdriver-monitoring/apis.md
specificationVersion: "0.14"
apis:
- name: Google Stackdriver Monitoring Get Project Metric Descriptors
  x-api-slug: google-stackdriver-monitoring
  description: List metric descriptors that match the query. If the query is not set,
    then all of the metric descriptors will be returned. Large responses will be paginated,
    use the nextPageToken returned in the response to request subsequent pages of
    results by setting the pageToken query parameter to the value of the nextPageToken.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-stackdriver.png
  humanURL: https://cloud.google.com/monitoring/docs/
  baseURL: https://///{project}/metricDescriptors
  tags: Monitoring
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/monitoring/master/_listings/google-stackdriver-monitoring/projectmetricdescriptors-get-openapi.md
- name: Google Stackdriver Monitoring Post Project Metric Descriptors
  x-api-slug: google-stackdriver-monitoring
  description: Create a new metric.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-stackdriver.png
  humanURL: https://cloud.google.com/monitoring/docs/
  baseURL: https://///{project}/metricDescriptors
  tags: Monitoring
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/monitoring/master/_listings/google-stackdriver-monitoring/projectmetricdescriptors-post-openapi.md
- name: Google Stackdriver Monitoring Delete Project Metric Descriptors Metric
  x-api-slug: google-stackdriver-monitoring
  description: Delete an existing metric.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-stackdriver.png
  humanURL: https://cloud.google.com/monitoring/docs/
  baseURL: https://///{project}/metricDescriptors/{metric}
  tags: Monitoring
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/monitoring/master/_listings/google-stackdriver-monitoring/projectmetricdescriptorsmetric-delete-openapi.md
- name: Google Stackdriver Monitoring Get Project Timeseries Metric
  x-api-slug: google-stackdriver-monitoring
  description: List the data points of the time series that match the metric and labels
    values and that have data points in the interval. Large responses are paginated;
    use the nextPageToken returned in the response to request subsequent pages of
    results by setting the pageToken query parameter to the value of the nextPageToken.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-stackdriver.png
  humanURL: https://cloud.google.com/monitoring/docs/
  baseURL: https://///{project}/timeseries/{metric}
  tags: Monitoring
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/monitoring/master/_listings/google-stackdriver-monitoring/projecttimeseriesmetric-get-openapi.md
- name: Google Stackdriver Monitoring Post Project Timeseries Write
  x-api-slug: google-stackdriver-monitoring
  description: Put data points to one or more time series for one or more metrics.
    If a time series does not exist, a new time series will be created. It is not
    allowed to write a time series point that is older than the existing youngest
    point of that time series. Points that are older than the existing youngest point
    of that time series will be discarded silently. Therefore, users should make sure
    that points of a time series are written sequentially in the order of their end
    time.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-stackdriver.png
  humanURL: https://cloud.google.com/monitoring/docs/
  baseURL: https://///{project}/timeseries:write
  tags: Monitoring
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/monitoring/master/_listings/google-stackdriver-monitoring/projecttimeserieswrite-post-openapi.md
- name: Google Stackdriver Monitoring Get Project Timeseriesdescriptors Metric
  x-api-slug: google-stackdriver-monitoring
  description: List the descriptors of the time series that match the metric and labels
    values and that have data points in the interval. Large responses are paginated;
    use the nextPageToken returned in the response to request subsequent pages of
    results by setting the pageToken query parameter to the value of the nextPageToken.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-stackdriver.png
  humanURL: https://cloud.google.com/monitoring/docs/
  baseURL: https://///{project}/timeseriesDescriptors/{metric}
  tags: Monitoring
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/monitoring/master/_listings/google-stackdriver-monitoring/projecttimeseriesdescriptorsmetric-get-openapi.md
- name: Google Stackdriver Monitoring
  x-api-slug: google-stackdriver-monitoring
  description: Google Stackdriver provides powerful monitoring, logging, and diagnostics.
    It equips you with insight into the health, performance, and availability of cloud-powered
    applications, enabling you to find and fix issues faster. It is natively integrated
    with Google Cloud Platform, Amazon Web Services, and popular open source packages.
    Stackdriver provides a wide variety of metrics, dashboards, alerting, log management,
    reporting, and tracing capabilities.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-stackdriver.png
  humanURL: https://cloud.google.com/monitoring/docs/
  baseURL: https:///
  tags: Monitoring
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/monitoring/master/_listings/google-stackdriver-monitoring/openapi.md
x-common:
- type: x-developer
  url: https://cloud.google.com/monitoring/api/v3/
- type: x-website
  url: https://cloud.google.com/monitoring/docs/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---