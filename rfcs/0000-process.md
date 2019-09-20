# Request for Comments

You need to follow this process if you intend to make a "substantial"
change to Suricata or a development process for Suricata. Changes that
require increased visibility, change how Suricata works in a
significant way, or change how we do things significantly should be
accompanied with an RFC. Although there isn't a strict set of rules
about what changes require an RFC, the following are examples of
changes which require an RFC:

* Any end user breaking change (change of output, configuration).
* Example 2
* Example 3

Examples of changes which do not require an RFC: 

* Internal changes to Suricata that do not affect input or output in a
  breaking fashion.

# Before Creating an RFC

A hastily-proposed RFC can hurt its chances of acceptance. Low quality
proposals, proposals for previously-rejected features, or those that
don't fit into the near-term roadmap, may be quickly rejected, which
can be demotivating for the unprepared contributor. Laying some
groundwork ahead of the RFC can make the process smoother.

Although there is no single way to prepare for submitting an RFC, it
is generally a good idea to pursue feedback from other project
developers beforehand, to ascertain that the RFC may be desirable;
having a consistent impact on the project requires concerted effort
toward consensus-building. It may be helpful to follow the RFC process
in the project most impacted, and then decide to promote to an
engineering RFC after discussion.

# What the Process Is

One must first get the RFC merged into the RFC repository as a
markdown file. At that point the RFC is "active" and may be
implemented with the goal of usage in engineering.

* Open an issue in the [RFC Project](https://github.com/oisf/suricata-rfcs/issues),
  with a basic description of your RFC.
* Clone the [repository](https://github.com/oisf/suricata-rfcs/)
* Create a branch rfcNNNN for your rfc, where NNNN corresponds to your
  issue number.
* Copy 0000-template.md to rfcs/NNNN-NAME.md where NAME is a short
  descriptive name for the RFC.
* Commit your changes, referencing your issue
* Push your branch
* Create a pull request for your branch
* Tag relevant suricata team members and request comments. It may also
  help to link your RFC on the Suricata IRC channels on FreeNode
  (#suricata and/or #suricata-dev), and the oisf-devel mailing list.
* When comments on the RFC have mostly reached a completion point
  (resolution or not), request Final Comment Period (FCP).
* Wait for completion of FCP (5 days).
  * This period can be compressed with Core team or higher
    approval. The Core team or higher approving the new FCP completion
    time must comment on the issue with the new FCP completion time
* If arguments or ideas are raised during FCP which make the RFC
  unacceptable, the RFC will go back to development mode. If no
  arguments or ideas are raised, the RFC will be merged or closed by
  Core team or higher.

# RFC Lifecycle

Once an RFC becomes active (issue is open and under discussion),
authors may implement the changes associated with it and prepare a
merge request against the appropriate project.

## References 

* [Rust RFC process](https://github.com/rust-lang/rfcs)
* [React RFC process](https://github.com/reactjs/rfcs)
* [Ember RFC process](https://github.com/emberjs/rfcs)
