# Product Tools

## Request Tracking \(Features, Bugs, Chores\)

We use [Clubhouse](https://app.clubhouse.io/replicated) as our story tracking system.

* Clubhouse [Quick Start Video](https://help.clubhouse.io/hc/en-us/articles/360049156072-Quickstart-Guide-New-Users-Members-)
  * [Tool Best Practices Guide](https://drive.google.com/file/d/1OICe-1Ed5y0wE0HNpKpStPjCAipOAvTo/view) from Clubhouse
* Walkthrough: [How to Enter a Feature or Bug Using a Clubhouse Template](https://docs.google.com/document/d/12oft90vPWFxfuRnspBMoacu2I-yjpAqDj8WuncF3aj0/edit?usp=sharing) \(internal link\)
* Walkthrough: [How the Clubhouse/Zapier automation works](https://drive.google.com/file/d/1dthwm5bQ1-U0iZOEPP6RXqnI_5zTrWgA/view?usp=sharing) \(internal link\). This allows us to connect clubhouse to our customer’s github issue trackers, and automatically notify them when their fix/request is released.
  * Things to be aware of given this automation:
    * We don’t move an item to “completed” until it is actually shipped. Items that are moved to the “completed” status in Clubhouse will automatically notify the customer that the item is completed in their linked github repo issue.
    * If Replicated creates the Clubhouse issue, and puts a customer requester label on it, the automation will create a corresponding issue in the customer’s Github tracker. The only content copied over is the title. Story titles should be meaningfully descriptive and external-friendly.

## Product Testing

### kURL

#### Test Grid

The kURL team uses [Test Grid](https://testgrid.kurl.sh) to test kURL. These tests are run daily on both staging and production, as well as when pull requests are created. A test performs a kURL installation of a particular spec on a particular operating system. For example, deploying [https://kurl.sh/0c3ff8a](https://kurl.sh/0c3ff8a) on CentOS 8.1 would be one test. Each test also uses Sonobuoy for conformance testing. Test Grid shows the number of successful, failed, and pending installs for each run.

The daily runs perform all the defined tests. This includes the installation of particular specs, upgrading from one particular spec to another, installing air gap bundles, etc. The test runs that are triggered by PRs perform a subset of tests, which are determined by the pull request changes.

For more detailed information, see the [Test Grid](https://wiki.replicated.io/doc/testing-help-Q6oPSqxvPh#h-testgrid-kurl) section of the engineering handbook.

### KOTS

#### TESTIM

An in initial walkthrough is available in the following Zoom recording: [https://replicated.zoom.us/rec/share/kY232o1dze05VKJZ1mBD9m98hJBPmctr8rnllaC3ktfxUR7MDfys9zXMJB1mnKmI.x714loRF7toxSqh1](https://replicated.zoom.us/rec/share/kY232o1dze05VKJZ1mBD9m98hJBPmctr8rnllaC3ktfxUR7MDfys9zXMJB1mnKmI.x714loRF7toxSqh1)

Passcode: S%&\*3S&&

#### kGrid

[kgrid](https://github.com/replicatedhq/kgrid) is a Kubernetes operator that is hosted in Replicated infrastructure with the purpose of running automated KOTS installs of vendor applications. kgrid helps ensure that we test each new KOTS version release against a selection of customer applications in order to reduce the risk of KOTS release regressions and other breaking changes that could unintentionally impact one of our customers.

More detail on how kgrid works is available in this [internal doc](https://docs.google.com/document/d/1L0-0yuYQevVCHi-xUB3QLCuoybvi30rVmC6w1bHNcl4/edit#heading=h.9dxn3dccs7b).

An initial walkthrough is available in the following Zoom recording: **&lt;**[**https://replicated.zoom.us/rec/share/LKF-ba-N9JgS-MsTr7QUXTH7w\_dltelRAX-D1ocQExxLZ24DPdnY1YerGKyArpcl.WKQZObqhLR7R\_NH7**](https://replicated.zoom.us/rec/share/LKF-ba-N9JgS-MsTr7QUXTH7w_dltelRAX-D1ocQExxLZ24DPdnY1YerGKyArpcl.WKQZObqhLR7R_NH7) **\]\(**[**https://replicated.zoom.us/rec/share/LKF-ba-N9JgS-MsTr7QUXTH7w\_dltelRAX-D1ocQExxLZ24DPdnY1YerGKyArpcl.WKQZObqhLR7R\_NH7**](https://replicated.zoom.us/rec/share/LKF-ba-N9JgS-MsTr7QUXTH7w_dltelRAX-D1ocQExxLZ24DPdnY1YerGKyArpcl.WKQZObqhLR7R_NH7)**\)**

Passcode: aF0=!31\*

