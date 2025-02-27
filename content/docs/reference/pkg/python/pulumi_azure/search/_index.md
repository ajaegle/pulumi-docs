---
title: Module search
---

<div class="section" id="search">
<h1>search<a class="headerlink" href="#search" title="Permalink to this headline">¶</a></h1>
<blockquote>
<div>This provider is a derived work of the <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm">Terraform Provider</a> distributed under
<a class="reference external" href="https://www.mozilla.org/en-US/MPL/2.0/">MPL 2.0</a>. If you encounter a bug or missing feature, first check the
<a class="reference external" href="https://github.com/pulumi/pulumi-azure/issues">pulumi/pulumi-azure repo</a>; however, if that doesn’t turn up
anything, please consult the source <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/issues">terraform-providers/terraform-provider-azurerm repo</a>.</div></blockquote>
<span class="target" id="module-pulumi_azure.search"></span><dl class="class">
<dt id="pulumi_azure.search.Service">
<em class="property">class </em><code class="descclassname">pulumi_azure.search.</code><code class="descname">Service</code><span class="sig-paren">(</span><em>resource_name</em>, <em>opts=None</em>, <em>location=None</em>, <em>name=None</em>, <em>partition_count=None</em>, <em>replica_count=None</em>, <em>resource_group_name=None</em>, <em>sku=None</em>, <em>tags=None</em>, <em>__props__=None</em>, <em>__name__=None</em>, <em>__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.search.Service" title="Permalink to this definition">¶</a></dt>
<dd><p>Allows you to manage an Azure Search Service.</p>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><ul class="first last simple">
<li><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</li>
<li><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</li>
<li><strong>location</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Specifies the supported Azure location where the resource exists. Changing this forces a new resource to be created.</li>
<li><strong>name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The name of the Search Service. Changing this forces a new resource to be created.</li>
<li><strong>partition_count</strong> (<em>pulumi.Input</em><em>[</em><em>float</em><em>]</em>) – Default is 1. Valid values include 1, 2, 3, 4, 6, or 12. Valid only when <code class="docutils literal notranslate"><span class="pre">sku</span></code> is <code class="docutils literal notranslate"><span class="pre">standard</span></code>. Changing this forces a new resource to be created.</li>
<li><strong>replica_count</strong> (<em>pulumi.Input</em><em>[</em><em>float</em><em>]</em>) – Default is 1. Valid values include 1 through 12. Valid only when <code class="docutils literal notranslate"><span class="pre">sku</span></code> is <code class="docutils literal notranslate"><span class="pre">standard</span></code>. Changing this forces a new resource to be created.</li>
<li><strong>resource_group_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The name of the resource group in which to create the Search Service. Changing this forces a new resource to be created.</li>
<li><strong>sku</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Valid values are <code class="docutils literal notranslate"><span class="pre">free</span></code> and <code class="docutils literal notranslate"><span class="pre">standard</span></code>. <code class="docutils literal notranslate"><span class="pre">standard2</span></code> and <code class="docutils literal notranslate"><span class="pre">standard3</span></code> are also valid, but can only be used when it’s enabled on the backend by Microsoft support. <code class="docutils literal notranslate"><span class="pre">free</span></code> provisions the service in shared clusters. <code class="docutils literal notranslate"><span class="pre">standard</span></code> provisions the service in dedicated clusters.  Changing this forces a new resource to be created.</li>
<li><strong>tags</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A mapping of tags to assign to the resource.</li>
</ul>
</td>
</tr>
</tbody>
</table>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/search_service.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/search_service.html.markdown</a>.</div></blockquote>
<dl class="attribute">
<dt id="pulumi_azure.search.Service.location">
<code class="descname">location</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.search.Service.location" title="Permalink to this definition">¶</a></dt>
<dd><p>Specifies the supported Azure location where the resource exists. Changing this forces a new resource to be created.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.search.Service.name">
<code class="descname">name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.search.Service.name" title="Permalink to this definition">¶</a></dt>
<dd><p>The name of the Search Service. Changing this forces a new resource to be created.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.search.Service.partition_count">
<code class="descname">partition_count</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.search.Service.partition_count" title="Permalink to this definition">¶</a></dt>
<dd><p>Default is 1. Valid values include 1, 2, 3, 4, 6, or 12. Valid only when <code class="docutils literal notranslate"><span class="pre">sku</span></code> is <code class="docutils literal notranslate"><span class="pre">standard</span></code>. Changing this forces a new resource to be created.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.search.Service.primary_key">
<code class="descname">primary_key</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.search.Service.primary_key" title="Permalink to this definition">¶</a></dt>
<dd><p>The Search Service Administration primary key.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.search.Service.replica_count">
<code class="descname">replica_count</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.search.Service.replica_count" title="Permalink to this definition">¶</a></dt>
<dd><p>Default is 1. Valid values include 1 through 12. Valid only when <code class="docutils literal notranslate"><span class="pre">sku</span></code> is <code class="docutils literal notranslate"><span class="pre">standard</span></code>. Changing this forces a new resource to be created.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.search.Service.resource_group_name">
<code class="descname">resource_group_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.search.Service.resource_group_name" title="Permalink to this definition">¶</a></dt>
<dd><p>The name of the resource group in which to create the Search Service. Changing this forces a new resource to be created.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.search.Service.secondary_key">
<code class="descname">secondary_key</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.search.Service.secondary_key" title="Permalink to this definition">¶</a></dt>
<dd><p>The Search Service Administration secondary key.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.search.Service.sku">
<code class="descname">sku</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.search.Service.sku" title="Permalink to this definition">¶</a></dt>
<dd><p>Valid values are <code class="docutils literal notranslate"><span class="pre">free</span></code> and <code class="docutils literal notranslate"><span class="pre">standard</span></code>. <code class="docutils literal notranslate"><span class="pre">standard2</span></code> and <code class="docutils literal notranslate"><span class="pre">standard3</span></code> are also valid, but can only be used when it’s enabled on the backend by Microsoft support. <code class="docutils literal notranslate"><span class="pre">free</span></code> provisions the service in shared clusters. <code class="docutils literal notranslate"><span class="pre">standard</span></code> provisions the service in dedicated clusters.  Changing this forces a new resource to be created.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.search.Service.tags">
<code class="descname">tags</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.search.Service.tags" title="Permalink to this definition">¶</a></dt>
<dd><p>A mapping of tags to assign to the resource.</p>
</dd></dl>

<dl class="staticmethod">
<dt id="pulumi_azure.search.Service.get">
<em class="property">static </em><code class="descname">get</code><span class="sig-paren">(</span><em>resource_name</em>, <em>id</em>, <em>opts=None</em>, <em>location=None</em>, <em>name=None</em>, <em>partition_count=None</em>, <em>primary_key=None</em>, <em>replica_count=None</em>, <em>resource_group_name=None</em>, <em>secondary_key=None</em>, <em>sku=None</em>, <em>tags=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.search.Service.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing Service resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.
:param str resource_name: The unique name of the resulting resource.
:param str id: The unique provider ID of the resource to lookup.
:param pulumi.ResourceOptions opts: Options for the resource.
:param pulumi.Input[str] location: Specifies the supported Azure location where the resource exists. Changing this forces a new resource to be created.
:param pulumi.Input[str] name: The name of the Search Service. Changing this forces a new resource to be created.
:param pulumi.Input[float] partition_count: Default is 1. Valid values include 1, 2, 3, 4, 6, or 12. Valid only when <code class="docutils literal notranslate"><span class="pre">sku</span></code> is <code class="docutils literal notranslate"><span class="pre">standard</span></code>. Changing this forces a new resource to be created.
:param pulumi.Input[str] primary_key: The Search Service Administration primary key.
:param pulumi.Input[float] replica_count: Default is 1. Valid values include 1 through 12. Valid only when <code class="docutils literal notranslate"><span class="pre">sku</span></code> is <code class="docutils literal notranslate"><span class="pre">standard</span></code>. Changing this forces a new resource to be created.
:param pulumi.Input[str] resource_group_name: The name of the resource group in which to create the Search Service. Changing this forces a new resource to be created.
:param pulumi.Input[str] secondary_key: The Search Service Administration secondary key.
:param pulumi.Input[str] sku: Valid values are <code class="docutils literal notranslate"><span class="pre">free</span></code> and <code class="docutils literal notranslate"><span class="pre">standard</span></code>. <code class="docutils literal notranslate"><span class="pre">standard2</span></code> and <code class="docutils literal notranslate"><span class="pre">standard3</span></code> are also valid, but can only be used when it’s enabled on the backend by Microsoft support. <code class="docutils literal notranslate"><span class="pre">free</span></code> provisions the service in shared clusters. <code class="docutils literal notranslate"><span class="pre">standard</span></code> provisions the service in dedicated clusters.  Changing this forces a new resource to be created.
:param pulumi.Input[dict] tags: A mapping of tags to assign to the resource.</p>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/search_service.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/search_service.html.markdown</a>.</div></blockquote>
</dd></dl>

<dl class="method">
<dt id="pulumi_azure.search.Service.translate_output_property">
<code class="descname">translate_output_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.search.Service.translate_output_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_azure.search.Service.translate_input_property">
<code class="descname">translate_input_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.search.Service.translate_input_property" title="Permalink to this definition">¶</a></dt>
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
