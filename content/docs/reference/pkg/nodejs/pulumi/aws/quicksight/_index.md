---
title: Module quicksight
---

<!-- WARNING: this page was generated by a tool. Do not edit it by hand. -->
<!-- To change it, please see https://github.com/pulumi/docs/tree/master/tools/tscdocgen. -->

<a href="../">@pulumi/aws</a> &gt; quicksight

> This provider is a derived work of the [Terraform Provider](https://github.com/terraform-providers/terraform-provider-aws)
> distributed under [MPL 2.0](https://www.mozilla.org/en-US/MPL/2.0/). If you encounter a bug or missing feature,
> first check the [`pulumi/pulumi-aws` repo](https://github.com/pulumi/pulumi-aws/issues); however, if that doesn't turn up anything,
> please consult the source [`terraform-providers/terraform-provider-aws` repo](https://github.com/terraform-providers/terraform-provider-aws/issues).



<div class="toggleVisible">
<div class="collapsed">
<h2 class="pdoc-module-header toggleButton" title="Click to show Index">Index ▹</h2>
</div>
<div class="expanded">
<h2 class="pdoc-module-header toggleButton" title="Click to hide Index">Index ▾</h2>
<div class="pdoc-module-contents">
<ul>
<li><a href="#Group">class Group</a></li>
<li><a href="#GroupArgs">interface GroupArgs</a></li>
<li><a href="#GroupState">interface GroupState</a></li>
</ul>

<a href="https://github.com/pulumi/pulumi-aws/blob/6597a59b9b5c887a5484c3c3198182fbd205f368/sdk/nodejs/quicksight/group.ts">quicksight/group.ts</a> 
</div>
</div>
</div>


<h2 class="pdoc-module-header" id="Group">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-aws/blob/6597a59b9b5c887a5484c3c3198182fbd205f368/sdk/nodejs/quicksight/group.ts#L23">class <b>Group</b></a>
</h2>
<div class="pdoc-module-contents">
<pre class="highlight"><span class='kd'>extends</span> <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResource'>CustomResource</a></pre>
{{% md %}}

Resource for managing Quick Sight Group

## Example Usage

```typescript
import * as pulumi from "@pulumi/pulumi";
import * as aws from "@pulumi/aws";

const example = new aws.quicksight.Group("example", {
    groupName: "tf-example",
});
```

> This content is derived from https://github.com/terraform-providers/terraform-provider-aws/blob/master/website/docs/r/quicksight_group.html.markdown.

{{% /md %}}
<h3 class="pdoc-member-header" id="Group-constructor">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/6597a59b9b5c887a5484c3c3198182fbd205f368/sdk/nodejs/quicksight/group.ts#L69"> <b>constructor</b></a>
</h3>
<div class="pdoc-member-contents">
{{% md %}}

<pre class="highlight"><span class='kd'></span><span class='kd'>new</span> Group(name: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>, args: <a href='#GroupArgs'>GroupArgs</a>, opts?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions'>pulumi.CustomResourceOptions</a>)</pre>


Create a Group resource with the given unique name, arguments, and options.

* `name` The _unique_ name of the resource.
* `args` The arguments to use to populate this resource&#39;s properties.
* `opts` A bag of options that control this resource&#39;s behavior.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Group-get">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/6597a59b9b5c887a5484c3c3198182fbd205f368/sdk/nodejs/quicksight/group.ts#L32">method <b>get</b></a>
</h3>
<div class="pdoc-member-contents">
{{% md %}}

<pre class="highlight"><span class='kd'>public static </span>get(name: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>, id: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#ID'>pulumi.ID</a>&gt;, state?: <a href='#GroupState'>GroupState</a>, opts?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions'>pulumi.CustomResourceOptions</a>): <a href='#Group'>Group</a></pre>


Get an existing Group resource's state with the given name, ID, and optional extra
properties used to qualify the lookup.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Group-getProvider">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/6597a59b9b5c887a5484c3c3198182fbd205f368/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L19">method <b>getProvider</b></a>
</h3>
<div class="pdoc-member-contents">
{{% md %}}

<pre class="highlight"><span class='kd'></span>getProvider(moduleMember: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>): ProviderResource | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span></pre>

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Group-isInstance">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/6597a59b9b5c887a5484c3c3198182fbd205f368/sdk/nodejs/quicksight/group.ts#L43">method <b>isInstance</b></a>
</h3>
<div class="pdoc-member-contents">
{{% md %}}

<pre class="highlight"><span class='kd'>public static </span>isInstance(obj: <span class='kd'><a href='https://www.typescriptlang.org/docs/handbook/basic-types.html#any'>any</a></span>): <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean'>boolean</a></span></pre>


Returns true if the given object is an instance of Group.  This is designed to work even
when multiple copies of the Pulumi SDK have been loaded into the same process.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Group-arn">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/6597a59b9b5c887a5484c3c3198182fbd205f368/sdk/nodejs/quicksight/group.ts#L53">property <b>arn</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>arn: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}

Amazon Resource Name (ARN) of group

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Group-awsAccountId">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/6597a59b9b5c887a5484c3c3198182fbd205f368/sdk/nodejs/quicksight/group.ts#L57">property <b>awsAccountId</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>awsAccountId: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}

The ID for the AWS account that the group is in. Currently, you use the ID for the AWS account that contains your Amazon QuickSight account.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Group-description">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/6597a59b9b5c887a5484c3c3198182fbd205f368/sdk/nodejs/quicksight/group.ts#L61">property <b>description</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>description: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span> | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span>&gt;;</pre>
{{% md %}}

A description for the group.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Group-groupName">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/6597a59b9b5c887a5484c3c3198182fbd205f368/sdk/nodejs/quicksight/group.ts#L65">property <b>groupName</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>groupName: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}

A name for the group.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Group-id">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/6597a59b9b5c887a5484c3c3198182fbd205f368/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L212">property <b>id</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>id: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>Output</a>&lt;<a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#ID'>ID</a>&gt;;</pre>
{{% md %}}

id is the provider-assigned unique ID for this managed resource.  It is set during
deployments and may be missing (undefined) during planning phases.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Group-namespace">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/6597a59b9b5c887a5484c3c3198182fbd205f368/sdk/nodejs/quicksight/group.ts#L69">property <b>namespace</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>namespace: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span> | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span>&gt;;</pre>
{{% md %}}

The namespace. Currently, you should set this to `default`.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Group-urn">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/6597a59b9b5c887a5484c3c3198182fbd205f368/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L17">property <b>urn</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>urn: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>Output</a>&lt;<a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#URN'>URN</a>&gt;;</pre>
{{% md %}}

urn is the stable logical URN used to distinctly address a resource, both before and after
deployments.

{{% /md %}}
</div>
</div>
<h2 class="pdoc-module-header" id="GroupArgs">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-aws/blob/6597a59b9b5c887a5484c3c3198182fbd205f368/sdk/nodejs/quicksight/group.ts#L139">interface <b>GroupArgs</b></a>
</h2>
<div class="pdoc-module-contents">
{{% md %}}

The set of arguments for constructing a Group resource.

{{% /md %}}
<h3 class="pdoc-member-header" id="GroupArgs-awsAccountId">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/6597a59b9b5c887a5484c3c3198182fbd205f368/sdk/nodejs/quicksight/group.ts#L143">property <b>awsAccountId</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>awsAccountId?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}

The ID for the AWS account that the group is in. Currently, you use the ID for the AWS account that contains your Amazon QuickSight account.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="GroupArgs-description">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/6597a59b9b5c887a5484c3c3198182fbd205f368/sdk/nodejs/quicksight/group.ts#L147">property <b>description</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>description?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}

A description for the group.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="GroupArgs-groupName">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/6597a59b9b5c887a5484c3c3198182fbd205f368/sdk/nodejs/quicksight/group.ts#L151">property <b>groupName</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>groupName: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}

A name for the group.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="GroupArgs-namespace">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/6597a59b9b5c887a5484c3c3198182fbd205f368/sdk/nodejs/quicksight/group.ts#L155">property <b>namespace</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>namespace?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}

The namespace. Currently, you should set this to `default`.

{{% /md %}}
</div>
</div>
<h2 class="pdoc-module-header" id="GroupState">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-aws/blob/6597a59b9b5c887a5484c3c3198182fbd205f368/sdk/nodejs/quicksight/group.ts#L113">interface <b>GroupState</b></a>
</h2>
<div class="pdoc-module-contents">
{{% md %}}

Input properties used for looking up and filtering Group resources.

{{% /md %}}
<h3 class="pdoc-member-header" id="GroupState-arn">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/6597a59b9b5c887a5484c3c3198182fbd205f368/sdk/nodejs/quicksight/group.ts#L117">property <b>arn</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>arn?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}

Amazon Resource Name (ARN) of group

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="GroupState-awsAccountId">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/6597a59b9b5c887a5484c3c3198182fbd205f368/sdk/nodejs/quicksight/group.ts#L121">property <b>awsAccountId</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>awsAccountId?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}

The ID for the AWS account that the group is in. Currently, you use the ID for the AWS account that contains your Amazon QuickSight account.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="GroupState-description">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/6597a59b9b5c887a5484c3c3198182fbd205f368/sdk/nodejs/quicksight/group.ts#L125">property <b>description</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>description?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}

A description for the group.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="GroupState-groupName">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/6597a59b9b5c887a5484c3c3198182fbd205f368/sdk/nodejs/quicksight/group.ts#L129">property <b>groupName</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>groupName?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}

A name for the group.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="GroupState-namespace">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/6597a59b9b5c887a5484c3c3198182fbd205f368/sdk/nodejs/quicksight/group.ts#L133">property <b>namespace</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>namespace?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}

The namespace. Currently, you should set this to `default`.

{{% /md %}}
</div>
</div>
