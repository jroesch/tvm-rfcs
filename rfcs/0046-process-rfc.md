- Feature Name: process_change_process
- Start Date: 2021-12-08
- RFC PR: [apache/tvm-rfcs#0000](https://github.com/apache/tvm-rfcs/pull/0000)
- GitHub Issue: [apache/tvm#0000](https://github.com/apache/tvm/issues/0000)

# Summary
[summary]: #summary

Today in the TVM community many processes have been left implicitly documented and maintained
as tribal knowledge. This was a perfectly acceptable way to operate as a smaller community but
is bringing new challenges as we grow. For example how can a community member suggest a process
change and also definitely know if it was accepted and thus endorsed by the larger community.

In order to address these challenges this RFC proposes the introduced of a Process RFC for
community-wide process changes. The goal of a process RFC is to:
1) Introduce a change not in the technical architecture of TVM, but to change the community architecture.
2) Result in a clear acceptance decision instead of soft-consensus on the mailing list or GitHub.
3) Result in clear documentation about accepted processes so new community members can learn how to
   properly follow community adopted processes.

# Motivation
[motivation]: #motivation

As we are growing many community members are getting busier and busier with their community responsibilities
as well as their own jobs and lives. We need to have clear processes that can scale to a larger community, a
and enable more community members to be productive without needing direct transmission of tribal knowledge.

One challenge today is we often discuss process changes but do not come to an official decision, or if we do
we do not document clearly enough for new community members to understand how to execute it.

To be concrete, in the past CI has been a process completely maintained by tribal knowledge of the PMC, and
if we wanted to codify new changes to our CI processes it is not clear how a contributor could suggest, ratify,
and rollout such a change without joining the PMC.

In the spirit of Apache we want to enable more of the community to help shape and grow the community without
having to first join the PMC before being able to influence the community.

# Guide-level explanation
[guide-level-explanation]: #guide-level-explanation

n/a

# Reference-level explanation
[reference-level-explanation]: #reference-level-explanation

My proposal is simple, a process rfc is just an RFC with extra semantics.

A process RFC enables a TVM community member to suggest a change in process for the TVM community which
can be discussed for a period of time.

1) The proposer will post the Process RFC, and can be anyone, including new contributors.
2) A TVM committer will be assigned to be the shepard of the process RFC.
3) After the arguments have been presented the shepard will invoke a committer vote which will last 10
days to ensure ample time to make any final arguments and vote.
4) At the end of the discussion the RFC will either be accepted, rejected or postponed.
5) The proposer will be responsible for converting the RFC to process documentation which will be committed to
   the official Apache TVM documentation.

# Drawbacks
[drawbacks]: #drawbacks

This adds more process then we currently have, but an overwhelming piece of feedback from the community is
that is not clear who can, and should make these changes. Then when changes are proposed what the timeline,
ratification, and rollout processes are.

# Rationale and alternatives
[rationale-and-alternatives]: #rationale-and-alternatives

I believe this design to be relatively simple, it just exposes a mechanism for any community member
to influence the project while remaining inline with Apache-style governance.

# Prior art
[prior-art]: #prior-art

Other communities use disagree-and-commit mechanisms to ensure that timely consensus is
reached and that processes eventually result in an outcome, even if its clear postponement
or rejection.

# Unresolved questions
[unresolved-questions]: #unresolved-questions

There are more details to work out about documenting this process, the form of process
documentation, and tweaking hyper parameters (i.e. comment period, voter calling, assignee),
which I expect to come out during RFC discussion.

# Future possibilities
[future-possibilities]: #future-possibilities

This will enable us a clear way to evolve things such as the RFC process, CI,
nightlies and so on in a way that empowers all contributors, but also fits into
the Apache way.
