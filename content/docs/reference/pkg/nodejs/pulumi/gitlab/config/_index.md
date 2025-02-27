---
title: Module config
---

<!-- WARNING: this page was generated by a tool. Do not edit it by hand. -->
<!-- To change it, please see https://github.com/pulumi/docs/tree/master/tools/tscdocgen. -->

<a href="../">@pulumi/gitlab</a> &gt; config

> This provider is a derived work of the [Terraform Provider](https://github.com/terraform-providers/terraform-provider-gitlab)
> distributed under [MPL 2.0](https://www.mozilla.org/en-US/MPL/2.0/). If you encounter a bug or missing feature,
> first check the [`pulumi/pulumi-gitlab` repo](https://github.com/pulumi/pulumi-gitlab/issues); however, if that doesn't turn up anything,
> please consult the source [`terraform-providers/terraform-provider-gitlab` repo](https://github.com/terraform-providers/terraform-provider-gitlab/issues).



<div class="toggleVisible">
<div class="collapsed">
<h2 class="pdoc-module-header toggleButton" title="Click to show Index">Index ▹</h2>
</div>
<div class="expanded">
<h2 class="pdoc-module-header toggleButton" title="Click to hide Index">Index ▾</h2>
<div class="pdoc-module-contents">
<ul>
<li><a href="#baseUrl">let baseUrl</a></li>
<li><a href="#cacertFile">let cacertFile</a></li>
<li><a href="#insecure">let insecure</a></li>
<li><a href="#token">let token</a></li>
</ul>

<a href="https://github.com/pulumi/pulumi-gitlab/blob/9557a766cfcc264c3060681e3516c505d8b125a7/sdk/nodejs/config/vars.ts">config/vars.ts</a> 
</div>
</div>
</div>


<h2 class="pdoc-module-header" id="baseUrl">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-gitlab/blob/9557a766cfcc264c3060681e3516c505d8b125a7/sdk/nodejs/config/vars.ts#L12">let <b>baseUrl</b></a>
</h2>
<div class="pdoc-module-contents">
<pre class="highlight"><span class='kd'>let</span> baseUrl: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span> | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span> = <span class='s2'> __config.get(&#34;baseUrl&#34;) || utilities.getEnv(&#34;GITLAB_BASE_URL&#34;)</span>;</pre>
{{% md %}}

The GitLab Base API URL

{{% /md %}}
</div>
<h2 class="pdoc-module-header" id="cacertFile">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-gitlab/blob/9557a766cfcc264c3060681e3516c505d8b125a7/sdk/nodejs/config/vars.ts#L16">let <b>cacertFile</b></a>
</h2>
<div class="pdoc-module-contents">
<pre class="highlight"><span class='kd'>let</span> cacertFile: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span> | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span> = <span class='s2'> __config.get(&#34;cacertFile&#34;)</span>;</pre>
{{% md %}}

A file containing the ca certificate to use in case ssl certificate is not from a standard chain

{{% /md %}}
</div>
<h2 class="pdoc-module-header" id="insecure">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-gitlab/blob/9557a766cfcc264c3060681e3516c505d8b125a7/sdk/nodejs/config/vars.ts#L20">let <b>insecure</b></a>
</h2>
<div class="pdoc-module-contents">
<pre class="highlight"><span class='kd'>let</span> insecure: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean'>boolean</a></span> | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span> = <span class='s2'> __config.getObject&lt;boolean&gt;(&#34;insecure&#34;)</span>;</pre>
{{% md %}}

Disable SSL verification of API calls

{{% /md %}}
</div>
<h2 class="pdoc-module-header" id="token">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-gitlab/blob/9557a766cfcc264c3060681e3516c505d8b125a7/sdk/nodejs/config/vars.ts#L24">let <b>token</b></a>
</h2>
<div class="pdoc-module-contents">
<pre class="highlight"><span class='kd'>let</span> token: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span> | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span> = <span class='s2'> __config.get(&#34;token&#34;) || utilities.getEnv(&#34;GITLAB_TOKEN&#34;)</span>;</pre>
{{% md %}}

The OAuth token used to connect to GitLab.

{{% /md %}}
</div>
