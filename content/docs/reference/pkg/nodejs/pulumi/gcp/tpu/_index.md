---
title: Module tpu
---

<!-- WARNING: this page was generated by a tool. Do not edit it by hand. -->
<!-- To change it, please see https://github.com/pulumi/docs/tree/master/tools/tscdocgen. -->

<a href="../">@pulumi/gcp</a> &gt; tpu

> This provider is a derived work of the [Terraform Provider](https://github.com/terraform-providers/terraform-provider-google)
> distributed under [MPL 2.0](https://www.mozilla.org/en-US/MPL/2.0/). If you encounter a bug or missing feature,
> first check the [`pulumi/pulumi-gcp` repo](https://github.com/pulumi/pulumi-gcp/issues); however, if that doesn't turn up anything,
> please consult the source [`terraform-providers/terraform-provider-google` repo](https://github.com/terraform-providers/terraform-provider-google/issues).



<div class="toggleVisible">
<div class="collapsed">
<h2 class="pdoc-module-header toggleButton" title="Click to show Index">Index ▹</h2>
</div>
<div class="expanded">
<h2 class="pdoc-module-header toggleButton" title="Click to hide Index">Index ▾</h2>
<div class="pdoc-module-contents">
<ul>
<li><a href="#Node">class Node</a></li>
<li><a href="#getTensorflowVersions">function getTensorflowVersions</a></li>
<li><a href="#GetTensorflowVersionsArgs">interface GetTensorflowVersionsArgs</a></li>
<li><a href="#GetTensorflowVersionsResult">interface GetTensorflowVersionsResult</a></li>
<li><a href="#NodeArgs">interface NodeArgs</a></li>
<li><a href="#NodeState">interface NodeState</a></li>
</ul>

<a href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/tpu/getTensorflowVersions.ts">tpu/getTensorflowVersions.ts</a> <a href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/tpu/node.ts">tpu/node.ts</a> 
</div>
</div>
</div>


<h2 class="pdoc-module-header" id="Node">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/tpu/node.ts#L58">class <b>Node</b></a>
</h2>
<div class="pdoc-module-contents">
<pre class="highlight"><span class='kd'>extends</span> <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResource'>CustomResource</a></pre>
{{% md %}}

A Cloud TPU instance.

To get more information about Node, see:

* [API documentation](https://cloud.google.com/tpu/docs/reference/rest/)
* How-to Guides
    * [Official Documentation](https://cloud.google.com/tpu/docs/)

## Example Usage - Tpu Node Basic


```typescript
import * as pulumi from "@pulumi/pulumi";
import * as gcp from "@pulumi/gcp";

const available = pulumi.output(gcp.tpu.getTensorflowVersions({}));
const tpu = new gcp.tpu.Node("tpu", {
    acceleratorType: "v3-8",
    cidrBlock: "10.2.0.0/29",
    tensorflowVersion: available.apply(available => available.versions[0]),
    zone: "us-central1-b",
});
```
## Example Usage - Tpu Node Full


```typescript
import * as pulumi from "@pulumi/pulumi";
import * as gcp from "@pulumi/gcp";

const available = pulumi.output(gcp.tpu.getTensorflowVersions({}));
const tpu = new gcp.tpu.Node("tpu", {
    acceleratorType: "v3-8",
    cidrBlock: "10.3.0.0/29",
    description: "Google Provider test TPU",
    labels: {
        foo: "bar",
    },
    network: "default",
    schedulingConfig: {
        preemptible: true,
    },
    tensorflowVersion: available.apply(available => available.versions[0]),
    zone: "us-central1-b",
});
```

> This content is derived from https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/tpu_node.html.markdown.

{{% /md %}}
<h3 class="pdoc-member-header" id="Node-constructor">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/tpu/node.ts#L100"> <b>constructor</b></a>
</h3>
<div class="pdoc-member-contents">
{{% md %}}

<pre class="highlight"><span class='kd'></span><span class='kd'>new</span> Node(name: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>, args: <a href='#NodeArgs'>NodeArgs</a>, opts?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions'>pulumi.CustomResourceOptions</a>)</pre>


Create a Node resource with the given unique name, arguments, and options.

* `name` The _unique_ name of the resource.
* `args` The arguments to use to populate this resource&#39;s properties.
* `opts` A bag of options that control this resource&#39;s behavior.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Node-get">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/tpu/node.ts#L67">method <b>get</b></a>
</h3>
<div class="pdoc-member-contents">
{{% md %}}

<pre class="highlight"><span class='kd'>public static </span>get(name: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>, id: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#ID'>pulumi.ID</a>&gt;, state?: <a href='#NodeState'>NodeState</a>, opts?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions'>pulumi.CustomResourceOptions</a>): <a href='#Node'>Node</a></pre>


Get an existing Node resource's state with the given name, ID, and optional extra
properties used to qualify the lookup.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Node-getProvider">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L19">method <b>getProvider</b></a>
</h3>
<div class="pdoc-member-contents">
{{% md %}}

<pre class="highlight"><span class='kd'></span>getProvider(moduleMember: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>): ProviderResource | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span></pre>

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Node-isInstance">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/tpu/node.ts#L78">method <b>isInstance</b></a>
</h3>
<div class="pdoc-member-contents">
{{% md %}}

<pre class="highlight"><span class='kd'>public static </span>isInstance(obj: <span class='kd'><a href='https://www.typescriptlang.org/docs/handbook/basic-types.html#any'>any</a></span>): <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean'>boolean</a></span></pre>


Returns true if the given object is an instance of Node.  This is designed to work even
when multiple copies of the Pulumi SDK have been loaded into the same process.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Node-acceleratorType">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/tpu/node.ts#L85">property <b>acceleratorType</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>acceleratorType: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Node-cidrBlock">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/tpu/node.ts#L86">property <b>cidrBlock</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>cidrBlock: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Node-description">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/tpu/node.ts#L87">property <b>description</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>description: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span> | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Node-id">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L212">property <b>id</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>id: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>Output</a>&lt;<a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#ID'>ID</a>&gt;;</pre>
{{% md %}}

id is the provider-assigned unique ID for this managed resource.  It is set during
deployments and may be missing (undefined) during planning phases.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Node-labels">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/tpu/node.ts#L88">property <b>labels</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>labels: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;{[key: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>]: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>} | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Node-name">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/tpu/node.ts#L89">property <b>name</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>name: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Node-network">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/tpu/node.ts#L90">property <b>network</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>network: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Node-networkEndpoints">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/tpu/node.ts#L91">property <b>networkEndpoints</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>networkEndpoints: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;{
    ipAddress: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>;
    port: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number'>number</a></span>;
}[]&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Node-project">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/tpu/node.ts#L96">property <b>project</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>project: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}

The ID of the project in which the resource belongs.
If it is not provided, the provider project is used.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Node-schedulingConfig">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/tpu/node.ts#L97">property <b>schedulingConfig</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>schedulingConfig: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;{
    preemptible: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span> | <span class='kd'>false</span> | <span class='kd'>true</span>;
} | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Node-serviceAccount">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/tpu/node.ts#L98">property <b>serviceAccount</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>serviceAccount: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Node-tensorflowVersion">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/tpu/node.ts#L99">property <b>tensorflowVersion</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>tensorflowVersion: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Node-urn">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L17">property <b>urn</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>urn: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>Output</a>&lt;<a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#URN'>URN</a>&gt;;</pre>
{{% md %}}

urn is the stable logical URN used to distinctly address a resource, both before and after
deployments.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Node-zone">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/tpu/node.ts#L100">property <b>zone</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>zone: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
</div>
<h2 class="pdoc-module-header" id="getTensorflowVersions">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/tpu/getTensorflowVersions.ts#L7">function <b>getTensorflowVersions</b></a>
</h2>
<div class="pdoc-module-contents">
{{% md %}}

<pre class="highlight"><span class='kd'></span>getTensorflowVersions(args?: <a href='#GetTensorflowVersionsArgs'>GetTensorflowVersionsArgs</a>, opts?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#InvokeOptions'>pulumi.InvokeOptions</a>): <a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise'>Promise</a>&lt;<a href='#GetTensorflowVersionsResult'>GetTensorflowVersionsResult</a>&gt; &amp; <a href='#GetTensorflowVersionsResult'>GetTensorflowVersionsResult</a></pre>

{{% /md %}}
</div>
<h2 class="pdoc-module-header" id="GetTensorflowVersionsArgs">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/tpu/getTensorflowVersions.ts#L27">interface <b>GetTensorflowVersionsArgs</b></a>
</h2>
<div class="pdoc-module-contents">
{{% md %}}

A collection of arguments for invoking getTensorflowVersions.

{{% /md %}}
<h3 class="pdoc-member-header" id="GetTensorflowVersionsArgs-project">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/tpu/getTensorflowVersions.ts#L28">property <b>project</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>project?: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span> | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="GetTensorflowVersionsArgs-zone">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/tpu/getTensorflowVersions.ts#L29">property <b>zone</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>zone?: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span> | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>;</pre>
{{% md %}}
{{% /md %}}
</div>
</div>
<h2 class="pdoc-module-header" id="GetTensorflowVersionsResult">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/tpu/getTensorflowVersions.ts#L35">interface <b>GetTensorflowVersionsResult</b></a>
</h2>
<div class="pdoc-module-contents">
{{% md %}}

A collection of values returned by getTensorflowVersions.

{{% /md %}}
<h3 class="pdoc-member-header" id="GetTensorflowVersionsResult-id">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/tpu/getTensorflowVersions.ts#L42">property <b>id</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>id: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>;</pre>
{{% md %}}

id is the provider-assigned unique ID for this managed resource.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="GetTensorflowVersionsResult-project">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/tpu/getTensorflowVersions.ts#L36">property <b>project</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>project: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="GetTensorflowVersionsResult-versions">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/tpu/getTensorflowVersions.ts#L37">property <b>versions</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>versions: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>[];</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="GetTensorflowVersionsResult-zone">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/tpu/getTensorflowVersions.ts#L38">property <b>zone</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>zone: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>;</pre>
{{% md %}}
{{% /md %}}
</div>
</div>
<h2 class="pdoc-module-header" id="NodeArgs">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/tpu/node.ts#L189">interface <b>NodeArgs</b></a>
</h2>
<div class="pdoc-module-contents">
{{% md %}}

The set of arguments for constructing a Node resource.

{{% /md %}}
<h3 class="pdoc-member-header" id="NodeArgs-acceleratorType">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/tpu/node.ts#L190">property <b>acceleratorType</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>acceleratorType: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="NodeArgs-cidrBlock">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/tpu/node.ts#L191">property <b>cidrBlock</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>cidrBlock: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="NodeArgs-description">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/tpu/node.ts#L192">property <b>description</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>description?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="NodeArgs-labels">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/tpu/node.ts#L193">property <b>labels</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>labels?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;{[key: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>]: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;}&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="NodeArgs-name">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/tpu/node.ts#L194">property <b>name</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>name?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="NodeArgs-network">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/tpu/node.ts#L195">property <b>network</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>network?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="NodeArgs-project">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/tpu/node.ts#L200">property <b>project</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>project?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}

The ID of the project in which the resource belongs.
If it is not provided, the provider project is used.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="NodeArgs-schedulingConfig">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/tpu/node.ts#L201">property <b>schedulingConfig</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>schedulingConfig?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;{
    preemptible: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean'>boolean</a></span>&gt;;
}&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="NodeArgs-tensorflowVersion">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/tpu/node.ts#L202">property <b>tensorflowVersion</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>tensorflowVersion: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="NodeArgs-zone">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/tpu/node.ts#L203">property <b>zone</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>zone: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
</div>
<h2 class="pdoc-module-header" id="NodeState">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/tpu/node.ts#L167">interface <b>NodeState</b></a>
</h2>
<div class="pdoc-module-contents">
{{% md %}}

Input properties used for looking up and filtering Node resources.

{{% /md %}}
<h3 class="pdoc-member-header" id="NodeState-acceleratorType">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/tpu/node.ts#L168">property <b>acceleratorType</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>acceleratorType?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="NodeState-cidrBlock">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/tpu/node.ts#L169">property <b>cidrBlock</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>cidrBlock?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="NodeState-description">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/tpu/node.ts#L170">property <b>description</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>description?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="NodeState-labels">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/tpu/node.ts#L171">property <b>labels</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>labels?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;{[key: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>]: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;}&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="NodeState-name">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/tpu/node.ts#L172">property <b>name</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>name?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="NodeState-network">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/tpu/node.ts#L173">property <b>network</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>network?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="NodeState-networkEndpoints">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/tpu/node.ts#L174">property <b>networkEndpoints</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>networkEndpoints?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;{
    ipAddress: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;
    port: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number'>number</a></span>&gt;;
}&gt;[]&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="NodeState-project">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/tpu/node.ts#L179">property <b>project</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>project?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}

The ID of the project in which the resource belongs.
If it is not provided, the provider project is used.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="NodeState-schedulingConfig">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/tpu/node.ts#L180">property <b>schedulingConfig</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>schedulingConfig?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;{
    preemptible: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean'>boolean</a></span>&gt;;
}&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="NodeState-serviceAccount">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/tpu/node.ts#L181">property <b>serviceAccount</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>serviceAccount?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="NodeState-tensorflowVersion">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/tpu/node.ts#L182">property <b>tensorflowVersion</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>tensorflowVersion?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="NodeState-zone">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/tpu/node.ts#L183">property <b>zone</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>zone?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
</div>
