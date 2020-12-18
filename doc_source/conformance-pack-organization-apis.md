# Managing Conformance Packs Across all Accounts in Your Organization<a name="conformance-pack-organization-apis"></a>

Use AWS Config to manage conformance packs across all AWS accounts within an organization\. You can do the following:
+ Centrally deploy, update, and delete conformance packs across member accounts in an organization in AWS Organizations\.
+ Deploy a common set of AWS Config rules and remediation actions across all accounts and specify accounts where AWS Config rules and remediation actions should not be created\.
+ Use the APIs from the master account in AWS Organizations to enforce governance by ensuring that the underlying AWS Config rules and remediation actions are not modifiable by your organization’s member accounts\.

Ensure AWS Config recording is on before you use the following APIs to manage conformance pack rules across all AWS accounts within an organization:
+ [DeleteOrganizationConformancePack](https://docs.aws.amazon.com/config/latest/APIReference/API_DeleteOrganizationConformancePack.html), deletes the specified organization conformance pack and all of the config rules and remediation actions from all member accounts in that organization\.
+ [DescribeOrganizationConformancePacks](https://docs.aws.amazon.com/config/latest/APIReference/API_DescribeOrganizationConformancePacks.html), returns a list of organization conformance packs\.
+ [DescribeOrganizationConformancePackStatuses](https://docs.aws.amazon.com/config/latest/APIReference/API_DescribeOrganizationConformancePackStatuses.html), provides organization conformance pack deployment status for an organization\.
+ [GetOrganizationConformancePackDetailedStatus](https://docs.aws.amazon.com/config/latest/APIReference/API_GetOrganizationConformancePackDetailedStatus.html), returns detailed status for each member account within an organization for a given organization conformance pack\.
+ [PutOrganizationConformancePack](https://docs.aws.amazon.com/config/latest/APIReference/API_PutOrganizationConformancePack.html), deploys conformance packs across member accounts in an AWS Organization\.