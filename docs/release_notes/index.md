# Release Notes

The release notes list the GitHub issues and a summary of what has changed in PeeringDB software releases.

Each new release has a one week beta test period on the [beta server](https://beta.peeringdb.com/) before it goes live.  The beta and new releases are announced on the [PeeringDB Announce Mailing List](https://lists.peeringdb.com/cgi-bin/mailman/listinfo/pdb-announce) and on [Twitter](https://twitter.com/PeeringDB), [LinkedIn](https://www.linkedin.com/company/peeringdb) and [Facebook](https://www.facebook.com/peeringdb).

This page was started in April 2020, and will only have information about PeeringDB releases starting from that date.

## Release 2.20.0
Planned Beta Announcement Date: 14 April, 2020
Planned Release Date: 22 April, 2020
Changes: [GitHub Milestone](https://github.com/peeringdb/peeringdb/milestone/37?closed=1)

| **GitHub Issue** | **Summary** |
| ----------------- | ----------- |
| [#151 - Validation of IRR Records](https://github.com/peeringdb/peeringdb/issues/151) |  |
| [#189 - Improve explanatory and help text](https://github.com/peeringdb/peeringdb/issues/189) | A clear help text is added for requesting affiliation to an organisation.  |
| [#251 - Limit number of concurrent affiliation requests per user](https://github.com/peeringdb/peeringdb/issues/251) | In order to reduce organization affiliation request spamming, the number of pending organization requests has been limited to 5. |
| [#295 Desk pro tickets -> DeskPRO tickets](https://github.com/peeringdb/peeringdb/issues/295)  | This is a bug fix and only affects the Admin UI. |
| [#378 - Add contact information for Facilities (fac) the same way as for ix and net](https://github.com/peeringdb/peeringdb/issues/378) | Contact information is added to Facilities and IXP. |
| [#452 - Org/Network name of a sponsor should not link to /sponsors, only the sponsor badge should](https://github.com/peeringdb/peeringdb/issues/452) | This is a bug fix. From now on only when clicking on the sponsor badge will direct to the sponsor page. |
| [#462 - Route-server URL starting with ssh://](https://github.com/peeringdb/peeringdb/issues/462) |  |
| [#539 - Add attribute 'operational' to 'netixlan'](https://github.com/peeringdb/peeringdb/issues/539) | This is a new feature and allows networks to give early notice to their peers that they soon will show up at an IXP. There is a new check box when adding an IXP connection. By default, a connection is considered operational and the box is ticked. When the connection is still in provisioning status, please untick the box. When viewing, the warning glyphicon is shown right to the network name. The correspondent API object netixlan is enhanced by a boolean field operational defaulting to true. This feature is in line with the [Data Ownership Policy](../gov/misc/2020-04-06_PeeringDB_Data_Ownership_Policy_Document_v1.0.pdf). |
| [#548 - containerize server](https://github.com/peeringdb/peeringdb/issues/548) | Internal software deployment system has been changed to use containers which reduces time spent by the ops team for deployments, allows for better scaling, and reduces the cost of entry for new developers to write and test their code. |
| [#555 - Notes field translate button disappears](https://github.com/peeringdb/peeringdb/issues/555) | This is a bug fix. The "Translate" button is there for a moment and then disappeared. |
| [#557 - Show all languages on beta, even if translation is not ready for prod](https://github.com/peeringdb/peeringdb/issues/557) | As soon as a new translation is starting it is available on the beta to help the translators and to encourage the community for input. |
| [#598 - bug caused by the org affiliationship request without an asn](https://github.com/peeringdb/peeringdb/issues/598) | This is a bug fix and is only relevant for the PeeringDB Admin Committee. |
| [#609 - When creating an ix via the API also return ixlan_id and ixpfx_id](https://github.com/peeringdb/peeringdb/issues/609) | When creating an IX record via API, the call will also return the implicitly created ixlan_id and ixpfx_id. This makes it simpler and reduces the number of calls that need to be made to the API. |
| [#615 - Insert links into ID fields in DESKPRO AUTOASN tickets](https://github.com/peeringdb/peeringdb/issues/615) | This only affects tickets generated for PeeringDB Admin Committee. A link to the object in the UI is added. |
| [#626 - Update API docs](https://github.com/peeringdb/peeringdb/issues/626) | Internal mechanisms for generating the API docs have been updated to current standards. This also allows for easier user contributions to the docs themselves. |
| [#634 - Remove support for python2](https://github.com/peeringdb/peeringdb/issues/634) | Python 2.7 and 3.4 support is removed bring removed from PeeringDB packages. |
| [#636 - Don’t create a new net object, when there only is an ASN block](https://github.com/peeringdb/peeringdb/issues/636) | This is a bug fix and is only relevant for the PeeringDB Admin Committee. |
| [#667 - Fix use autocomplete fields in the admincom controlpanel to speed up loading times](https://github.com/peeringdb/peeringdb/issues/667) | This is a bug fix and is only relevant for the PeeringDB Admin Committee. |

**Notes:** 
[#519 Make spelling of traffic levels consistent](https://github.com/peeringdb/peeringdb/issues/519) is also planned to be added to beta.peeringdb.com in April 2020 however it will NOT be released in the immediate next release (2.20.0). This is in order to allow more time for API users for awareness and testing. It will be added to a future May/June release.






