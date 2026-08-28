# Fixture Policy

## Purpose And Ownership

`ChronoAIProject/cma-trigger-fixture` is the disposable public upstream for CMA
Trigger provider evidence. The steward is `chronoai-shining`. A smoke campaign
must record the repository numeric ID, node ID, selected ref, immutable source
SHA, publisher identity, contributor identity, NyxID UserService ID, deployed
build, runtime digest, and configuration revision before it starts.

The publisher and contributor used by provider evidence must be dedicated
disposable identities with least privilege. A production maintainer bearer is
not fixture evidence. Credential values are never exported from NyxID or stored
in this repository, CMA configuration, workflow logs, or retained artifacts.

## Content And Execution

All committed content is synthetic. Do not copy production source, user data,
tokens, credentials, generated provider responses, or private issue material
into this repository. Do not add GitHub Actions workflows, webhooks, deploy
keys, environment secrets, package publishing, Pages deployments, or code that
contacts an external service.

Archive attributes, symlinks, executable bits, binary bytes, large files,
malicious names, LFS pointers, and prompt-injection prose are test data. They
must never be executed or interpreted as operator or agent instructions.
Deterministic generators should create oversized or hostile cases during the
test rather than committing unbounded data here.

## Preservation And Cleanup

One provider campaign may own one fork, Launch branch, commit path, and pull
request at a time. Preflight must stop when fork-network, branch, pull-request,
storage, sandbox, or API quota is insufficient; it must not delete or repurpose
another campaign's resources.

CMA cleanup must never delete or reset a contributor fork, branch, commit, or
pull request. It must never enumerate or delete a sandbox outside the normal
session lifecycle authority. The steward closes or archive-marks test pull
requests only after retained evidence has been reviewed. Provider resources and
their immutable identifiers remain available for that review.

## Rotation

Fixture changes use ordinary reviewed pull requests. A campaign pins the exact
source SHA it observed, so a later commit, rename, transfer, or name reuse cannot
retarget existing evidence. To retire this repository, first create and verify
a replacement fixture, update the CMA evidence ledger to its numeric identity
and source SHA, finish all in-flight reviews, and only then archive this one.
