# AWS WAF dashboards Search pack
----
This pack serves as a starting point to get started with searching and visualising the AWS WAF logs. 

## About this Pack
This pack is using the out of the box JSON format produced by AWS WAF logging.


## Deployment
The default dataset displays sample data just to show you the art of the possible. 
To connect it to you real dataset, create the S3 dataset pointing at the S3 bucket containing WAF logs and update the `wafDataset` macro value from this:
* `"$vt_lookups" lookupFile="waf_data" | extract type=json`

To this (assuming your search dataset name is `waf_data`):
* `"waf_data"`

## Upgrades

## Release Notes

### Version 0.0.4 - 2025-10-31

Updated pack setting and moved the search queries into saved searches.


### Version 0.0.3 - 2025-09-26

Initial release 

## Contributing to the Pack
 
To contribute to this Pack, or to report any issues or enhancement requests, please connect with Michael Hyatt on [Cribl Community Slack](https://cribl-community.slack.com).

## Contact
To contact us please email mhyatt@cribl.io

## License
All publicly posted Packs must include a license that allows for use by the general public, such as Apache 2.0, MIT, or GNU.
(Most Packs use the Apache 2.0 license.)

This Pack uses the following license: [`Apache 2.0`](https://github.com/criblio/appscope/blob/master/LICENSE).