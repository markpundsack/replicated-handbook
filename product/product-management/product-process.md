# Product Process

On this page, you’ll find an overview of how we do our PM work at Replicated.

## Team Meetings

* Product Meeting \(Weekly\)
  * What: A weekly meeting for the Product team. All team members can add items to the agenda \(in meeting planner\). Examples of potential agenda items: Discussion of a strategic item; Sharing interesting customer insights from the week.

## Communication

* Weekly Product Team Meeting
* [Product slack channel](https://app.slack.com/client/T031GF04S/C68QDSQ64)

### Working with Product Marketing \(PMM\)

\(Content coming\)

### Release Posts

As a PM, you are accountable for contributing content to our monthly feature release blog. Currently Amber writes this each month, but the intention is to begin to rotate post creation leadership among the PMs each month. These posts should highlight customer meaningful feature benefits that may not warrant their own dedicated feature release. We often create these posts from the weekly, internal product update email, so keeping up with content contributions is key.

## How to work as a PM

### Strategic Planning

* Prioritize impact. How might we make a small change that can make a big impact?
* Break things down into Problems & Opportunities; Identify Assumptions

### Prioritization

The following types of issues should always be prioritized highly:

* Security patches
  * bugs via bug bounty program will be labeled `requester/hackerone`, general security will be labeled `area/security`
* Critical bugs
  * labeled`p0;`a P0 is an issue that affects customers with no reasonable workaround
* Introduced regressions
  * labeled `regression`
* Blocking customer requests
  * labeled `customer-blocker`
* Issues with performance, stability, reliability
* Issues with ease of use

Other factors that can raise issue/request priority

* It is strategically valuable for our broader goals \(labeled `direction`\)
* The Solutions Engineering team has ranked it as a Top-10 want \(labeled `se/top-ten`\)
  * Meant to represent key requests that would help close deals, reduce sales or POC friction
* The TAM \(Technical Account Manager\) team has ranked it as a Top-10 want \(labeled `tam/top-ten`\)
  * Meant to represent a curated set of key requests across many customer top ten rankings
* Multiple customers are requesting and/or being impacted \(labels follow a `requester/(customer name)` convention\)
* A customer has ranked it as a top item for them \(labeled `customer-high`\)
* The product Engineering team has marked it as something they think is important \(labeled `engineering-high`\)

\(Content on Prioritization models coming\)

### Iteration Strategies

\(Content coming\)

### Team Execution Best Practices

* Docs are required for a feature to be complete. Docs are not an afterthought and should be part of the story implementation discussion
* Proper testing is required for a feature to be complete. Consult the [Guidelines for Releasing a Major Feature](https://wiki.replicated.io/doc/product-process-6uKJ1RPmCd#h-guidelines-for-releasing-a-major-feature) as a reference for the types of testing permutations that may apply.
* Regression related bugs shouldn’t be marked as completed unless a test to prevent it from happening again has been added
* The team is responsible for the repos in their product/problem space. This includes ensuring PRs from customers receive feedback and consideration in a timely manner and that dependency related PRs are merged regularly.

### Working with Customers

At Replicated we record our notes for a customer meeting within that customer’s shared google doc within the Replicated Drive. Relevant notes may end up in stories, proposals, etc, but as a general rule, a record of your customer conversation, and any associated feedback and/or action items, should be captured in the main \(shared\) customer notes doc.

### Sourcing Customer Input

\(Content coming\)

### Tools to understand product and customer data

\(Content Coming\)

### \#Product Considerations

* **Upgradability**
  * Customers should always be able to move between versions of our software with minimal friction
  * For kURL: We'll make sure clusters are always upgradable unless an add-on introduces a breaking change
* **Breaking changes:**
  * No breaking changes or deprecations should occur until a planned major version change. Ideally, major versions should consider announcing 6-12 mo out.
  * If a feature is in BETA, PMs have more flexibility to change/eliminate, but consider the impact on any customers that may have leveraged beta functionality.
* **Product Versioning \(KOTS\)**
  * Major = large changes in functionality, breaking changes, changes in underlying defaults \(ex: moving from Helm v2 default to Helm v3 default\)
  * Minor = new features, meaningful improvements
  * Patch = Bug fixes, minor improvements
  * LTS = We do not currently offer an LTS \(long-term support release\). An LTS release should be limited to security patches and possibly bug fixes.
* **Special Technology Considerations**
  * Use of MinIO - Minio is under the AGPL v3 license.
    * \(more content coming\)
  * Use of Grafana, Loki, or any other software under AGPL v3 license.
    * As of May 2021 any current use of these technologies in Replicated’s stack is approved. If we intend to make any architectural changes and/or new uses of these technologies \(new features, etc\) you must review with leadership before proceeding.

### Product Security Considerations

* If there's an upstream patch available in an open source component that we use, then we need to update in our products. We have not committed to fixing all upstream CVEs \(i.e. where there's not a patch available\). Our goal is to avoid forking and maintaining customer images of upstream components, and we strive to automate our CVE upkeep process.
* [Vulnerability and CVE Policy](https://kots.io/vendor/packaging/vulnerability-patch-policy/)

### Product Support Considerations

* kURL: We support the supported versions of Kubernetes \(n-2\)
* KOTS: We support KOTS running on the supported Kubernetes versions we declare in the KOTS docs \(release notes, system requirements\). When a given version of Kubernetes falls out of support, we technically no longer support those KOTS versions where Kubernetes compatibility is fully outdated.

### Guidelines for Releasing a Major Feature GA

_Not all of these items may apply in all scenarios._

* **Business Readiness Considerations**
  * Customer facing business teams are aware of intended scope and delivery timeline
  * Marketing team is aware of intended scope and delivery timeline
  * Product team has received sufficient input/feedback \(during BETA, etc\) to feel confident defining GA boundaries
  * Product team has determined pricing strategy for feature availability, and shared these plans with Sales & Customer Engineering teams
  * Product team has PMM engaged on GTM positioning
  * Product team has engaged Marketing team in advanced conversation on launch messaging
  * Cross-team demo/training was provided to Customer Engineering Team
* **Support Readiness Considerations**
  * Product & Engineering have engaged Support Team to discuss intended scope and delivery timeline and potential risks for supportability \(staffing, tech knowledge, etc\)
  * Cross-team demo/training was provided to Support Team
* **Product Readiness Considerations**
  * Compatibility & Permutation Testing: Embedded Cluster
  * Compatibility & Permutation Testing: Existing Cluster
  * Compatibility & Permutation Testing: Interactive, manual installs/updates
  * Compatibility & Permutation Testing: GitOps automated installs/updates \([https://kots.io/kotsadm/installing/automating/](https://kots.io/kotsadm/installing/automating/)\)
  * Compatibility & Permutation Testing: Minimal RBAC
  * Compatibility & Permutation Testing: Single Vendor, Single App
  * Compatibility & Permutation Testing: Single Vendor, Multi-App
  * Compatibility & Permutation Testing: Multi "Single App" Vendors
  * Compatibility & Permutation Testing: Multi "Multi App" Vendors
  * Troubleshoot analyzers & support bundles have been added and/or updated as appropriate for this feature
  * Regression, security & other on-going test coverage updated as appropriate
  * Feature\(s\) validated with key customers and/or traditionally problematic customer applications
  * Appropriate user-facing feature docs are available
  * Desired feature metrics are in place \(defined, being collected, available in reporting\)
  * Key features identified by team as must-have for GA are complete

