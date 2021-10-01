# Being a Product Manager at Replicated

On this page, you’ll find an overview as well as links to helpful resources for working as a product manager at Replicated.

## Core Responsibilities

**As a PM at Replicated, you are primarily responsible for:**

* Understanding and communicating the problems of our users and our customers
* Contributing to building products and capabilities desirable to our users and customers
* Ensuring that our product continues to be viable for Replicated

**As a PM you should be able to communicate**

* What we are doing
* Why doing these things is valuable
* How we are measuring that we’re being successful.

**Success for a PM at Replicated looks like:**

* Demonstrated ownership of your product\(s\) and/or problem space\(s\), working with your team to innovate and improve these areas based on a strong understanding of customer wants/needs and business wants/needs.
* Working cross functionally with other groups needed to successfully implement cross-team initiatives.
* Contributing to how we shape and evolve Replicated’s product culture.
* Modeling product thinking to enable the entire team to be asking why, making good product decisions even when you can’t be available

## Core PM Tasks

* Triage new issues in your product/problem space area \(features, bugs, security vulnerabilities\)
  * New stories should route into the “Untriaged” column of ClubHouse. As a PM, you should be paying attention to this column and triaging new stories.
  * Is the story assigned to the right project? If not, reassign it and tag the correct PM
  * Is the story in the right categorization? Feature vs Bug
  * Are the right labels applied to the story? Is the customer requestor label present \(if applicable\)? Is it a `customer-blocker` or a `regression`. We sometimes use labels to help classify functional groupings, such as `vendor-cli` or `preflights`. This is at your discretion to apply if you find useful to making stories easier to find.
  * See [Prioritization](https://wiki.replicated.io/doc/product-process-6uKJ1RPmCd#h-prioritization)
  * As you review, please move them into the correct column \(ex: Unscheduled, Backlog, This Week\) once you’ve had an opportunity to determine how the request should be prioritized.
* Backlog Prioritization
* Iteration and Release planning
  * **Weekly Priorities:** The team should be working on at least one strategic thing during each week’s iteration, preferably more.
  * **Release notes:** The engineering team is expected to contribute to the release notes for each release, but the PM is typically the final reviewer. Look for styling consistency, and readability. Can a reader easily understand what change was made, and why?
* Contribute to weekly internal-facing product update email content
  * During the week, or by the end of the week, you should have contributed your product area highlights to the weekly Product Update email that we typically send out on Monday to the entire company. [Working draft](https://docs.google.com/document/d/1KpxBnOPExVQsS95MCsCbb4vpsJgmerUGC9czYZCVilc/edit)
* Participate in weekly support retros
  * These are excellent opportunities to get more exposure to product issues. It is also a great opportunity to get additional input on urgency from the engineer that helped resolve the issue.
  * As a PM you should be asking:
    * What would have made this easier to resolve?
    * What support analyzer could have caught this? \(We want to prioritize creation of these types of support analyzers\)
* Connect with key customers semi-regularly
* Review Product Telemetry
  * See [Product Telemetry section](https://wiki.replicated.io/doc/product-process-6uKJ1RPmCd#h-tools-to-understand-product-and-customer-data)
  * As we continue to improve here, we’ll expect PMs to pay attention to and report on relevant data points \(such as leading and lagging indicators\) and expand on what we are learning and/or how we are adjusting strategies based on this information
* Create monthly release post content, and any major release content
* Determine pricing tier for new features

Also see [How to Work as a PM](https://wiki.replicated.io/doc/product-process-6uKJ1RPmCd#h-how-to-work-as-a-pm).

## Getting started as a PM at Replicated

You should have been provided access to an Asana project to help you onboard successfully during your first month at Replicated. Eventually we’ll migrate that content over to this Handbook.

### New PM Tips - The Weekly Planning Meeting

* As the PM you should represent what key stories need to happen that week in order to drive forward our strategy and goals.
  * Reference [Prioritization](https://wiki.replicated.io/doc/product-process-6uKJ1RPmCd#h-prioritization)
  * If possible, consider doing weekly themes \(ex: improve customer management, improve app config capabilities and UX\) so the team is delivering towards a shared goal and a bigger impact is felt at the end of the week
  * It can be useful to review the upcoming [support schedule](https://replicated.app.opsgenie.com/schedule/whoIsOnCall) ahead of planning to get a sense of your team’s potential capacity for the week. When an engineer is on a support rotation, their ability to execute will be very limited for that week.
  * The VEXT Team is currently running an experiment with a dedicated bug track
    * Each week, one engineer will be dedicated exclusively to bug fixes. As a general rule, that engineer should be the engineer that was on day support last week.
    * This person will take care of the weekly team CVE, dependabot, testgrid upkeep chores. This person will work down the backlog tackling bugs exclusively, with the goal to squash as many as they can.
    * This person has the autonomy to cherry pick quicks wins from the backlog, but would ideally not skip over "customer-blocker" or "customer-high"
* Ask your other team members what they think we should be working on with any additional capacity. The larger team often advocates for bug fixes and improvements, and has valuable first hand experience on customer and/or supportability friction points from their support escalation involvement.
* When discussing stories, ensure we are considering designing for failure, not just the happy path.
* When discussing stories, look to break things down into the smallest parts needed to deliver and learn.
  * Break the big things down into the least risky decision
  * What's the minimum thing, the smallest increment you can ship this week, in order to learn/get-feedback?
  * If a feature release is dependent on several pieces being completed, consider putting it behind a feature flag so that we can continue to ship & iterate weekly without unmerged code building up. Also consider if this is an opportunity to get feedback from a smaller customer pool while the effort is still in progress.
* As part of the planning meeting, every story pulled into “This Week” should have an engineer assigned as the owner. We assign stories as part of the planning discussion. Before planning wraps up, ensure each team member has a good balance of work. We are striving for a balance of fast progress on the backlog with a sustainable workload that we believe can be completed within the week.
* The PM should not be the only source of input when questions, or trade-off considerations, are raised. Ask the team “what’s your recommendation?” When discussing potential tradeoffs or limitations. Product team members should be thinking about the impacts to business viability, usefulness and usability. Engineering should be helping to think about the technical feasibility, and other potential system impacts.

### New PM Tips - The Daily Standup Meeting

* We use a method often referred to as “Run the Board”. The team should talk through any newly completed stories first. Then the newly Ready for Deploy stories. The goal is to ensure alignment among the team that the feature is in the correct state and ready to call “done” or “ready for release” \(Testing plan in place? Docs in place?\). We then talk through each story in the In Development column one-by-one.

## Where should you look when you need help?

Consider asking your team for help if appropriate. You can also reach your fellow PMs in \#product on Replicated Slack.

