# TC39 and IP

## How TC39 works

TC39 is a technical committee of Ecma, which creates and maintains ECMA-262, the standard for the JavaScript programming language, and some
other JavaScript-related specifications such as ECMA-402 ("Intl").

### Meetings

TC39 meets once every two months for three days. Meetings are primarily attended by delegates from Ecma member organizations. Non-members who are invited by the committee to attend TC39 can do so in two ways:
- "Invited Experts" may contribute to the discussions.
- "Observers" are simply watching a TC39 meeting, without
contributing.

In practice, both of these designations are most often used for prospective Ecma members, and rarely for other purposes. In these meetings, we discuss proposals, recommend modifications, and promote proposals through a ["stage" process][1]. When a proposal advances to Stage 4, we add it to the draft specification.

### Work on GitHub

Most deep technical work in TC39 takes place on GitHub. The [main specification][2] has a GitHub repository, as do other specifications such as [ECMA-402][3]. Small changes to the draft specification are done via GitHub Pull Requests, and larger changes are done via staged proposals which are maintained in [separate GitHub repositories][4].

### Annual specification releases

Every year, around the end of January or beginning of February, the ECMA-262 editor makes a branch of the ecma262 repository for future as the annual "ECMAScript20xx" standard. Backports of small fixes, both editorial and normative, may be targeted at this branch, but new features are not landed there. In June, this branch is passed on to the Ecma General Assembly for ratification as an Ecma standard.

## Legal agreements

### Ecma membership agreements

Ecma members are organizations, such as corporations or
universities, which sign up in one of [Ecma's membership categories][5]. There are separate forms for each membership category, but they each contain the following text:

b) We confirm that we have knowledge of the By-laws, Rules and the
Code of Conduct in Patent Matters of Ecma International and that we
will comply with them.
c) We irrevocably grant Ecma International the right to use
contributions, in part or whole, whether adapted or not, that we
submit to Ecma International, for Ecma International’s purposes of
standardisation, while we retain all the rights we may have on those
contributions.

Ecma members who participate in TC39 must sign the RFTG agreement as
well, described below.

### Contributor IPR license

TC39 is open to individuals who are not associated with Ecma members to contribute, either through comments made in TC39 meetings as invited experts, or as normative patches to the specification made via GitHub. Both of these kinds of contributors are required to sign [the non-member contributor agreement][6].

If a TC39 delegate does not have an agreement with their relevant member organization that allows the member organization to license the related IPR to Ecma, then the delegate must individually sign the non-member contributor agreement as well.

When a non-member contributor works within an organization where they do not have the authorization to license their contributed IPR, the form can be filled out with separate "signatory" and "contributor" fields, where the "contributor" is the participant in TC39 work, and the "signatory" is the member of the organization who is authorized to license the IPR. The form must be signed for each individual contributor who participates in TC39, and does not apply organization-wide.

### Ecma Royalty-Free Task Groups

Ecma specifications generally have related patents from member
organizations licensed under RAND scheme, but TC39 uses a distinct
royalty-free policy based on the use of Ecma's ["Royalty-Free Task
Groups"][7]. All of TC39's work actually takes place in the TC39 RFTG, with a [separately-tracked membership][8]. The period between the branch point and ratification at the GA serves as the Opt-Out Review Window. Such an Opt-Out has never been taken in TC39's history.

### Copyright licenses

The annual ECMA-262 and ECMA-402 are licensed under Ecma's [text
copyright policy][9].

TC39 maintains a test suite for ECMA-262 and ECMA-402, called test262, which is licensed under [Ecma's software license][10]. Contributors to test262 are required to sign the separate [software submitter license][11]. Files added to test262 have a [copyright header indicating an initial author][12], following previous legal advice; it is unclear whether this is actually needed, and test262 maintainers would prefer to
not require this header.

### Processes to ensure contributors have granted appropriate licenses

- In physical meetings, the chair and vice chairs verify that all meeting attendees are either delegates of member companies, or otherwise have chosen among the observer/invited expert options explained above. There is a quick agenda item to clarify the IPR agreements.
- For contributions on GitHub, there is [a bot in development][13] to check that non-member contributors have signed the appropriate agreement.  Until then, the set of contributions has been manually surveyed going back to the beginning of GitHub use, and all contributors have been verified to have signed the agreement; this manual check continues for current contributions.

[1]: http://tc39.github.io/process-document/
[2]: https://github.com/tc39/ecma262/
[3]: https://github.com/tc39/ecma402/
[4]: https://github.com/tc39/proposals/
[5]: http://www.ecma-international.org/memento/join.htm
[6]: https://tc39.github.io/agreements/contributor/
[7]: https://www.ecma-international.org/memento/Policies/Ecma_Royalty-Free_Patent_Policy_Extension_Option.htm
[8]: https://www.ecma-international.org/memento/TC39-RF-TG.htm
[9]: https://www.ecma-international.org/memento/Ecma%20copyright%20FAQ.htm
[10]: https://www.ecma-international.org/memento/Policies/Ecma_Policy_on_Submission_Inclusion_and_Licensing_of_Software.htm
[11]: https://tc39.github.io/test262-cla/
[12]: https://github.com/tc39/test262/blob/master/CONTRIBUTING.md#test-case-style
[13]: https://github.com/IgnoredAmbience/tc39-bot/