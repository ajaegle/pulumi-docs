---
title: Module billing
---

<div class="section" id="billing">
<h1>billing<a class="headerlink" href="#billing" title="Permalink to this headline">¶</a></h1>
<blockquote>
<div>This provider is a derived work of the <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-google">Terraform Provider</a> distributed under
<a class="reference external" href="https://www.mozilla.org/en-US/MPL/2.0/">MPL 2.0</a>. If you encounter a bug or missing feature, first check the
<a class="reference external" href="https://github.com/pulumi/pulumi-gcp/issues">pulumi/pulumi-gcp repo</a>; however, if that doesn’t turn up
anything, please consult the source <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-google/issues">terraform-providers/terraform-provider-google repo</a>.</div></blockquote>
<span class="target" id="module-pulumi_gcp.billing"></span><dl class="class">
<dt id="pulumi_gcp.billing.AccountIamBinding">
<em class="property">class </em><code class="descclassname">pulumi_gcp.billing.</code><code class="descname">AccountIamBinding</code><span class="sig-paren">(</span><em>resource_name</em>, <em>opts=None</em>, <em>billing_account_id=None</em>, <em>members=None</em>, <em>role=None</em>, <em>__props__=None</em>, <em>__name__=None</em>, <em>__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.billing.AccountIamBinding" title="Permalink to this definition">¶</a></dt>
<dd><p>Allows creation and management of a single binding within IAM policy for
an existing Google Cloud Platform Billing Account.</p>
<blockquote>
<div><dl class="docutils">
<dt><strong>Note:</strong> This resource <strong>must not</strong> be used in conjunction with</dt>
<dd><code class="docutils literal notranslate"><span class="pre">billing.AccountIamMember</span></code> for the <strong>same role</strong> or they will fight over
what your policy should be.</dd>
<dt><strong>Note:</strong> On create, this resource will overwrite members of any existing roles.</dt>
<dd>Use <code class="docutils literal notranslate"><span class="pre">import</span></code> and inspect the preview output to ensure
your existing members are preserved.</dd>
</dl>
</div></blockquote>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><ul class="first last simple">
<li><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</li>
<li><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</li>
<li><strong>billing_account_id</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The billing account id.</li>
<li><strong>members</strong> (<em>pulumi.Input</em><em>[</em><em>list</em><em>]</em>) – A list of users that the role should apply to. For more details on format and restrictions see <a class="reference external" href="https://cloud.google.com/billing/reference/rest/v1/Policy#Binding">https://cloud.google.com/billing/reference/rest/v1/Policy#Binding</a></li>
<li><strong>role</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The role that should be applied.</li>
</ul>
</td>
</tr>
</tbody>
</table>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/billing_account_iam_binding.html.markdown">https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/billing_account_iam_binding.html.markdown</a>.</div></blockquote>
<dl class="attribute">
<dt id="pulumi_gcp.billing.AccountIamBinding.billing_account_id">
<code class="descname">billing_account_id</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.billing.AccountIamBinding.billing_account_id" title="Permalink to this definition">¶</a></dt>
<dd><p>The billing account id.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_gcp.billing.AccountIamBinding.etag">
<code class="descname">etag</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.billing.AccountIamBinding.etag" title="Permalink to this definition">¶</a></dt>
<dd><p>(Computed) The etag of the billing account’s IAM policy.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_gcp.billing.AccountIamBinding.members">
<code class="descname">members</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.billing.AccountIamBinding.members" title="Permalink to this definition">¶</a></dt>
<dd><p>A list of users that the role should apply to. For more details on format and restrictions see <a class="reference external" href="https://cloud.google.com/billing/reference/rest/v1/Policy#Binding">https://cloud.google.com/billing/reference/rest/v1/Policy#Binding</a></p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_gcp.billing.AccountIamBinding.role">
<code class="descname">role</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.billing.AccountIamBinding.role" title="Permalink to this definition">¶</a></dt>
<dd><p>The role that should be applied.</p>
</dd></dl>

<dl class="staticmethod">
<dt id="pulumi_gcp.billing.AccountIamBinding.get">
<em class="property">static </em><code class="descname">get</code><span class="sig-paren">(</span><em>resource_name</em>, <em>id</em>, <em>opts=None</em>, <em>billing_account_id=None</em>, <em>etag=None</em>, <em>members=None</em>, <em>role=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.billing.AccountIamBinding.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing AccountIamBinding resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.
:param str resource_name: The unique name of the resulting resource.
:param str id: The unique provider ID of the resource to lookup.
:param pulumi.ResourceOptions opts: Options for the resource.
:param pulumi.Input[str] billing_account_id: The billing account id.
:param pulumi.Input[str] etag: (Computed) The etag of the billing account’s IAM policy.
:param pulumi.Input[list] members: A list of users that the role should apply to. For more details on format and restrictions see <a class="reference external" href="https://cloud.google.com/billing/reference/rest/v1/Policy#Binding">https://cloud.google.com/billing/reference/rest/v1/Policy#Binding</a>
:param pulumi.Input[str] role: The role that should be applied.</p>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/billing_account_iam_binding.html.markdown">https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/billing_account_iam_binding.html.markdown</a>.</div></blockquote>
</dd></dl>

<dl class="method">
<dt id="pulumi_gcp.billing.AccountIamBinding.translate_output_property">
<code class="descname">translate_output_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.billing.AccountIamBinding.translate_output_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_gcp.billing.AccountIamBinding.translate_input_property">
<code class="descname">translate_input_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.billing.AccountIamBinding.translate_input_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_gcp.billing.AccountIamMember">
<em class="property">class </em><code class="descclassname">pulumi_gcp.billing.</code><code class="descname">AccountIamMember</code><span class="sig-paren">(</span><em>resource_name</em>, <em>opts=None</em>, <em>billing_account_id=None</em>, <em>member=None</em>, <em>role=None</em>, <em>__props__=None</em>, <em>__name__=None</em>, <em>__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.billing.AccountIamMember" title="Permalink to this definition">¶</a></dt>
<dd><p>Allows creation and management of a single member for a single binding within
the IAM policy for an existing Google Cloud Platform Billing Account.</p>
<blockquote>
<div><dl class="docutils">
<dt><strong>Note:</strong> This resource <strong>must not</strong> be used in conjunction with</dt>
<dd><code class="docutils literal notranslate"><span class="pre">billing.AccountIamBinding</span></code> for the <strong>same role</strong> or they will fight over
what your policy should be.</dd>
</dl>
</div></blockquote>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><ul class="first last simple">
<li><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</li>
<li><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</li>
<li><strong>billing_account_id</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The billing account id.</li>
<li><strong>member</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The user that the role should apply to. For more details on format and restrictions see <a class="reference external" href="https://cloud.google.com/billing/reference/rest/v1/Policy#Binding">https://cloud.google.com/billing/reference/rest/v1/Policy#Binding</a></li>
<li><strong>role</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The role that should be applied.</li>
</ul>
</td>
</tr>
</tbody>
</table>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/billing_account_iam_member.html.markdown">https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/billing_account_iam_member.html.markdown</a>.</div></blockquote>
<dl class="attribute">
<dt id="pulumi_gcp.billing.AccountIamMember.billing_account_id">
<code class="descname">billing_account_id</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.billing.AccountIamMember.billing_account_id" title="Permalink to this definition">¶</a></dt>
<dd><p>The billing account id.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_gcp.billing.AccountIamMember.etag">
<code class="descname">etag</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.billing.AccountIamMember.etag" title="Permalink to this definition">¶</a></dt>
<dd><p>(Computed) The etag of the billing account’s IAM policy.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_gcp.billing.AccountIamMember.member">
<code class="descname">member</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.billing.AccountIamMember.member" title="Permalink to this definition">¶</a></dt>
<dd><p>The user that the role should apply to. For more details on format and restrictions see <a class="reference external" href="https://cloud.google.com/billing/reference/rest/v1/Policy#Binding">https://cloud.google.com/billing/reference/rest/v1/Policy#Binding</a></p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_gcp.billing.AccountIamMember.role">
<code class="descname">role</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.billing.AccountIamMember.role" title="Permalink to this definition">¶</a></dt>
<dd><p>The role that should be applied.</p>
</dd></dl>

<dl class="staticmethod">
<dt id="pulumi_gcp.billing.AccountIamMember.get">
<em class="property">static </em><code class="descname">get</code><span class="sig-paren">(</span><em>resource_name</em>, <em>id</em>, <em>opts=None</em>, <em>billing_account_id=None</em>, <em>etag=None</em>, <em>member=None</em>, <em>role=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.billing.AccountIamMember.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing AccountIamMember resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.
:param str resource_name: The unique name of the resulting resource.
:param str id: The unique provider ID of the resource to lookup.
:param pulumi.ResourceOptions opts: Options for the resource.
:param pulumi.Input[str] billing_account_id: The billing account id.
:param pulumi.Input[str] etag: (Computed) The etag of the billing account’s IAM policy.
:param pulumi.Input[str] member: The user that the role should apply to. For more details on format and restrictions see <a class="reference external" href="https://cloud.google.com/billing/reference/rest/v1/Policy#Binding">https://cloud.google.com/billing/reference/rest/v1/Policy#Binding</a>
:param pulumi.Input[str] role: The role that should be applied.</p>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/billing_account_iam_member.html.markdown">https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/billing_account_iam_member.html.markdown</a>.</div></blockquote>
</dd></dl>

<dl class="method">
<dt id="pulumi_gcp.billing.AccountIamMember.translate_output_property">
<code class="descname">translate_output_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.billing.AccountIamMember.translate_output_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_gcp.billing.AccountIamMember.translate_input_property">
<code class="descname">translate_input_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.billing.AccountIamMember.translate_input_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_gcp.billing.AccountIamPolicy">
<em class="property">class </em><code class="descclassname">pulumi_gcp.billing.</code><code class="descname">AccountIamPolicy</code><span class="sig-paren">(</span><em>resource_name</em>, <em>opts=None</em>, <em>billing_account_id=None</em>, <em>policy_data=None</em>, <em>__props__=None</em>, <em>__name__=None</em>, <em>__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.billing.AccountIamPolicy" title="Permalink to this definition">¶</a></dt>
<dd><p>Allows management of the entire IAM policy for an existing Google Cloud Platform Billing Account.</p>
<blockquote>
<div><p><strong>Warning:</strong> Billing accounts have a default user that can be <strong>overwritten</strong>
by use of this resource. The safest alternative is to use multiple <code class="docutils literal notranslate"><span class="pre">billing.AccountIamBinding</span></code></p>
<blockquote>
<div>resources. If you do use this resource, the best way to be sure that you are
not making dangerous changes is to start by importing your existing policy,
and examining the diff very closely.</div></blockquote>
<dl class="docutils">
<dt><strong>Note:</strong> This resource <strong>must not</strong> be used in conjunction with</dt>
<dd><code class="docutils literal notranslate"><span class="pre">billing.AccountIamMember</span></code> or <code class="docutils literal notranslate"><span class="pre">billing.AccountIamBinding</span></code>
or they will fight over what your policy should be.</dd>
</dl>
</div></blockquote>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><ul class="first last simple">
<li><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</li>
<li><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</li>
<li><strong>billing_account_id</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The billing account id.</li>
<li><strong>policy_data</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The <code class="docutils literal notranslate"><span class="pre">organizations.getIAMPolicy</span></code> data source that represents
the IAM policy that will be applied to the billing account. This policy overrides any existing
policy applied to the billing account.</li>
</ul>
</td>
</tr>
</tbody>
</table>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/billing_account_iam_policy.html.markdown">https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/billing_account_iam_policy.html.markdown</a>.</div></blockquote>
<dl class="attribute">
<dt id="pulumi_gcp.billing.AccountIamPolicy.billing_account_id">
<code class="descname">billing_account_id</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.billing.AccountIamPolicy.billing_account_id" title="Permalink to this definition">¶</a></dt>
<dd><p>The billing account id.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_gcp.billing.AccountIamPolicy.policy_data">
<code class="descname">policy_data</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.billing.AccountIamPolicy.policy_data" title="Permalink to this definition">¶</a></dt>
<dd><p>The <code class="docutils literal notranslate"><span class="pre">organizations.getIAMPolicy</span></code> data source that represents
the IAM policy that will be applied to the billing account. This policy overrides any existing
policy applied to the billing account.</p>
</dd></dl>

<dl class="staticmethod">
<dt id="pulumi_gcp.billing.AccountIamPolicy.get">
<em class="property">static </em><code class="descname">get</code><span class="sig-paren">(</span><em>resource_name</em>, <em>id</em>, <em>opts=None</em>, <em>billing_account_id=None</em>, <em>etag=None</em>, <em>policy_data=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.billing.AccountIamPolicy.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing AccountIamPolicy resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.
:param str resource_name: The unique name of the resulting resource.
:param str id: The unique provider ID of the resource to lookup.
:param pulumi.ResourceOptions opts: Options for the resource.
:param pulumi.Input[str] billing_account_id: The billing account id.
:param pulumi.Input[str] policy_data: The <code class="docutils literal notranslate"><span class="pre">organizations.getIAMPolicy</span></code> data source that represents</p>
<blockquote>
<div>the IAM policy that will be applied to the billing account. This policy overrides any existing
policy applied to the billing account.</div></blockquote>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/billing_account_iam_policy.html.markdown">https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/billing_account_iam_policy.html.markdown</a>.</div></blockquote>
</dd></dl>

<dl class="method">
<dt id="pulumi_gcp.billing.AccountIamPolicy.translate_output_property">
<code class="descname">translate_output_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.billing.AccountIamPolicy.translate_output_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_gcp.billing.AccountIamPolicy.translate_input_property">
<code class="descname">translate_input_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.billing.AccountIamPolicy.translate_input_property" title="Permalink to this definition">¶</a></dt>
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
