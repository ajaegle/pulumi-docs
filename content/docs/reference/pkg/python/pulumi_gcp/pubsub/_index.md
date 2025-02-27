---
title: Module pubsub
---

<div class="section" id="pubsub">
<h1>pubsub<a class="headerlink" href="#pubsub" title="Permalink to this headline">¶</a></h1>
<blockquote>
<div>This provider is a derived work of the <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-google">Terraform Provider</a> distributed under
<a class="reference external" href="https://www.mozilla.org/en-US/MPL/2.0/">MPL 2.0</a>. If you encounter a bug or missing feature, first check the
<a class="reference external" href="https://github.com/pulumi/pulumi-gcp/issues">pulumi/pulumi-gcp repo</a>; however, if that doesn’t turn up
anything, please consult the source <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-google/issues">terraform-providers/terraform-provider-google repo</a>.</div></blockquote>
<span class="target" id="module-pulumi_gcp.pubsub"></span><dl class="class">
<dt id="pulumi_gcp.pubsub.Subscription">
<em class="property">class </em><code class="descclassname">pulumi_gcp.pubsub.</code><code class="descname">Subscription</code><span class="sig-paren">(</span><em>resource_name</em>, <em>opts=None</em>, <em>ack_deadline_seconds=None</em>, <em>expiration_policy=None</em>, <em>labels=None</em>, <em>message_retention_duration=None</em>, <em>name=None</em>, <em>project=None</em>, <em>push_config=None</em>, <em>retain_acked_messages=None</em>, <em>topic=None</em>, <em>__props__=None</em>, <em>__name__=None</em>, <em>__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.pubsub.Subscription" title="Permalink to this definition">¶</a></dt>
<dd><p>A named resource representing the stream of messages from a single,
specific topic, to be delivered to the subscribing application.</p>
<p>To get more information about Subscription, see:</p>
<ul class="simple">
<li><a class="reference external" href="https://cloud.google.com/pubsub/docs/reference/rest/v1/projects.subscriptions">API documentation</a></li>
<li>How-to Guides<ul>
<li><a class="reference external" href="https://cloud.google.com/pubsub/docs/admin#managing_subscriptions">Managing Subscriptions</a></li>
</ul>
</li>
</ul>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><ul class="first last simple">
<li><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</li>
<li><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</li>
<li><strong>project</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The ID of the project in which the resource belongs.
If it is not provided, the provider project is used.</li>
</ul>
</td>
</tr>
</tbody>
</table>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/pubsub_subscription.html.markdown">https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/pubsub_subscription.html.markdown</a>.</div></blockquote>
<dl class="attribute">
<dt id="pulumi_gcp.pubsub.Subscription.project">
<code class="descname">project</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.pubsub.Subscription.project" title="Permalink to this definition">¶</a></dt>
<dd><p>The ID of the project in which the resource belongs.
If it is not provided, the provider project is used.</p>
</dd></dl>

<dl class="staticmethod">
<dt id="pulumi_gcp.pubsub.Subscription.get">
<em class="property">static </em><code class="descname">get</code><span class="sig-paren">(</span><em>resource_name</em>, <em>id</em>, <em>opts=None</em>, <em>ack_deadline_seconds=None</em>, <em>expiration_policy=None</em>, <em>labels=None</em>, <em>message_retention_duration=None</em>, <em>name=None</em>, <em>path=None</em>, <em>project=None</em>, <em>push_config=None</em>, <em>retain_acked_messages=None</em>, <em>topic=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.pubsub.Subscription.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing Subscription resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.
:param str resource_name: The unique name of the resulting resource.
:param str id: The unique provider ID of the resource to lookup.
:param pulumi.ResourceOptions opts: Options for the resource.
:param pulumi.Input[str] project: The ID of the project in which the resource belongs.</p>
<blockquote>
<div>If it is not provided, the provider project is used.</div></blockquote>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/pubsub_subscription.html.markdown">https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/pubsub_subscription.html.markdown</a>.</div></blockquote>
</dd></dl>

<dl class="method">
<dt id="pulumi_gcp.pubsub.Subscription.translate_output_property">
<code class="descname">translate_output_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.pubsub.Subscription.translate_output_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of output properties
into a format of their choosing before writing those properties to the resource object.</p>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><strong>prop</strong> (<em>str</em>) – A property name.</td>
</tr>
<tr class="field-even field"><th class="field-name">Returns:</th><td class="field-body">A potentially transformed property name.</td>
</tr>
<tr class="field-odd field"><th class="field-name">Return type:</th><td class="field-body">str</td>
</tr>
</tbody>
</table>
</dd></dl>

<dl class="method">
<dt id="pulumi_gcp.pubsub.Subscription.translate_input_property">
<code class="descname">translate_input_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.pubsub.Subscription.translate_input_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of input properties into
a format of their choosing before sending those properties to the Pulumi engine.</p>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><strong>prop</strong> (<em>str</em>) – A property name.</td>
</tr>
<tr class="field-even field"><th class="field-name">Returns:</th><td class="field-body">A potentially transformed property name.</td>
</tr>
<tr class="field-odd field"><th class="field-name">Return type:</th><td class="field-body">str</td>
</tr>
</tbody>
</table>
</dd></dl>

</dd></dl>

<dl class="class">
<dt id="pulumi_gcp.pubsub.SubscriptionIAMBinding">
<em class="property">class </em><code class="descclassname">pulumi_gcp.pubsub.</code><code class="descname">SubscriptionIAMBinding</code><span class="sig-paren">(</span><em>resource_name</em>, <em>opts=None</em>, <em>members=None</em>, <em>project=None</em>, <em>role=None</em>, <em>subscription=None</em>, <em>__props__=None</em>, <em>__name__=None</em>, <em>__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.pubsub.SubscriptionIAMBinding" title="Permalink to this definition">¶</a></dt>
<dd><p>Three different resources help you manage your IAM policy for pubsub subscription. Each of these resources serves a different use case:</p>
<ul class="simple">
<li><code class="docutils literal notranslate"><span class="pre">pubsub.SubscriptionIAMPolicy</span></code>: Authoritative. Sets the IAM policy for the subscription and replaces any existing policy already attached.</li>
<li><code class="docutils literal notranslate"><span class="pre">pubsub.SubscriptionIAMBinding</span></code>: Authoritative for a given role. Updates the IAM policy to grant a role to a list of members. Other roles within the IAM policy for the subscription are preserved.</li>
<li><code class="docutils literal notranslate"><span class="pre">pubsub.SubscriptionIAMMember</span></code>: Non-authoritative. Updates the IAM policy to grant a role to a new member. Other members for the role for the subscription are preserved.</li>
</ul>
<blockquote>
<div><p><strong>Note:</strong> <code class="docutils literal notranslate"><span class="pre">pubsub.SubscriptionIAMPolicy</span></code> <strong>cannot</strong> be used in conjunction with <code class="docutils literal notranslate"><span class="pre">pubsub.SubscriptionIAMBinding</span></code> and <code class="docutils literal notranslate"><span class="pre">pubsub.SubscriptionIAMMember</span></code> or they will fight over what your policy should be.</p>
<p><strong>Note:</strong> <code class="docutils literal notranslate"><span class="pre">pubsub.SubscriptionIAMBinding</span></code> resources <strong>can be</strong> used in conjunction with <code class="docutils literal notranslate"><span class="pre">pubsub.SubscriptionIAMMember</span></code> resources <strong>only if</strong> they do not grant privilege to the same role.</p>
</div></blockquote>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><ul class="first last simple">
<li><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</li>
<li><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</li>
<li><strong>project</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The project in which the resource belongs. If it
is not provided, the provider project is used.</li>
<li><strong>role</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The role that should be applied. Only one
<code class="docutils literal notranslate"><span class="pre">pubsub.SubscriptionIAMBinding</span></code> can be used per role. Note that custom roles must be of the format
<code class="docutils literal notranslate"><span class="pre">[projects|organizations]/{parent-name}/roles/{role-name}</span></code>.</li>
<li><strong>subscription</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The subscription name or id to bind to attach IAM policy to.</li>
</ul>
</td>
</tr>
</tbody>
</table>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/pubsub_subscription_iam_binding.html.markdown">https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/pubsub_subscription_iam_binding.html.markdown</a>.</div></blockquote>
<dl class="attribute">
<dt id="pulumi_gcp.pubsub.SubscriptionIAMBinding.etag">
<code class="descname">etag</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.pubsub.SubscriptionIAMBinding.etag" title="Permalink to this definition">¶</a></dt>
<dd><p>(Computed) The etag of the subscription’s IAM policy.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_gcp.pubsub.SubscriptionIAMBinding.project">
<code class="descname">project</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.pubsub.SubscriptionIAMBinding.project" title="Permalink to this definition">¶</a></dt>
<dd><p>The project in which the resource belongs. If it
is not provided, the provider project is used.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_gcp.pubsub.SubscriptionIAMBinding.role">
<code class="descname">role</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.pubsub.SubscriptionIAMBinding.role" title="Permalink to this definition">¶</a></dt>
<dd><p>The role that should be applied. Only one
<code class="docutils literal notranslate"><span class="pre">pubsub.SubscriptionIAMBinding</span></code> can be used per role. Note that custom roles must be of the format
<code class="docutils literal notranslate"><span class="pre">[projects|organizations]/{parent-name}/roles/{role-name}</span></code>.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_gcp.pubsub.SubscriptionIAMBinding.subscription">
<code class="descname">subscription</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.pubsub.SubscriptionIAMBinding.subscription" title="Permalink to this definition">¶</a></dt>
<dd><p>The subscription name or id to bind to attach IAM policy to.</p>
</dd></dl>

<dl class="staticmethod">
<dt id="pulumi_gcp.pubsub.SubscriptionIAMBinding.get">
<em class="property">static </em><code class="descname">get</code><span class="sig-paren">(</span><em>resource_name</em>, <em>id</em>, <em>opts=None</em>, <em>etag=None</em>, <em>members=None</em>, <em>project=None</em>, <em>role=None</em>, <em>subscription=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.pubsub.SubscriptionIAMBinding.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing SubscriptionIAMBinding resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.
:param str resource_name: The unique name of the resulting resource.
:param str id: The unique provider ID of the resource to lookup.
:param pulumi.ResourceOptions opts: Options for the resource.
:param pulumi.Input[str] etag: (Computed) The etag of the subscription’s IAM policy.
:param pulumi.Input[str] project: The project in which the resource belongs. If it</p>
<blockquote>
<div>is not provided, the provider project is used.</div></blockquote>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><ul class="first last simple">
<li><strong>role</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The role that should be applied. Only one
<code class="docutils literal notranslate"><span class="pre">pubsub.SubscriptionIAMBinding</span></code> can be used per role. Note that custom roles must be of the format
<code class="docutils literal notranslate"><span class="pre">[projects|organizations]/{parent-name}/roles/{role-name}</span></code>.</li>
<li><strong>subscription</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The subscription name or id to bind to attach IAM policy to.</li>
</ul>
</td>
</tr>
</tbody>
</table>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/pubsub_subscription_iam_binding.html.markdown">https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/pubsub_subscription_iam_binding.html.markdown</a>.</div></blockquote>
</dd></dl>

<dl class="method">
<dt id="pulumi_gcp.pubsub.SubscriptionIAMBinding.translate_output_property">
<code class="descname">translate_output_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.pubsub.SubscriptionIAMBinding.translate_output_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of output properties
into a format of their choosing before writing those properties to the resource object.</p>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><strong>prop</strong> (<em>str</em>) – A property name.</td>
</tr>
<tr class="field-even field"><th class="field-name">Returns:</th><td class="field-body">A potentially transformed property name.</td>
</tr>
<tr class="field-odd field"><th class="field-name">Return type:</th><td class="field-body">str</td>
</tr>
</tbody>
</table>
</dd></dl>

<dl class="method">
<dt id="pulumi_gcp.pubsub.SubscriptionIAMBinding.translate_input_property">
<code class="descname">translate_input_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.pubsub.SubscriptionIAMBinding.translate_input_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of input properties into
a format of their choosing before sending those properties to the Pulumi engine.</p>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><strong>prop</strong> (<em>str</em>) – A property name.</td>
</tr>
<tr class="field-even field"><th class="field-name">Returns:</th><td class="field-body">A potentially transformed property name.</td>
</tr>
<tr class="field-odd field"><th class="field-name">Return type:</th><td class="field-body">str</td>
</tr>
</tbody>
</table>
</dd></dl>

</dd></dl>

<dl class="class">
<dt id="pulumi_gcp.pubsub.SubscriptionIAMMember">
<em class="property">class </em><code class="descclassname">pulumi_gcp.pubsub.</code><code class="descname">SubscriptionIAMMember</code><span class="sig-paren">(</span><em>resource_name</em>, <em>opts=None</em>, <em>member=None</em>, <em>project=None</em>, <em>role=None</em>, <em>subscription=None</em>, <em>__props__=None</em>, <em>__name__=None</em>, <em>__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.pubsub.SubscriptionIAMMember" title="Permalink to this definition">¶</a></dt>
<dd><p>Three different resources help you manage your IAM policy for pubsub subscription. Each of these resources serves a different use case:</p>
<ul class="simple">
<li><code class="docutils literal notranslate"><span class="pre">pubsub.SubscriptionIAMPolicy</span></code>: Authoritative. Sets the IAM policy for the subscription and replaces any existing policy already attached.</li>
<li><code class="docutils literal notranslate"><span class="pre">pubsub.SubscriptionIAMBinding</span></code>: Authoritative for a given role. Updates the IAM policy to grant a role to a list of members. Other roles within the IAM policy for the subscription are preserved.</li>
<li><code class="docutils literal notranslate"><span class="pre">pubsub.SubscriptionIAMMember</span></code>: Non-authoritative. Updates the IAM policy to grant a role to a new member. Other members for the role for the subscription are preserved.</li>
</ul>
<blockquote>
<div><p><strong>Note:</strong> <code class="docutils literal notranslate"><span class="pre">pubsub.SubscriptionIAMPolicy</span></code> <strong>cannot</strong> be used in conjunction with <code class="docutils literal notranslate"><span class="pre">pubsub.SubscriptionIAMBinding</span></code> and <code class="docutils literal notranslate"><span class="pre">pubsub.SubscriptionIAMMember</span></code> or they will fight over what your policy should be.</p>
<p><strong>Note:</strong> <code class="docutils literal notranslate"><span class="pre">pubsub.SubscriptionIAMBinding</span></code> resources <strong>can be</strong> used in conjunction with <code class="docutils literal notranslate"><span class="pre">pubsub.SubscriptionIAMMember</span></code> resources <strong>only if</strong> they do not grant privilege to the same role.</p>
</div></blockquote>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><ul class="first last simple">
<li><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</li>
<li><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</li>
<li><strong>project</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The project in which the resource belongs. If it
is not provided, the provider project is used.</li>
<li><strong>role</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The role that should be applied. Only one
<code class="docutils literal notranslate"><span class="pre">pubsub.SubscriptionIAMBinding</span></code> can be used per role. Note that custom roles must be of the format
<code class="docutils literal notranslate"><span class="pre">[projects|organizations]/{parent-name}/roles/{role-name}</span></code>.</li>
<li><strong>subscription</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The subscription name or id to bind to attach IAM policy to.</li>
</ul>
</td>
</tr>
</tbody>
</table>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/pubsub_subscription_iam_member.html.markdown">https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/pubsub_subscription_iam_member.html.markdown</a>.</div></blockquote>
<dl class="attribute">
<dt id="pulumi_gcp.pubsub.SubscriptionIAMMember.etag">
<code class="descname">etag</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.pubsub.SubscriptionIAMMember.etag" title="Permalink to this definition">¶</a></dt>
<dd><p>(Computed) The etag of the subscription’s IAM policy.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_gcp.pubsub.SubscriptionIAMMember.project">
<code class="descname">project</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.pubsub.SubscriptionIAMMember.project" title="Permalink to this definition">¶</a></dt>
<dd><p>The project in which the resource belongs. If it
is not provided, the provider project is used.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_gcp.pubsub.SubscriptionIAMMember.role">
<code class="descname">role</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.pubsub.SubscriptionIAMMember.role" title="Permalink to this definition">¶</a></dt>
<dd><p>The role that should be applied. Only one
<code class="docutils literal notranslate"><span class="pre">pubsub.SubscriptionIAMBinding</span></code> can be used per role. Note that custom roles must be of the format
<code class="docutils literal notranslate"><span class="pre">[projects|organizations]/{parent-name}/roles/{role-name}</span></code>.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_gcp.pubsub.SubscriptionIAMMember.subscription">
<code class="descname">subscription</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.pubsub.SubscriptionIAMMember.subscription" title="Permalink to this definition">¶</a></dt>
<dd><p>The subscription name or id to bind to attach IAM policy to.</p>
</dd></dl>

<dl class="staticmethod">
<dt id="pulumi_gcp.pubsub.SubscriptionIAMMember.get">
<em class="property">static </em><code class="descname">get</code><span class="sig-paren">(</span><em>resource_name</em>, <em>id</em>, <em>opts=None</em>, <em>etag=None</em>, <em>member=None</em>, <em>project=None</em>, <em>role=None</em>, <em>subscription=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.pubsub.SubscriptionIAMMember.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing SubscriptionIAMMember resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.
:param str resource_name: The unique name of the resulting resource.
:param str id: The unique provider ID of the resource to lookup.
:param pulumi.ResourceOptions opts: Options for the resource.
:param pulumi.Input[str] etag: (Computed) The etag of the subscription’s IAM policy.
:param pulumi.Input[str] project: The project in which the resource belongs. If it</p>
<blockquote>
<div>is not provided, the provider project is used.</div></blockquote>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><ul class="first last simple">
<li><strong>role</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The role that should be applied. Only one
<code class="docutils literal notranslate"><span class="pre">pubsub.SubscriptionIAMBinding</span></code> can be used per role. Note that custom roles must be of the format
<code class="docutils literal notranslate"><span class="pre">[projects|organizations]/{parent-name}/roles/{role-name}</span></code>.</li>
<li><strong>subscription</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The subscription name or id to bind to attach IAM policy to.</li>
</ul>
</td>
</tr>
</tbody>
</table>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/pubsub_subscription_iam_member.html.markdown">https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/pubsub_subscription_iam_member.html.markdown</a>.</div></blockquote>
</dd></dl>

<dl class="method">
<dt id="pulumi_gcp.pubsub.SubscriptionIAMMember.translate_output_property">
<code class="descname">translate_output_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.pubsub.SubscriptionIAMMember.translate_output_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of output properties
into a format of their choosing before writing those properties to the resource object.</p>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><strong>prop</strong> (<em>str</em>) – A property name.</td>
</tr>
<tr class="field-even field"><th class="field-name">Returns:</th><td class="field-body">A potentially transformed property name.</td>
</tr>
<tr class="field-odd field"><th class="field-name">Return type:</th><td class="field-body">str</td>
</tr>
</tbody>
</table>
</dd></dl>

<dl class="method">
<dt id="pulumi_gcp.pubsub.SubscriptionIAMMember.translate_input_property">
<code class="descname">translate_input_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.pubsub.SubscriptionIAMMember.translate_input_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of input properties into
a format of their choosing before sending those properties to the Pulumi engine.</p>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><strong>prop</strong> (<em>str</em>) – A property name.</td>
</tr>
<tr class="field-even field"><th class="field-name">Returns:</th><td class="field-body">A potentially transformed property name.</td>
</tr>
<tr class="field-odd field"><th class="field-name">Return type:</th><td class="field-body">str</td>
</tr>
</tbody>
</table>
</dd></dl>

</dd></dl>

<dl class="class">
<dt id="pulumi_gcp.pubsub.SubscriptionIAMPolicy">
<em class="property">class </em><code class="descclassname">pulumi_gcp.pubsub.</code><code class="descname">SubscriptionIAMPolicy</code><span class="sig-paren">(</span><em>resource_name</em>, <em>opts=None</em>, <em>policy_data=None</em>, <em>project=None</em>, <em>subscription=None</em>, <em>__props__=None</em>, <em>__name__=None</em>, <em>__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.pubsub.SubscriptionIAMPolicy" title="Permalink to this definition">¶</a></dt>
<dd><p>Three different resources help you manage your IAM policy for pubsub subscription. Each of these resources serves a different use case:</p>
<ul class="simple">
<li><code class="docutils literal notranslate"><span class="pre">pubsub.SubscriptionIAMPolicy</span></code>: Authoritative. Sets the IAM policy for the subscription and replaces any existing policy already attached.</li>
<li><code class="docutils literal notranslate"><span class="pre">pubsub.SubscriptionIAMBinding</span></code>: Authoritative for a given role. Updates the IAM policy to grant a role to a list of members. Other roles within the IAM policy for the subscription are preserved.</li>
<li><code class="docutils literal notranslate"><span class="pre">pubsub.SubscriptionIAMMember</span></code>: Non-authoritative. Updates the IAM policy to grant a role to a new member. Other members for the role for the subscription are preserved.</li>
</ul>
<blockquote>
<div><p><strong>Note:</strong> <code class="docutils literal notranslate"><span class="pre">pubsub.SubscriptionIAMPolicy</span></code> <strong>cannot</strong> be used in conjunction with <code class="docutils literal notranslate"><span class="pre">pubsub.SubscriptionIAMBinding</span></code> and <code class="docutils literal notranslate"><span class="pre">pubsub.SubscriptionIAMMember</span></code> or they will fight over what your policy should be.</p>
<p><strong>Note:</strong> <code class="docutils literal notranslate"><span class="pre">pubsub.SubscriptionIAMBinding</span></code> resources <strong>can be</strong> used in conjunction with <code class="docutils literal notranslate"><span class="pre">pubsub.SubscriptionIAMMember</span></code> resources <strong>only if</strong> they do not grant privilege to the same role.</p>
</div></blockquote>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><ul class="first last simple">
<li><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</li>
<li><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</li>
<li><strong>policy_data</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The policy data generated by
a <code class="docutils literal notranslate"><span class="pre">organizations.getIAMPolicy</span></code> data source.</li>
<li><strong>project</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The project in which the resource belongs. If it
is not provided, the provider project is used.</li>
<li><strong>subscription</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The subscription name or id to bind to attach IAM policy to.</li>
</ul>
</td>
</tr>
</tbody>
</table>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/pubsub_subscription_iam_policy.html.markdown">https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/pubsub_subscription_iam_policy.html.markdown</a>.</div></blockquote>
<dl class="attribute">
<dt id="pulumi_gcp.pubsub.SubscriptionIAMPolicy.etag">
<code class="descname">etag</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.pubsub.SubscriptionIAMPolicy.etag" title="Permalink to this definition">¶</a></dt>
<dd><p>(Computed) The etag of the subscription’s IAM policy.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_gcp.pubsub.SubscriptionIAMPolicy.policy_data">
<code class="descname">policy_data</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.pubsub.SubscriptionIAMPolicy.policy_data" title="Permalink to this definition">¶</a></dt>
<dd><p>The policy data generated by
a <code class="docutils literal notranslate"><span class="pre">organizations.getIAMPolicy</span></code> data source.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_gcp.pubsub.SubscriptionIAMPolicy.project">
<code class="descname">project</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.pubsub.SubscriptionIAMPolicy.project" title="Permalink to this definition">¶</a></dt>
<dd><p>The project in which the resource belongs. If it
is not provided, the provider project is used.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_gcp.pubsub.SubscriptionIAMPolicy.subscription">
<code class="descname">subscription</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.pubsub.SubscriptionIAMPolicy.subscription" title="Permalink to this definition">¶</a></dt>
<dd><p>The subscription name or id to bind to attach IAM policy to.</p>
</dd></dl>

<dl class="staticmethod">
<dt id="pulumi_gcp.pubsub.SubscriptionIAMPolicy.get">
<em class="property">static </em><code class="descname">get</code><span class="sig-paren">(</span><em>resource_name</em>, <em>id</em>, <em>opts=None</em>, <em>etag=None</em>, <em>policy_data=None</em>, <em>project=None</em>, <em>subscription=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.pubsub.SubscriptionIAMPolicy.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing SubscriptionIAMPolicy resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.
:param str resource_name: The unique name of the resulting resource.
:param str id: The unique provider ID of the resource to lookup.
:param pulumi.ResourceOptions opts: Options for the resource.
:param pulumi.Input[str] etag: (Computed) The etag of the subscription’s IAM policy.
:param pulumi.Input[str] policy_data: The policy data generated by</p>
<blockquote>
<div>a <code class="docutils literal notranslate"><span class="pre">organizations.getIAMPolicy</span></code> data source.</div></blockquote>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><ul class="first last simple">
<li><strong>project</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The project in which the resource belongs. If it
is not provided, the provider project is used.</li>
<li><strong>subscription</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The subscription name or id to bind to attach IAM policy to.</li>
</ul>
</td>
</tr>
</tbody>
</table>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/pubsub_subscription_iam_policy.html.markdown">https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/pubsub_subscription_iam_policy.html.markdown</a>.</div></blockquote>
</dd></dl>

<dl class="method">
<dt id="pulumi_gcp.pubsub.SubscriptionIAMPolicy.translate_output_property">
<code class="descname">translate_output_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.pubsub.SubscriptionIAMPolicy.translate_output_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of output properties
into a format of their choosing before writing those properties to the resource object.</p>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><strong>prop</strong> (<em>str</em>) – A property name.</td>
</tr>
<tr class="field-even field"><th class="field-name">Returns:</th><td class="field-body">A potentially transformed property name.</td>
</tr>
<tr class="field-odd field"><th class="field-name">Return type:</th><td class="field-body">str</td>
</tr>
</tbody>
</table>
</dd></dl>

<dl class="method">
<dt id="pulumi_gcp.pubsub.SubscriptionIAMPolicy.translate_input_property">
<code class="descname">translate_input_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.pubsub.SubscriptionIAMPolicy.translate_input_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of input properties into
a format of their choosing before sending those properties to the Pulumi engine.</p>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><strong>prop</strong> (<em>str</em>) – A property name.</td>
</tr>
<tr class="field-even field"><th class="field-name">Returns:</th><td class="field-body">A potentially transformed property name.</td>
</tr>
<tr class="field-odd field"><th class="field-name">Return type:</th><td class="field-body">str</td>
</tr>
</tbody>
</table>
</dd></dl>

</dd></dl>

<dl class="class">
<dt id="pulumi_gcp.pubsub.Topic">
<em class="property">class </em><code class="descclassname">pulumi_gcp.pubsub.</code><code class="descname">Topic</code><span class="sig-paren">(</span><em>resource_name</em>, <em>opts=None</em>, <em>kms_key_name=None</em>, <em>labels=None</em>, <em>name=None</em>, <em>project=None</em>, <em>__props__=None</em>, <em>__name__=None</em>, <em>__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.pubsub.Topic" title="Permalink to this definition">¶</a></dt>
<dd><p>A named resource to which messages are sent by publishers.</p>
<p>To get more information about Topic, see:</p>
<ul class="simple">
<li><a class="reference external" href="https://cloud.google.com/pubsub/docs/reference/rest/v1/projects.topics">API documentation</a></li>
<li>How-to Guides<ul>
<li><a class="reference external" href="https://cloud.google.com/pubsub/docs/admin#managing_topics">Managing Topics</a></li>
</ul>
</li>
</ul>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><ul class="first last simple">
<li><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</li>
<li><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</li>
<li><strong>project</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The ID of the project in which the resource belongs.
If it is not provided, the provider project is used.</li>
</ul>
</td>
</tr>
</tbody>
</table>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/pubsub_topic.html.markdown">https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/pubsub_topic.html.markdown</a>.</div></blockquote>
<dl class="attribute">
<dt id="pulumi_gcp.pubsub.Topic.project">
<code class="descname">project</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.pubsub.Topic.project" title="Permalink to this definition">¶</a></dt>
<dd><p>The ID of the project in which the resource belongs.
If it is not provided, the provider project is used.</p>
</dd></dl>

<dl class="staticmethod">
<dt id="pulumi_gcp.pubsub.Topic.get">
<em class="property">static </em><code class="descname">get</code><span class="sig-paren">(</span><em>resource_name</em>, <em>id</em>, <em>opts=None</em>, <em>kms_key_name=None</em>, <em>labels=None</em>, <em>name=None</em>, <em>project=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.pubsub.Topic.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing Topic resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.
:param str resource_name: The unique name of the resulting resource.
:param str id: The unique provider ID of the resource to lookup.
:param pulumi.ResourceOptions opts: Options for the resource.
:param pulumi.Input[str] project: The ID of the project in which the resource belongs.</p>
<blockquote>
<div>If it is not provided, the provider project is used.</div></blockquote>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/pubsub_topic.html.markdown">https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/pubsub_topic.html.markdown</a>.</div></blockquote>
</dd></dl>

<dl class="method">
<dt id="pulumi_gcp.pubsub.Topic.translate_output_property">
<code class="descname">translate_output_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.pubsub.Topic.translate_output_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of output properties
into a format of their choosing before writing those properties to the resource object.</p>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><strong>prop</strong> (<em>str</em>) – A property name.</td>
</tr>
<tr class="field-even field"><th class="field-name">Returns:</th><td class="field-body">A potentially transformed property name.</td>
</tr>
<tr class="field-odd field"><th class="field-name">Return type:</th><td class="field-body">str</td>
</tr>
</tbody>
</table>
</dd></dl>

<dl class="method">
<dt id="pulumi_gcp.pubsub.Topic.translate_input_property">
<code class="descname">translate_input_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.pubsub.Topic.translate_input_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of input properties into
a format of their choosing before sending those properties to the Pulumi engine.</p>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><strong>prop</strong> (<em>str</em>) – A property name.</td>
</tr>
<tr class="field-even field"><th class="field-name">Returns:</th><td class="field-body">A potentially transformed property name.</td>
</tr>
<tr class="field-odd field"><th class="field-name">Return type:</th><td class="field-body">str</td>
</tr>
</tbody>
</table>
</dd></dl>

</dd></dl>

<dl class="class">
<dt id="pulumi_gcp.pubsub.TopicIAMBinding">
<em class="property">class </em><code class="descclassname">pulumi_gcp.pubsub.</code><code class="descname">TopicIAMBinding</code><span class="sig-paren">(</span><em>resource_name</em>, <em>opts=None</em>, <em>members=None</em>, <em>project=None</em>, <em>role=None</em>, <em>topic=None</em>, <em>__props__=None</em>, <em>__name__=None</em>, <em>__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.pubsub.TopicIAMBinding" title="Permalink to this definition">¶</a></dt>
<dd><p>Three different resources help you manage your IAM policy for Pubsub Topic. Each of these resources serves a different use case:</p>
<ul class="simple">
<li><code class="docutils literal notranslate"><span class="pre">pubsub.TopicIAMPolicy</span></code>: Authoritative. Sets the IAM policy for the topic and replaces any existing policy already attached.</li>
<li><code class="docutils literal notranslate"><span class="pre">pubsub.TopicIAMBinding</span></code>: Authoritative for a given role. Updates the IAM policy to grant a role to a list of members. Other roles within the IAM policy for the topic are preserved.</li>
<li><code class="docutils literal notranslate"><span class="pre">pubsub.TopicIAMMember</span></code>: Non-authoritative. Updates the IAM policy to grant a role to a new member. Other members for the role for the topic are preserved.</li>
</ul>
<blockquote>
<div><p><strong>Note:</strong> <code class="docutils literal notranslate"><span class="pre">pubsub.TopicIAMPolicy</span></code> <strong>cannot</strong> be used in conjunction with <code class="docutils literal notranslate"><span class="pre">pubsub.TopicIAMBinding</span></code> and <code class="docutils literal notranslate"><span class="pre">pubsub.TopicIAMMember</span></code> or they will fight over what your policy should be.</p>
<p><strong>Note:</strong> <code class="docutils literal notranslate"><span class="pre">pubsub.TopicIAMBinding</span></code> resources <strong>can be</strong> used in conjunction with <code class="docutils literal notranslate"><span class="pre">pubsub.TopicIAMMember</span></code> resources <strong>only if</strong> they do not grant privilege to the same role.</p>
</div></blockquote>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><ul class="first last simple">
<li><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</li>
<li><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</li>
<li><strong>project</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The project in which the resource belongs. If it
is not provided, the provider project is used.</li>
<li><strong>role</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The role that should be applied. Only one
<code class="docutils literal notranslate"><span class="pre">pubsub.TopicIAMBinding</span></code> can be used per role. Note that custom roles must be of the format
<code class="docutils literal notranslate"><span class="pre">[projects|organizations]/{parent-name}/roles/{role-name}</span></code>.</li>
<li><strong>topic</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The topic name or id to bind to attach IAM policy to.</li>
</ul>
</td>
</tr>
</tbody>
</table>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/pubsub_topic_iam_binding.html.markdown">https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/pubsub_topic_iam_binding.html.markdown</a>.</div></blockquote>
<dl class="attribute">
<dt id="pulumi_gcp.pubsub.TopicIAMBinding.etag">
<code class="descname">etag</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.pubsub.TopicIAMBinding.etag" title="Permalink to this definition">¶</a></dt>
<dd><p>(Computed) The etag of the topic’s IAM policy.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_gcp.pubsub.TopicIAMBinding.project">
<code class="descname">project</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.pubsub.TopicIAMBinding.project" title="Permalink to this definition">¶</a></dt>
<dd><p>The project in which the resource belongs. If it
is not provided, the provider project is used.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_gcp.pubsub.TopicIAMBinding.role">
<code class="descname">role</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.pubsub.TopicIAMBinding.role" title="Permalink to this definition">¶</a></dt>
<dd><p>The role that should be applied. Only one
<code class="docutils literal notranslate"><span class="pre">pubsub.TopicIAMBinding</span></code> can be used per role. Note that custom roles must be of the format
<code class="docutils literal notranslate"><span class="pre">[projects|organizations]/{parent-name}/roles/{role-name}</span></code>.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_gcp.pubsub.TopicIAMBinding.topic">
<code class="descname">topic</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.pubsub.TopicIAMBinding.topic" title="Permalink to this definition">¶</a></dt>
<dd><p>The topic name or id to bind to attach IAM policy to.</p>
</dd></dl>

<dl class="staticmethod">
<dt id="pulumi_gcp.pubsub.TopicIAMBinding.get">
<em class="property">static </em><code class="descname">get</code><span class="sig-paren">(</span><em>resource_name</em>, <em>id</em>, <em>opts=None</em>, <em>etag=None</em>, <em>members=None</em>, <em>project=None</em>, <em>role=None</em>, <em>topic=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.pubsub.TopicIAMBinding.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing TopicIAMBinding resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.
:param str resource_name: The unique name of the resulting resource.
:param str id: The unique provider ID of the resource to lookup.
:param pulumi.ResourceOptions opts: Options for the resource.
:param pulumi.Input[str] etag: (Computed) The etag of the topic’s IAM policy.
:param pulumi.Input[str] project: The project in which the resource belongs. If it</p>
<blockquote>
<div>is not provided, the provider project is used.</div></blockquote>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><ul class="first last simple">
<li><strong>role</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The role that should be applied. Only one
<code class="docutils literal notranslate"><span class="pre">pubsub.TopicIAMBinding</span></code> can be used per role. Note that custom roles must be of the format
<code class="docutils literal notranslate"><span class="pre">[projects|organizations]/{parent-name}/roles/{role-name}</span></code>.</li>
<li><strong>topic</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The topic name or id to bind to attach IAM policy to.</li>
</ul>
</td>
</tr>
</tbody>
</table>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/pubsub_topic_iam_binding.html.markdown">https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/pubsub_topic_iam_binding.html.markdown</a>.</div></blockquote>
</dd></dl>

<dl class="method">
<dt id="pulumi_gcp.pubsub.TopicIAMBinding.translate_output_property">
<code class="descname">translate_output_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.pubsub.TopicIAMBinding.translate_output_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of output properties
into a format of their choosing before writing those properties to the resource object.</p>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><strong>prop</strong> (<em>str</em>) – A property name.</td>
</tr>
<tr class="field-even field"><th class="field-name">Returns:</th><td class="field-body">A potentially transformed property name.</td>
</tr>
<tr class="field-odd field"><th class="field-name">Return type:</th><td class="field-body">str</td>
</tr>
</tbody>
</table>
</dd></dl>

<dl class="method">
<dt id="pulumi_gcp.pubsub.TopicIAMBinding.translate_input_property">
<code class="descname">translate_input_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.pubsub.TopicIAMBinding.translate_input_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of input properties into
a format of their choosing before sending those properties to the Pulumi engine.</p>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><strong>prop</strong> (<em>str</em>) – A property name.</td>
</tr>
<tr class="field-even field"><th class="field-name">Returns:</th><td class="field-body">A potentially transformed property name.</td>
</tr>
<tr class="field-odd field"><th class="field-name">Return type:</th><td class="field-body">str</td>
</tr>
</tbody>
</table>
</dd></dl>

</dd></dl>

<dl class="class">
<dt id="pulumi_gcp.pubsub.TopicIAMMember">
<em class="property">class </em><code class="descclassname">pulumi_gcp.pubsub.</code><code class="descname">TopicIAMMember</code><span class="sig-paren">(</span><em>resource_name</em>, <em>opts=None</em>, <em>member=None</em>, <em>project=None</em>, <em>role=None</em>, <em>topic=None</em>, <em>__props__=None</em>, <em>__name__=None</em>, <em>__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.pubsub.TopicIAMMember" title="Permalink to this definition">¶</a></dt>
<dd><p>Three different resources help you manage your IAM policy for Pubsub Topic. Each of these resources serves a different use case:</p>
<ul class="simple">
<li><code class="docutils literal notranslate"><span class="pre">pubsub.TopicIAMPolicy</span></code>: Authoritative. Sets the IAM policy for the topic and replaces any existing policy already attached.</li>
<li><code class="docutils literal notranslate"><span class="pre">pubsub.TopicIAMBinding</span></code>: Authoritative for a given role. Updates the IAM policy to grant a role to a list of members. Other roles within the IAM policy for the topic are preserved.</li>
<li><code class="docutils literal notranslate"><span class="pre">pubsub.TopicIAMMember</span></code>: Non-authoritative. Updates the IAM policy to grant a role to a new member. Other members for the role for the topic are preserved.</li>
</ul>
<blockquote>
<div><p><strong>Note:</strong> <code class="docutils literal notranslate"><span class="pre">pubsub.TopicIAMPolicy</span></code> <strong>cannot</strong> be used in conjunction with <code class="docutils literal notranslate"><span class="pre">pubsub.TopicIAMBinding</span></code> and <code class="docutils literal notranslate"><span class="pre">pubsub.TopicIAMMember</span></code> or they will fight over what your policy should be.</p>
<p><strong>Note:</strong> <code class="docutils literal notranslate"><span class="pre">pubsub.TopicIAMBinding</span></code> resources <strong>can be</strong> used in conjunction with <code class="docutils literal notranslate"><span class="pre">pubsub.TopicIAMMember</span></code> resources <strong>only if</strong> they do not grant privilege to the same role.</p>
</div></blockquote>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><ul class="first last simple">
<li><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</li>
<li><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</li>
<li><strong>project</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The project in which the resource belongs. If it
is not provided, the provider project is used.</li>
<li><strong>role</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The role that should be applied. Only one
<code class="docutils literal notranslate"><span class="pre">pubsub.TopicIAMBinding</span></code> can be used per role. Note that custom roles must be of the format
<code class="docutils literal notranslate"><span class="pre">[projects|organizations]/{parent-name}/roles/{role-name}</span></code>.</li>
<li><strong>topic</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The topic name or id to bind to attach IAM policy to.</li>
</ul>
</td>
</tr>
</tbody>
</table>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/pubsub_topic_iam_member.html.markdown">https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/pubsub_topic_iam_member.html.markdown</a>.</div></blockquote>
<dl class="attribute">
<dt id="pulumi_gcp.pubsub.TopicIAMMember.etag">
<code class="descname">etag</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.pubsub.TopicIAMMember.etag" title="Permalink to this definition">¶</a></dt>
<dd><p>(Computed) The etag of the topic’s IAM policy.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_gcp.pubsub.TopicIAMMember.project">
<code class="descname">project</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.pubsub.TopicIAMMember.project" title="Permalink to this definition">¶</a></dt>
<dd><p>The project in which the resource belongs. If it
is not provided, the provider project is used.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_gcp.pubsub.TopicIAMMember.role">
<code class="descname">role</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.pubsub.TopicIAMMember.role" title="Permalink to this definition">¶</a></dt>
<dd><p>The role that should be applied. Only one
<code class="docutils literal notranslate"><span class="pre">pubsub.TopicIAMBinding</span></code> can be used per role. Note that custom roles must be of the format
<code class="docutils literal notranslate"><span class="pre">[projects|organizations]/{parent-name}/roles/{role-name}</span></code>.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_gcp.pubsub.TopicIAMMember.topic">
<code class="descname">topic</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.pubsub.TopicIAMMember.topic" title="Permalink to this definition">¶</a></dt>
<dd><p>The topic name or id to bind to attach IAM policy to.</p>
</dd></dl>

<dl class="staticmethod">
<dt id="pulumi_gcp.pubsub.TopicIAMMember.get">
<em class="property">static </em><code class="descname">get</code><span class="sig-paren">(</span><em>resource_name</em>, <em>id</em>, <em>opts=None</em>, <em>etag=None</em>, <em>member=None</em>, <em>project=None</em>, <em>role=None</em>, <em>topic=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.pubsub.TopicIAMMember.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing TopicIAMMember resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.
:param str resource_name: The unique name of the resulting resource.
:param str id: The unique provider ID of the resource to lookup.
:param pulumi.ResourceOptions opts: Options for the resource.
:param pulumi.Input[str] etag: (Computed) The etag of the topic’s IAM policy.
:param pulumi.Input[str] project: The project in which the resource belongs. If it</p>
<blockquote>
<div>is not provided, the provider project is used.</div></blockquote>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><ul class="first last simple">
<li><strong>role</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The role that should be applied. Only one
<code class="docutils literal notranslate"><span class="pre">pubsub.TopicIAMBinding</span></code> can be used per role. Note that custom roles must be of the format
<code class="docutils literal notranslate"><span class="pre">[projects|organizations]/{parent-name}/roles/{role-name}</span></code>.</li>
<li><strong>topic</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The topic name or id to bind to attach IAM policy to.</li>
</ul>
</td>
</tr>
</tbody>
</table>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/pubsub_topic_iam_member.html.markdown">https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/pubsub_topic_iam_member.html.markdown</a>.</div></blockquote>
</dd></dl>

<dl class="method">
<dt id="pulumi_gcp.pubsub.TopicIAMMember.translate_output_property">
<code class="descname">translate_output_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.pubsub.TopicIAMMember.translate_output_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of output properties
into a format of their choosing before writing those properties to the resource object.</p>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><strong>prop</strong> (<em>str</em>) – A property name.</td>
</tr>
<tr class="field-even field"><th class="field-name">Returns:</th><td class="field-body">A potentially transformed property name.</td>
</tr>
<tr class="field-odd field"><th class="field-name">Return type:</th><td class="field-body">str</td>
</tr>
</tbody>
</table>
</dd></dl>

<dl class="method">
<dt id="pulumi_gcp.pubsub.TopicIAMMember.translate_input_property">
<code class="descname">translate_input_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.pubsub.TopicIAMMember.translate_input_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of input properties into
a format of their choosing before sending those properties to the Pulumi engine.</p>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><strong>prop</strong> (<em>str</em>) – A property name.</td>
</tr>
<tr class="field-even field"><th class="field-name">Returns:</th><td class="field-body">A potentially transformed property name.</td>
</tr>
<tr class="field-odd field"><th class="field-name">Return type:</th><td class="field-body">str</td>
</tr>
</tbody>
</table>
</dd></dl>

</dd></dl>

<dl class="class">
<dt id="pulumi_gcp.pubsub.TopicIAMPolicy">
<em class="property">class </em><code class="descclassname">pulumi_gcp.pubsub.</code><code class="descname">TopicIAMPolicy</code><span class="sig-paren">(</span><em>resource_name</em>, <em>opts=None</em>, <em>policy_data=None</em>, <em>project=None</em>, <em>topic=None</em>, <em>__props__=None</em>, <em>__name__=None</em>, <em>__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.pubsub.TopicIAMPolicy" title="Permalink to this definition">¶</a></dt>
<dd><p>Three different resources help you manage your IAM policy for Pubsub Topic. Each of these resources serves a different use case:</p>
<ul class="simple">
<li><code class="docutils literal notranslate"><span class="pre">pubsub.TopicIAMPolicy</span></code>: Authoritative. Sets the IAM policy for the topic and replaces any existing policy already attached.</li>
<li><code class="docutils literal notranslate"><span class="pre">pubsub.TopicIAMBinding</span></code>: Authoritative for a given role. Updates the IAM policy to grant a role to a list of members. Other roles within the IAM policy for the topic are preserved.</li>
<li><code class="docutils literal notranslate"><span class="pre">pubsub.TopicIAMMember</span></code>: Non-authoritative. Updates the IAM policy to grant a role to a new member. Other members for the role for the topic are preserved.</li>
</ul>
<blockquote>
<div><p><strong>Note:</strong> <code class="docutils literal notranslate"><span class="pre">pubsub.TopicIAMPolicy</span></code> <strong>cannot</strong> be used in conjunction with <code class="docutils literal notranslate"><span class="pre">pubsub.TopicIAMBinding</span></code> and <code class="docutils literal notranslate"><span class="pre">pubsub.TopicIAMMember</span></code> or they will fight over what your policy should be.</p>
<p><strong>Note:</strong> <code class="docutils literal notranslate"><span class="pre">pubsub.TopicIAMBinding</span></code> resources <strong>can be</strong> used in conjunction with <code class="docutils literal notranslate"><span class="pre">pubsub.TopicIAMMember</span></code> resources <strong>only if</strong> they do not grant privilege to the same role.</p>
</div></blockquote>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><ul class="first last simple">
<li><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</li>
<li><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</li>
<li><strong>policy_data</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The policy data generated by
a <code class="docutils literal notranslate"><span class="pre">organizations.getIAMPolicy</span></code> data source.</li>
<li><strong>project</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The project in which the resource belongs. If it
is not provided, the provider project is used.</li>
<li><strong>topic</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The topic name or id to bind to attach IAM policy to.</li>
</ul>
</td>
</tr>
</tbody>
</table>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/pubsub_topic_iam_policy.html.markdown">https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/pubsub_topic_iam_policy.html.markdown</a>.</div></blockquote>
<dl class="attribute">
<dt id="pulumi_gcp.pubsub.TopicIAMPolicy.etag">
<code class="descname">etag</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.pubsub.TopicIAMPolicy.etag" title="Permalink to this definition">¶</a></dt>
<dd><p>(Computed) The etag of the topic’s IAM policy.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_gcp.pubsub.TopicIAMPolicy.policy_data">
<code class="descname">policy_data</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.pubsub.TopicIAMPolicy.policy_data" title="Permalink to this definition">¶</a></dt>
<dd><p>The policy data generated by
a <code class="docutils literal notranslate"><span class="pre">organizations.getIAMPolicy</span></code> data source.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_gcp.pubsub.TopicIAMPolicy.project">
<code class="descname">project</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.pubsub.TopicIAMPolicy.project" title="Permalink to this definition">¶</a></dt>
<dd><p>The project in which the resource belongs. If it
is not provided, the provider project is used.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_gcp.pubsub.TopicIAMPolicy.topic">
<code class="descname">topic</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.pubsub.TopicIAMPolicy.topic" title="Permalink to this definition">¶</a></dt>
<dd><p>The topic name or id to bind to attach IAM policy to.</p>
</dd></dl>

<dl class="staticmethod">
<dt id="pulumi_gcp.pubsub.TopicIAMPolicy.get">
<em class="property">static </em><code class="descname">get</code><span class="sig-paren">(</span><em>resource_name</em>, <em>id</em>, <em>opts=None</em>, <em>etag=None</em>, <em>policy_data=None</em>, <em>project=None</em>, <em>topic=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.pubsub.TopicIAMPolicy.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing TopicIAMPolicy resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.
:param str resource_name: The unique name of the resulting resource.
:param str id: The unique provider ID of the resource to lookup.
:param pulumi.ResourceOptions opts: Options for the resource.
:param pulumi.Input[str] etag: (Computed) The etag of the topic’s IAM policy.
:param pulumi.Input[str] policy_data: The policy data generated by</p>
<blockquote>
<div>a <code class="docutils literal notranslate"><span class="pre">organizations.getIAMPolicy</span></code> data source.</div></blockquote>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><ul class="first last simple">
<li><strong>project</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The project in which the resource belongs. If it
is not provided, the provider project is used.</li>
<li><strong>topic</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The topic name or id to bind to attach IAM policy to.</li>
</ul>
</td>
</tr>
</tbody>
</table>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/pubsub_topic_iam_policy.html.markdown">https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/pubsub_topic_iam_policy.html.markdown</a>.</div></blockquote>
</dd></dl>

<dl class="method">
<dt id="pulumi_gcp.pubsub.TopicIAMPolicy.translate_output_property">
<code class="descname">translate_output_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.pubsub.TopicIAMPolicy.translate_output_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of output properties
into a format of their choosing before writing those properties to the resource object.</p>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><strong>prop</strong> (<em>str</em>) – A property name.</td>
</tr>
<tr class="field-even field"><th class="field-name">Returns:</th><td class="field-body">A potentially transformed property name.</td>
</tr>
<tr class="field-odd field"><th class="field-name">Return type:</th><td class="field-body">str</td>
</tr>
</tbody>
</table>
</dd></dl>

<dl class="method">
<dt id="pulumi_gcp.pubsub.TopicIAMPolicy.translate_input_property">
<code class="descname">translate_input_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.pubsub.TopicIAMPolicy.translate_input_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of input properties into
a format of their choosing before sending those properties to the Pulumi engine.</p>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><strong>prop</strong> (<em>str</em>) – A property name.</td>
</tr>
<tr class="field-even field"><th class="field-name">Returns:</th><td class="field-body">A potentially transformed property name.</td>
</tr>
<tr class="field-odd field"><th class="field-name">Return type:</th><td class="field-body">str</td>
</tr>
</tbody>
</table>
</dd></dl>

</dd></dl>

</div>
