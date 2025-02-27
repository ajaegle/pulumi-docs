---
title: Module codebuild
---

<div class="section" id="codebuild">
<h1>codebuild<a class="headerlink" href="#codebuild" title="Permalink to this headline">¶</a></h1>
<blockquote>
<div>This provider is a derived work of the <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-aws">Terraform Provider</a> distributed under
<a class="reference external" href="https://www.mozilla.org/en-US/MPL/2.0/">MPL 2.0</a>. If you encounter a bug or missing feature, first check the
<a class="reference external" href="https://github.com/pulumi/pulumi-aws/issues">pulumi/pulumi-aws repo</a>; however, if that doesn’t turn up
anything, please consult the source <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-aws/issues">terraform-providers/terraform-provider-aws repo</a>.</div></blockquote>
<span class="target" id="module-pulumi_aws.codebuild"></span><dl class="class">
<dt id="pulumi_aws.codebuild.Project">
<em class="property">class </em><code class="descclassname">pulumi_aws.codebuild.</code><code class="descname">Project</code><span class="sig-paren">(</span><em>resource_name</em>, <em>opts=None</em>, <em>artifacts=None</em>, <em>badge_enabled=None</em>, <em>build_timeout=None</em>, <em>cache=None</em>, <em>description=None</em>, <em>encryption_key=None</em>, <em>environment=None</em>, <em>logs_config=None</em>, <em>name=None</em>, <em>secondary_artifacts=None</em>, <em>secondary_sources=None</em>, <em>service_role=None</em>, <em>source=None</em>, <em>tags=None</em>, <em>vpc_config=None</em>, <em>__props__=None</em>, <em>__name__=None</em>, <em>__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_aws.codebuild.Project" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides a CodeBuild Project resource. See also the <cite>``codebuild.Webhook`</cite> resource &lt;<a class="reference external" href="https://www.terraform.io/docs/providers/aws/r/codebuild_webhook.html">https://www.terraform.io/docs/providers/aws/r/codebuild_webhook.html</a>&gt;`_, which manages the webhook to the source (e.g. the “rebuild every time a code change is pushed” option in the CodeBuild web console).</p>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><ul class="first last simple">
<li><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</li>
<li><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</li>
<li><strong>artifacts</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – Information about the project’s build output artifacts. Artifact blocks are documented below.</li>
<li><strong>badge_enabled</strong> (<em>pulumi.Input</em><em>[</em><em>bool</em><em>]</em>) – Generates a publicly-accessible URL for the projects build badge. Available as <code class="docutils literal notranslate"><span class="pre">badge_url</span></code> attribute when enabled.</li>
<li><strong>build_timeout</strong> (<em>pulumi.Input</em><em>[</em><em>float</em><em>]</em>) – How long in minutes, from 5 to 480 (8 hours), for AWS CodeBuild to wait until timing out any related build that does not get marked as completed. The default is 60 minutes.</li>
<li><strong>cache</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – Information about the cache storage for the project. Cache blocks are documented below.</li>
<li><strong>description</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – A short description of the project.</li>
<li><strong>encryption_key</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The AWS Key Management Service (AWS KMS) customer master key (CMK) to be used for encrypting the build project’s build output artifacts.</li>
<li><strong>environment</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – Information about the project’s build environment. Environment blocks are documented below.</li>
<li><strong>logs_config</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – Configuration for the builds to store log data to CloudWatch or S3.</li>
<li><strong>name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The name of the project. If <code class="docutils literal notranslate"><span class="pre">type</span></code> is set to <code class="docutils literal notranslate"><span class="pre">S3</span></code>, this is the name of the output artifact object</li>
<li><strong>secondary_artifacts</strong> (<em>pulumi.Input</em><em>[</em><em>list</em><em>]</em>) – A set of secondary artifacts to be used inside the build. Secondary artifacts blocks are documented below.</li>
<li><strong>secondary_sources</strong> (<em>pulumi.Input</em><em>[</em><em>list</em><em>]</em>) – A set of secondary sources to be used inside the build. Secondary sources blocks are documented below.</li>
<li><strong>service_role</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The Amazon Resource Name (ARN) of the AWS Identity and Access Management (IAM) role that enables AWS CodeBuild to interact with dependent AWS services on behalf of the AWS account.</li>
<li><strong>source</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – Information about the project’s input source code. Source blocks are documented below.</li>
<li><strong>tags</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A mapping of tags to assign to the resource.</li>
<li><strong>vpc_config</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – Configuration for the builds to run inside a VPC. VPC config blocks are documented below.</li>
</ul>
</td>
</tr>
</tbody>
</table>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-aws/blob/master/website/docs/r/codebuild_project.html.markdown">https://github.com/terraform-providers/terraform-provider-aws/blob/master/website/docs/r/codebuild_project.html.markdown</a>.</div></blockquote>
<dl class="attribute">
<dt id="pulumi_aws.codebuild.Project.arn">
<code class="descname">arn</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_aws.codebuild.Project.arn" title="Permalink to this definition">¶</a></dt>
<dd><p>The ARN of the CodeBuild project.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_aws.codebuild.Project.artifacts">
<code class="descname">artifacts</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_aws.codebuild.Project.artifacts" title="Permalink to this definition">¶</a></dt>
<dd><p>Information about the project’s build output artifacts. Artifact blocks are documented below.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_aws.codebuild.Project.badge_enabled">
<code class="descname">badge_enabled</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_aws.codebuild.Project.badge_enabled" title="Permalink to this definition">¶</a></dt>
<dd><p>Generates a publicly-accessible URL for the projects build badge. Available as <code class="docutils literal notranslate"><span class="pre">badge_url</span></code> attribute when enabled.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_aws.codebuild.Project.badge_url">
<code class="descname">badge_url</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_aws.codebuild.Project.badge_url" title="Permalink to this definition">¶</a></dt>
<dd><p>The URL of the build badge when <code class="docutils literal notranslate"><span class="pre">badge_enabled</span></code> is enabled.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_aws.codebuild.Project.build_timeout">
<code class="descname">build_timeout</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_aws.codebuild.Project.build_timeout" title="Permalink to this definition">¶</a></dt>
<dd><p>How long in minutes, from 5 to 480 (8 hours), for AWS CodeBuild to wait until timing out any related build that does not get marked as completed. The default is 60 minutes.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_aws.codebuild.Project.cache">
<code class="descname">cache</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_aws.codebuild.Project.cache" title="Permalink to this definition">¶</a></dt>
<dd><p>Information about the cache storage for the project. Cache blocks are documented below.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_aws.codebuild.Project.description">
<code class="descname">description</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_aws.codebuild.Project.description" title="Permalink to this definition">¶</a></dt>
<dd><p>A short description of the project.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_aws.codebuild.Project.encryption_key">
<code class="descname">encryption_key</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_aws.codebuild.Project.encryption_key" title="Permalink to this definition">¶</a></dt>
<dd><p>The AWS Key Management Service (AWS KMS) customer master key (CMK) to be used for encrypting the build project’s build output artifacts.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_aws.codebuild.Project.environment">
<code class="descname">environment</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_aws.codebuild.Project.environment" title="Permalink to this definition">¶</a></dt>
<dd><p>Information about the project’s build environment. Environment blocks are documented below.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_aws.codebuild.Project.logs_config">
<code class="descname">logs_config</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_aws.codebuild.Project.logs_config" title="Permalink to this definition">¶</a></dt>
<dd><p>Configuration for the builds to store log data to CloudWatch or S3.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_aws.codebuild.Project.name">
<code class="descname">name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_aws.codebuild.Project.name" title="Permalink to this definition">¶</a></dt>
<dd><p>The name of the project. If <code class="docutils literal notranslate"><span class="pre">type</span></code> is set to <code class="docutils literal notranslate"><span class="pre">S3</span></code>, this is the name of the output artifact object</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_aws.codebuild.Project.secondary_artifacts">
<code class="descname">secondary_artifacts</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_aws.codebuild.Project.secondary_artifacts" title="Permalink to this definition">¶</a></dt>
<dd><p>A set of secondary artifacts to be used inside the build. Secondary artifacts blocks are documented below.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_aws.codebuild.Project.secondary_sources">
<code class="descname">secondary_sources</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_aws.codebuild.Project.secondary_sources" title="Permalink to this definition">¶</a></dt>
<dd><p>A set of secondary sources to be used inside the build. Secondary sources blocks are documented below.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_aws.codebuild.Project.service_role">
<code class="descname">service_role</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_aws.codebuild.Project.service_role" title="Permalink to this definition">¶</a></dt>
<dd><p>The Amazon Resource Name (ARN) of the AWS Identity and Access Management (IAM) role that enables AWS CodeBuild to interact with dependent AWS services on behalf of the AWS account.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_aws.codebuild.Project.source">
<code class="descname">source</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_aws.codebuild.Project.source" title="Permalink to this definition">¶</a></dt>
<dd><p>Information about the project’s input source code. Source blocks are documented below.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_aws.codebuild.Project.tags">
<code class="descname">tags</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_aws.codebuild.Project.tags" title="Permalink to this definition">¶</a></dt>
<dd><p>A mapping of tags to assign to the resource.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_aws.codebuild.Project.vpc_config">
<code class="descname">vpc_config</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_aws.codebuild.Project.vpc_config" title="Permalink to this definition">¶</a></dt>
<dd><p>Configuration for the builds to run inside a VPC. VPC config blocks are documented below.</p>
</dd></dl>

<dl class="staticmethod">
<dt id="pulumi_aws.codebuild.Project.get">
<em class="property">static </em><code class="descname">get</code><span class="sig-paren">(</span><em>resource_name</em>, <em>id</em>, <em>opts=None</em>, <em>arn=None</em>, <em>artifacts=None</em>, <em>badge_enabled=None</em>, <em>badge_url=None</em>, <em>build_timeout=None</em>, <em>cache=None</em>, <em>description=None</em>, <em>encryption_key=None</em>, <em>environment=None</em>, <em>logs_config=None</em>, <em>name=None</em>, <em>secondary_artifacts=None</em>, <em>secondary_sources=None</em>, <em>service_role=None</em>, <em>source=None</em>, <em>tags=None</em>, <em>vpc_config=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_aws.codebuild.Project.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing Project resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.
:param str resource_name: The unique name of the resulting resource.
:param str id: The unique provider ID of the resource to lookup.
:param pulumi.ResourceOptions opts: Options for the resource.
:param pulumi.Input[str] arn: The ARN of the CodeBuild project.
:param pulumi.Input[dict] artifacts: Information about the project’s build output artifacts. Artifact blocks are documented below.
:param pulumi.Input[bool] badge_enabled: Generates a publicly-accessible URL for the projects build badge. Available as <code class="docutils literal notranslate"><span class="pre">badge_url</span></code> attribute when enabled.
:param pulumi.Input[str] badge_url: The URL of the build badge when <code class="docutils literal notranslate"><span class="pre">badge_enabled</span></code> is enabled.
:param pulumi.Input[float] build_timeout: How long in minutes, from 5 to 480 (8 hours), for AWS CodeBuild to wait until timing out any related build that does not get marked as completed. The default is 60 minutes.
:param pulumi.Input[dict] cache: Information about the cache storage for the project. Cache blocks are documented below.
:param pulumi.Input[str] description: A short description of the project.
:param pulumi.Input[str] encryption_key: The AWS Key Management Service (AWS KMS) customer master key (CMK) to be used for encrypting the build project’s build output artifacts.
:param pulumi.Input[dict] environment: Information about the project’s build environment. Environment blocks are documented below.
:param pulumi.Input[dict] logs_config: Configuration for the builds to store log data to CloudWatch or S3.
:param pulumi.Input[str] name: The name of the project. If <code class="docutils literal notranslate"><span class="pre">type</span></code> is set to <code class="docutils literal notranslate"><span class="pre">S3</span></code>, this is the name of the output artifact object
:param pulumi.Input[list] secondary_artifacts: A set of secondary artifacts to be used inside the build. Secondary artifacts blocks are documented below.
:param pulumi.Input[list] secondary_sources: A set of secondary sources to be used inside the build. Secondary sources blocks are documented below.
:param pulumi.Input[str] service_role: The Amazon Resource Name (ARN) of the AWS Identity and Access Management (IAM) role that enables AWS CodeBuild to interact with dependent AWS services on behalf of the AWS account.
:param pulumi.Input[dict] source: Information about the project’s input source code. Source blocks are documented below.
:param pulumi.Input[dict] tags: A mapping of tags to assign to the resource.
:param pulumi.Input[dict] vpc_config: Configuration for the builds to run inside a VPC. VPC config blocks are documented below.</p>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-aws/blob/master/website/docs/r/codebuild_project.html.markdown">https://github.com/terraform-providers/terraform-provider-aws/blob/master/website/docs/r/codebuild_project.html.markdown</a>.</div></blockquote>
</dd></dl>

<dl class="method">
<dt id="pulumi_aws.codebuild.Project.translate_output_property">
<code class="descname">translate_output_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_aws.codebuild.Project.translate_output_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_aws.codebuild.Project.translate_input_property">
<code class="descname">translate_input_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_aws.codebuild.Project.translate_input_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_aws.codebuild.SourceCredential">
<em class="property">class </em><code class="descclassname">pulumi_aws.codebuild.</code><code class="descname">SourceCredential</code><span class="sig-paren">(</span><em>resource_name</em>, <em>opts=None</em>, <em>auth_type=None</em>, <em>server_type=None</em>, <em>token=None</em>, <em>user_name=None</em>, <em>__props__=None</em>, <em>__name__=None</em>, <em>__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_aws.codebuild.SourceCredential" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides a CodeBuild Source Credentials Resource.</p>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><ul class="first last simple">
<li><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</li>
<li><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</li>
<li><strong>auth_type</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The type of authentication used to connect to a GitHub, GitHub Enterprise, or Bitbucket repository. An OAUTH connection is not supported by the API.</li>
<li><strong>server_type</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The source provider used for this project.</li>
<li><strong>token</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – For <code class="docutils literal notranslate"><span class="pre">GitHub</span></code> or <code class="docutils literal notranslate"><span class="pre">GitHub</span> <span class="pre">Enterprise</span></code>, this is the personal access token. For <code class="docutils literal notranslate"><span class="pre">Bitbucket</span></code>, this is the app password.</li>
<li><strong>user_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The Bitbucket username when the authType is <code class="docutils literal notranslate"><span class="pre">BASIC_AUTH</span></code>. This parameter is not valid for other types of source providers or connections.</li>
</ul>
</td>
</tr>
</tbody>
</table>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-aws/blob/master/website/docs/r/codebuild_source_credential.html.markdown">https://github.com/terraform-providers/terraform-provider-aws/blob/master/website/docs/r/codebuild_source_credential.html.markdown</a>.</div></blockquote>
<dl class="attribute">
<dt id="pulumi_aws.codebuild.SourceCredential.arn">
<code class="descname">arn</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_aws.codebuild.SourceCredential.arn" title="Permalink to this definition">¶</a></dt>
<dd><p>The ARN of Source Credential.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_aws.codebuild.SourceCredential.auth_type">
<code class="descname">auth_type</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_aws.codebuild.SourceCredential.auth_type" title="Permalink to this definition">¶</a></dt>
<dd><p>The type of authentication used to connect to a GitHub, GitHub Enterprise, or Bitbucket repository. An OAUTH connection is not supported by the API.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_aws.codebuild.SourceCredential.server_type">
<code class="descname">server_type</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_aws.codebuild.SourceCredential.server_type" title="Permalink to this definition">¶</a></dt>
<dd><p>The source provider used for this project.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_aws.codebuild.SourceCredential.token">
<code class="descname">token</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_aws.codebuild.SourceCredential.token" title="Permalink to this definition">¶</a></dt>
<dd><p>For <code class="docutils literal notranslate"><span class="pre">GitHub</span></code> or <code class="docutils literal notranslate"><span class="pre">GitHub</span> <span class="pre">Enterprise</span></code>, this is the personal access token. For <code class="docutils literal notranslate"><span class="pre">Bitbucket</span></code>, this is the app password.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_aws.codebuild.SourceCredential.user_name">
<code class="descname">user_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_aws.codebuild.SourceCredential.user_name" title="Permalink to this definition">¶</a></dt>
<dd><p>The Bitbucket username when the authType is <code class="docutils literal notranslate"><span class="pre">BASIC_AUTH</span></code>. This parameter is not valid for other types of source providers or connections.</p>
</dd></dl>

<dl class="staticmethod">
<dt id="pulumi_aws.codebuild.SourceCredential.get">
<em class="property">static </em><code class="descname">get</code><span class="sig-paren">(</span><em>resource_name</em>, <em>id</em>, <em>opts=None</em>, <em>arn=None</em>, <em>auth_type=None</em>, <em>server_type=None</em>, <em>token=None</em>, <em>user_name=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_aws.codebuild.SourceCredential.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing SourceCredential resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.
:param str resource_name: The unique name of the resulting resource.
:param str id: The unique provider ID of the resource to lookup.
:param pulumi.ResourceOptions opts: Options for the resource.
:param pulumi.Input[str] arn: The ARN of Source Credential.
:param pulumi.Input[str] auth_type: The type of authentication used to connect to a GitHub, GitHub Enterprise, or Bitbucket repository. An OAUTH connection is not supported by the API.
:param pulumi.Input[str] server_type: The source provider used for this project.
:param pulumi.Input[str] token: For <code class="docutils literal notranslate"><span class="pre">GitHub</span></code> or <code class="docutils literal notranslate"><span class="pre">GitHub</span> <span class="pre">Enterprise</span></code>, this is the personal access token. For <code class="docutils literal notranslate"><span class="pre">Bitbucket</span></code>, this is the app password.
:param pulumi.Input[str] user_name: The Bitbucket username when the authType is <code class="docutils literal notranslate"><span class="pre">BASIC_AUTH</span></code>. This parameter is not valid for other types of source providers or connections.</p>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-aws/blob/master/website/docs/r/codebuild_source_credential.html.markdown">https://github.com/terraform-providers/terraform-provider-aws/blob/master/website/docs/r/codebuild_source_credential.html.markdown</a>.</div></blockquote>
</dd></dl>

<dl class="method">
<dt id="pulumi_aws.codebuild.SourceCredential.translate_output_property">
<code class="descname">translate_output_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_aws.codebuild.SourceCredential.translate_output_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_aws.codebuild.SourceCredential.translate_input_property">
<code class="descname">translate_input_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_aws.codebuild.SourceCredential.translate_input_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_aws.codebuild.Webhook">
<em class="property">class </em><code class="descclassname">pulumi_aws.codebuild.</code><code class="descname">Webhook</code><span class="sig-paren">(</span><em>resource_name</em>, <em>opts=None</em>, <em>branch_filter=None</em>, <em>filter_groups=None</em>, <em>project_name=None</em>, <em>__props__=None</em>, <em>__name__=None</em>, <em>__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_aws.codebuild.Webhook" title="Permalink to this definition">¶</a></dt>
<dd><p>Manages a CodeBuild webhook, which is an endpoint accepted by the CodeBuild service to trigger builds from source code repositories. Depending on the source type of the CodeBuild project, the CodeBuild service may also automatically create and delete the actual repository webhook as well.</p>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><ul class="first last simple">
<li><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</li>
<li><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</li>
<li><strong>branch_filter</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – A regular expression used to determine which branches get built. Default is all branches are built. It is recommended to use <code class="docutils literal notranslate"><span class="pre">filter_group</span></code> over <code class="docutils literal notranslate"><span class="pre">branch_filter</span></code>.</li>
<li><strong>filter_groups</strong> (<em>pulumi.Input</em><em>[</em><em>list</em><em>]</em>) – Information about the webhook’s trigger. Filter group blocks are documented below.</li>
<li><strong>project_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The name of the build project.</li>
</ul>
</td>
</tr>
</tbody>
</table>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-aws/blob/master/website/docs/r/codebuild_webhook.html.markdown">https://github.com/terraform-providers/terraform-provider-aws/blob/master/website/docs/r/codebuild_webhook.html.markdown</a>.</div></blockquote>
<dl class="attribute">
<dt id="pulumi_aws.codebuild.Webhook.branch_filter">
<code class="descname">branch_filter</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_aws.codebuild.Webhook.branch_filter" title="Permalink to this definition">¶</a></dt>
<dd><p>A regular expression used to determine which branches get built. Default is all branches are built. It is recommended to use <code class="docutils literal notranslate"><span class="pre">filter_group</span></code> over <code class="docutils literal notranslate"><span class="pre">branch_filter</span></code>.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_aws.codebuild.Webhook.filter_groups">
<code class="descname">filter_groups</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_aws.codebuild.Webhook.filter_groups" title="Permalink to this definition">¶</a></dt>
<dd><p>Information about the webhook’s trigger. Filter group blocks are documented below.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_aws.codebuild.Webhook.payload_url">
<code class="descname">payload_url</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_aws.codebuild.Webhook.payload_url" title="Permalink to this definition">¶</a></dt>
<dd><p>The CodeBuild endpoint where webhook events are sent.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_aws.codebuild.Webhook.project_name">
<code class="descname">project_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_aws.codebuild.Webhook.project_name" title="Permalink to this definition">¶</a></dt>
<dd><p>The name of the build project.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_aws.codebuild.Webhook.secret">
<code class="descname">secret</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_aws.codebuild.Webhook.secret" title="Permalink to this definition">¶</a></dt>
<dd><p>The secret token of the associated repository. Not returned by the CodeBuild API for all source types.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_aws.codebuild.Webhook.url">
<code class="descname">url</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_aws.codebuild.Webhook.url" title="Permalink to this definition">¶</a></dt>
<dd><p>The URL to the webhook.</p>
</dd></dl>

<dl class="staticmethod">
<dt id="pulumi_aws.codebuild.Webhook.get">
<em class="property">static </em><code class="descname">get</code><span class="sig-paren">(</span><em>resource_name</em>, <em>id</em>, <em>opts=None</em>, <em>branch_filter=None</em>, <em>filter_groups=None</em>, <em>payload_url=None</em>, <em>project_name=None</em>, <em>secret=None</em>, <em>url=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_aws.codebuild.Webhook.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing Webhook resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.
:param str resource_name: The unique name of the resulting resource.
:param str id: The unique provider ID of the resource to lookup.
:param pulumi.ResourceOptions opts: Options for the resource.
:param pulumi.Input[str] branch_filter: A regular expression used to determine which branches get built. Default is all branches are built. It is recommended to use <code class="docutils literal notranslate"><span class="pre">filter_group</span></code> over <code class="docutils literal notranslate"><span class="pre">branch_filter</span></code>.
:param pulumi.Input[list] filter_groups: Information about the webhook’s trigger. Filter group blocks are documented below.
:param pulumi.Input[str] payload_url: The CodeBuild endpoint where webhook events are sent.
:param pulumi.Input[str] project_name: The name of the build project.
:param pulumi.Input[str] secret: The secret token of the associated repository. Not returned by the CodeBuild API for all source types.
:param pulumi.Input[str] url: The URL to the webhook.</p>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-aws/blob/master/website/docs/r/codebuild_webhook.html.markdown">https://github.com/terraform-providers/terraform-provider-aws/blob/master/website/docs/r/codebuild_webhook.html.markdown</a>.</div></blockquote>
</dd></dl>

<dl class="method">
<dt id="pulumi_aws.codebuild.Webhook.translate_output_property">
<code class="descname">translate_output_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_aws.codebuild.Webhook.translate_output_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_aws.codebuild.Webhook.translate_input_property">
<code class="descname">translate_input_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_aws.codebuild.Webhook.translate_input_property" title="Permalink to this definition">¶</a></dt>
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
