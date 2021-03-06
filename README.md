[![New Relic Experimental header](https://github.com/newrelic/opensource-website/raw/master/src/images/categories/Experimental.png)](https://opensource.newrelic.com/oss-category/#new-relic-experimental)

# New Relic Partner Enablement Microsite

The New Relic Partner Enablement Microsite is here to enable partners with their practical New Relic knowledge.

## Accessing and using the Microsite

[Public site](http://partners.newrelic-es.com/) is intended to be the default access  

## Contributing Content
We would love to have you contribute content to the microsite. We are accepting pull requests.

## Local Builds

`npm i` to install the dependencies

`gatsby develop` to run this repository locally - [http://localhost:8000](http://localhost:8000)

`npm build` to build the gatsby site

## Remote Builds

First, have had a local build. Then:

```shell
pip install awscli
aws configure
```
Modify [package.json](/blob/main/package.json) to include the name of your s3 bucket. 

That is essentially all! There are also [Gatsby docs](https://www.gatsbyjs.com/docs/how-to/previews-deploys-hosting/deploying-to-s3-cloudfront) - npm package is already included in this repo.

That's pretty much it! Then `npm run build && npm run deploy` 

### Relic Remote Builds
Following the above instructions and being a member of the AWS ES Org (no need to change s3 bucket).

If you're a Relic wishing to submit new content, you should enter a pull request and not perform a remote build.

The s3 bucket has an associated Cloudfront distribution which in turn has a Route 53 hosted zone and record. Changes to the bucket will directly go to the hosted zone. 

Slack'ing gspencer is the preferred approach - but you can do a remote build if Gary is out and you really need to.

## Support

New Relic hosts and moderates an online forum where customers can interact with
New Relic employees as well as other customers to get help and share best
practices. Like all official New Relic open source projects, there's a related
Community topic in the New Relic Explorers Hub. You can find this project's
topic/threads here:

## Contributing

We encourage your contributions to improve [project name]! Keep in mind when you
submit your pull request, you'll need to sign the CLA via the click-through
using CLA-Assistant. You only have to sign the CLA one time per project.
If you have any questions, or to execute our corporate CLA, required if your
contribution is on behalf of a company,  please drop us an email at
opensource@newrelic.com.

## Security

As noted in our [security policy](../../security/policy), New Relic is committed
to the privacy and security of our customers and their data. We believe that
providing coordinated disclosure by security researchers and engaging with the
security community are important means to achieve our security goals.

If you believe you have found a security vulnerability in this project or any of
New Relic's products or websites, we welcome and greatly appreciate you
reporting it to New Relic through [HackerOne](https://hackerone.com/newrelic).

## License

The New Relic Partner Enablement Microsite is licensed under the
[Apache 2.0](http://apache.org/licenses/LICENSE-2.0.txt) License.

The NR1 App Buildert also uses source code from third-party libraries. You can
find full details on which libraries are used and the terms under which they
are licensed in the third-party notices document.
