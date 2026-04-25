### What's changed in v1.0.0

* feat: rename project to aws-lbc-stack (by @patrickleet)

  BREAKING CHANGE: Renames the configuration package from aws-base-stack to aws-lbc-stack
  since the package only installs the AWS Load Balancer Controller. The
  "base" name was misleading.

  BREAKING CHANGE: XRD kind is now LBCStack (was BaseStack), CRD is
  lbcstacks.aws.hops.ops.com.ai (was basestacks.aws.hops.ops.com.ai),
  package is published as ghcr.io/hops-ops/aws-lbc-stack.

  Existing XRs deployed as kind: BaseStack must be migrated to
  kind: LBCStack and any references to the old CRD/repo updated.


See full diff: [v0.15.0...v1.0.0](https://github.com/hops-ops/aws-lbc-stack/compare/v0.15.0...v1.0.0)
