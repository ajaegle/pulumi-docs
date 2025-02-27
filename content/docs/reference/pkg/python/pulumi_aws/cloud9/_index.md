---
title: Module cloud9
---

<div class="section" id="cloud9">
<h1>cloud9<a class="headerlink" href="#cloud9" title="Permalink to this headline">¶</a></h1>
<blockquote>
<div>This provider is a derived work of the <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-aws">Terraform Provider</a> distributed under
<a class="reference external" href="https://www.mozilla.org/en-US/MPL/2.0/">MPL 2.0</a>. If you encounter a bug or missing feature, first check the
<a class="reference external" href="https://github.com/pulumi/pulumi-aws/issues">pulumi/pulumi-aws repo</a>; however, if that doesn’t turn up
anything, please consult the source <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-aws/issues">terraform-providers/terraform-provider-aws repo</a>.</div></blockquote>
<span class="target" id="module-pulumi_aws.cloud9"></span><dl class="class">
<dt id="pulumi_aws.cloud9.EnvironmentEC2">
<em class="property">class </em><code class="descclassname">pulumi_aws.cloud9.</code><code class="descname">EnvironmentEC2</code><span class="sig-paren">(</span><em>resource_name</em>, <em>opts=None</em>, <em>automatic_stop_time_minutes=None</em>, <em>description=None</em>, <em>instance_type=None</em>, <em>name=None</em>, <em>owner_arn=None</em>, <em>subnet_id=None</em>, <em>__props__=None</em>, <em>__name__=None</em>, <em>__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_aws.cloud9.EnvironmentEC2" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides a Cloud9 EC2 Development Environment.</p>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><ul class="first last simple">
<li><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</li>
<li><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</li>
<li><strong>automatic_stop_time_minutes</strong> (<em>pulumi.Input</em><em>[</em><em>float</em><em>]</em>) – The number of minutes until the running instance is shut down after the environment has last been used.</li>
<li><strong>description</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The description of the environment.</li>
<li><strong>instance_type</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The type of instance to connect to the environment, e.g. <code class="docutils literal notranslate"><span class="pre">t2.micro</span></code>.</li>
<li><strong>name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The name of the environment.</li>
<li><strong>owner_arn</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The ARN of the environment owner. This can be ARN of any AWS IAM principal. Defaults to the environment’s creator.</li>
<li><strong>subnet_id</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The ID of the subnet in Amazon VPC that AWS Cloud9 will use to communicate with the Amazon EC2 instance.</li>
</ul>
</td>
</tr>
</tbody>
</table>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-aws/blob/master/website/docs/r/cloud9_environment_ec2.html.markdown">https://github.com/terraform-providers/terraform-provider-aws/blob/master/website/docs/r/cloud9_environment_ec2.html.markdown</a>.</div></blockquote>
<dl class="attribute">
<dt id="pulumi_aws.cloud9.EnvironmentEC2.arn">
<code class="descname">arn</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_aws.cloud9.EnvironmentEC2.arn" title="Permalink to this definition">¶</a></dt>
<dd><p>The ARN of the environment.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_aws.cloud9.EnvironmentEC2.automatic_stop_time_minutes">
<code class="descname">automatic_stop_time_minutes</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_aws.cloud9.EnvironmentEC2.automatic_stop_time_minutes" title="Permalink to this definition">¶</a></dt>
<dd><p>The number of minutes until the running instance is shut down after the environment has last been used.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_aws.cloud9.EnvironmentEC2.description">
<code class="descname">description</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_aws.cloud9.EnvironmentEC2.description" title="Permalink to this definition">¶</a></dt>
<dd><p>The description of the environment.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_aws.cloud9.EnvironmentEC2.instance_type">
<code class="descname">instance_type</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_aws.cloud9.EnvironmentEC2.instance_type" title="Permalink to this definition">¶</a></dt>
<dd><p>The type of instance to connect to the environment, e.g. <code class="docutils literal notranslate"><span class="pre">t2.micro</span></code>.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_aws.cloud9.EnvironmentEC2.name">
<code class="descname">name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_aws.cloud9.EnvironmentEC2.name" title="Permalink to this definition">¶</a></dt>
<dd><p>The name of the environment.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_aws.cloud9.EnvironmentEC2.owner_arn">
<code class="descname">owner_arn</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_aws.cloud9.EnvironmentEC2.owner_arn" title="Permalink to this definition">¶</a></dt>
<dd><p>The ARN of the environment owner. This can be ARN of any AWS IAM principal. Defaults to the environment’s creator.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_aws.cloud9.EnvironmentEC2.subnet_id">
<code class="descname">subnet_id</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_aws.cloud9.EnvironmentEC2.subnet_id" title="Permalink to this definition">¶</a></dt>
<dd><p>The ID of the subnet in Amazon VPC that AWS Cloud9 will use to communicate with the Amazon EC2 instance.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_aws.cloud9.EnvironmentEC2.type">
<code class="descname">type</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_aws.cloud9.EnvironmentEC2.type" title="Permalink to this definition">¶</a></dt>
<dd><p>The type of the environment (e.g. <code class="docutils literal notranslate"><span class="pre">ssh</span></code> or <code class="docutils literal notranslate"><span class="pre">ec2</span></code>)</p>
</dd></dl>

<dl class="staticmethod">
<dt id="pulumi_aws.cloud9.EnvironmentEC2.get">
<em class="property">static </em><code class="descname">get</code><span class="sig-paren">(</span><em>resource_name</em>, <em>id</em>, <em>opts=None</em>, <em>arn=None</em>, <em>automatic_stop_time_minutes=None</em>, <em>description=None</em>, <em>instance_type=None</em>, <em>name=None</em>, <em>owner_arn=None</em>, <em>subnet_id=None</em>, <em>type=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_aws.cloud9.EnvironmentEC2.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing EnvironmentEC2 resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.
:param str resource_name: The unique name of the resulting resource.
:param str id: The unique provider ID of the resource to lookup.
:param pulumi.ResourceOptions opts: Options for the resource.
:param pulumi.Input[str] arn: The ARN of the environment.
:param pulumi.Input[float] automatic_stop_time_minutes: The number of minutes until the running instance is shut down after the environment has last been used.
:param pulumi.Input[str] description: The description of the environment.
:param pulumi.Input[str] instance_type: The type of instance to connect to the environment, e.g. <code class="docutils literal notranslate"><span class="pre">t2.micro</span></code>.
:param pulumi.Input[str] name: The name of the environment.
:param pulumi.Input[str] owner_arn: The ARN of the environment owner. This can be ARN of any AWS IAM principal. Defaults to the environment’s creator.
:param pulumi.Input[str] subnet_id: The ID of the subnet in Amazon VPC that AWS Cloud9 will use to communicate with the Amazon EC2 instance.
:param pulumi.Input[str] type: The type of the environment (e.g. <code class="docutils literal notranslate"><span class="pre">ssh</span></code> or <code class="docutils literal notranslate"><span class="pre">ec2</span></code>)</p>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-aws/blob/master/website/docs/r/cloud9_environment_ec2.html.markdown">https://github.com/terraform-providers/terraform-provider-aws/blob/master/website/docs/r/cloud9_environment_ec2.html.markdown</a>.</div></blockquote>
</dd></dl>

<dl class="method">
<dt id="pulumi_aws.cloud9.EnvironmentEC2.translate_output_property">
<code class="descname">translate_output_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_aws.cloud9.EnvironmentEC2.translate_output_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_aws.cloud9.EnvironmentEC2.translate_input_property">
<code class="descname">translate_input_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_aws.cloud9.EnvironmentEC2.translate_input_property" title="Permalink to this definition">¶</a></dt>
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
