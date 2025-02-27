---
title: Module dns
---

<div class="section" id="dns">
<h1>dns<a class="headerlink" href="#dns" title="Permalink to this headline">¶</a></h1>
<blockquote>
<div>This provider is a derived work of the <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm">Terraform Provider</a> distributed under
<a class="reference external" href="https://www.mozilla.org/en-US/MPL/2.0/">MPL 2.0</a>. If you encounter a bug or missing feature, first check the
<a class="reference external" href="https://github.com/pulumi/pulumi-azure/issues">pulumi/pulumi-azure repo</a>; however, if that doesn’t turn up
anything, please consult the source <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/issues">terraform-providers/terraform-provider-azurerm repo</a>.</div></blockquote>
<span class="target" id="module-pulumi_azure.dns"></span><dl class="class">
<dt id="pulumi_azure.dns.ARecord">
<em class="property">class </em><code class="descclassname">pulumi_azure.dns.</code><code class="descname">ARecord</code><span class="sig-paren">(</span><em>resource_name</em>, <em>opts=None</em>, <em>name=None</em>, <em>records=None</em>, <em>resource_group_name=None</em>, <em>tags=None</em>, <em>ttl=None</em>, <em>zone_name=None</em>, <em>__props__=None</em>, <em>__name__=None</em>, <em>__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.dns.ARecord" title="Permalink to this definition">¶</a></dt>
<dd><p>Enables you to manage DNS A Records within Azure DNS.</p>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><ul class="first last simple">
<li><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</li>
<li><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</li>
<li><strong>name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The name of the DNS A Record.</li>
<li><strong>records</strong> (<em>pulumi.Input</em><em>[</em><em>list</em><em>]</em>) – List of IPv4 Addresses.</li>
<li><strong>resource_group_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Specifies the resource group where the resource exists. Changing this forces a new resource to be created.</li>
<li><strong>tags</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A mapping of tags to assign to the resource.</li>
<li><strong>zone_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Specifies the DNS Zone where the resource exists. Changing this forces a new resource to be created.</li>
</ul>
</td>
</tr>
</tbody>
</table>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/dns_a_record.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/dns_a_record.html.markdown</a>.</div></blockquote>
<dl class="attribute">
<dt id="pulumi_azure.dns.ARecord.name">
<code class="descname">name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.ARecord.name" title="Permalink to this definition">¶</a></dt>
<dd><p>The name of the DNS A Record.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.dns.ARecord.records">
<code class="descname">records</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.ARecord.records" title="Permalink to this definition">¶</a></dt>
<dd><p>List of IPv4 Addresses.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.dns.ARecord.resource_group_name">
<code class="descname">resource_group_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.ARecord.resource_group_name" title="Permalink to this definition">¶</a></dt>
<dd><p>Specifies the resource group where the resource exists. Changing this forces a new resource to be created.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.dns.ARecord.tags">
<code class="descname">tags</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.ARecord.tags" title="Permalink to this definition">¶</a></dt>
<dd><p>A mapping of tags to assign to the resource.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.dns.ARecord.zone_name">
<code class="descname">zone_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.ARecord.zone_name" title="Permalink to this definition">¶</a></dt>
<dd><p>Specifies the DNS Zone where the resource exists. Changing this forces a new resource to be created.</p>
</dd></dl>

<dl class="staticmethod">
<dt id="pulumi_azure.dns.ARecord.get">
<em class="property">static </em><code class="descname">get</code><span class="sig-paren">(</span><em>resource_name</em>, <em>id</em>, <em>opts=None</em>, <em>name=None</em>, <em>records=None</em>, <em>resource_group_name=None</em>, <em>tags=None</em>, <em>ttl=None</em>, <em>zone_name=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.dns.ARecord.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing ARecord resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.
:param str resource_name: The unique name of the resulting resource.
:param str id: The unique provider ID of the resource to lookup.
:param pulumi.ResourceOptions opts: Options for the resource.
:param pulumi.Input[str] name: The name of the DNS A Record.
:param pulumi.Input[list] records: List of IPv4 Addresses.
:param pulumi.Input[str] resource_group_name: Specifies the resource group where the resource exists. Changing this forces a new resource to be created.
:param pulumi.Input[dict] tags: A mapping of tags to assign to the resource.
:param pulumi.Input[str] zone_name: Specifies the DNS Zone where the resource exists. Changing this forces a new resource to be created.</p>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/dns_a_record.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/dns_a_record.html.markdown</a>.</div></blockquote>
</dd></dl>

<dl class="method">
<dt id="pulumi_azure.dns.ARecord.translate_output_property">
<code class="descname">translate_output_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.dns.ARecord.translate_output_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_azure.dns.ARecord.translate_input_property">
<code class="descname">translate_input_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.dns.ARecord.translate_input_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_azure.dns.AaaaRecord">
<em class="property">class </em><code class="descclassname">pulumi_azure.dns.</code><code class="descname">AaaaRecord</code><span class="sig-paren">(</span><em>resource_name</em>, <em>opts=None</em>, <em>name=None</em>, <em>records=None</em>, <em>resource_group_name=None</em>, <em>tags=None</em>, <em>ttl=None</em>, <em>zone_name=None</em>, <em>__props__=None</em>, <em>__name__=None</em>, <em>__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.dns.AaaaRecord" title="Permalink to this definition">¶</a></dt>
<dd><p>Enables you to manage DNS AAAA Records within Azure DNS.</p>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><ul class="first last simple">
<li><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</li>
<li><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</li>
<li><strong>name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The name of the DNS AAAA Record.</li>
<li><strong>records</strong> (<em>pulumi.Input</em><em>[</em><em>list</em><em>]</em>) – List of IPv6 Addresses.</li>
<li><strong>resource_group_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Specifies the resource group where the resource exists. Changing this forces a new resource to be created.</li>
<li><strong>tags</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A mapping of tags to assign to the resource.</li>
<li><strong>zone_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Specifies the DNS Zone where the resource exists. Changing this forces a new resource to be created.</li>
</ul>
</td>
</tr>
</tbody>
</table>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/dns_aaaa_record.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/dns_aaaa_record.html.markdown</a>.</div></blockquote>
<dl class="attribute">
<dt id="pulumi_azure.dns.AaaaRecord.name">
<code class="descname">name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.AaaaRecord.name" title="Permalink to this definition">¶</a></dt>
<dd><p>The name of the DNS AAAA Record.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.dns.AaaaRecord.records">
<code class="descname">records</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.AaaaRecord.records" title="Permalink to this definition">¶</a></dt>
<dd><p>List of IPv6 Addresses.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.dns.AaaaRecord.resource_group_name">
<code class="descname">resource_group_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.AaaaRecord.resource_group_name" title="Permalink to this definition">¶</a></dt>
<dd><p>Specifies the resource group where the resource exists. Changing this forces a new resource to be created.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.dns.AaaaRecord.tags">
<code class="descname">tags</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.AaaaRecord.tags" title="Permalink to this definition">¶</a></dt>
<dd><p>A mapping of tags to assign to the resource.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.dns.AaaaRecord.zone_name">
<code class="descname">zone_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.AaaaRecord.zone_name" title="Permalink to this definition">¶</a></dt>
<dd><p>Specifies the DNS Zone where the resource exists. Changing this forces a new resource to be created.</p>
</dd></dl>

<dl class="staticmethod">
<dt id="pulumi_azure.dns.AaaaRecord.get">
<em class="property">static </em><code class="descname">get</code><span class="sig-paren">(</span><em>resource_name</em>, <em>id</em>, <em>opts=None</em>, <em>name=None</em>, <em>records=None</em>, <em>resource_group_name=None</em>, <em>tags=None</em>, <em>ttl=None</em>, <em>zone_name=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.dns.AaaaRecord.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing AaaaRecord resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.
:param str resource_name: The unique name of the resulting resource.
:param str id: The unique provider ID of the resource to lookup.
:param pulumi.ResourceOptions opts: Options for the resource.
:param pulumi.Input[str] name: The name of the DNS AAAA Record.
:param pulumi.Input[list] records: List of IPv6 Addresses.
:param pulumi.Input[str] resource_group_name: Specifies the resource group where the resource exists. Changing this forces a new resource to be created.
:param pulumi.Input[dict] tags: A mapping of tags to assign to the resource.
:param pulumi.Input[str] zone_name: Specifies the DNS Zone where the resource exists. Changing this forces a new resource to be created.</p>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/dns_aaaa_record.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/dns_aaaa_record.html.markdown</a>.</div></blockquote>
</dd></dl>

<dl class="method">
<dt id="pulumi_azure.dns.AaaaRecord.translate_output_property">
<code class="descname">translate_output_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.dns.AaaaRecord.translate_output_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_azure.dns.AaaaRecord.translate_input_property">
<code class="descname">translate_input_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.dns.AaaaRecord.translate_input_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_azure.dns.AwaitableGetZoneResult">
<em class="property">class </em><code class="descclassname">pulumi_azure.dns.</code><code class="descname">AwaitableGetZoneResult</code><span class="sig-paren">(</span><em>max_number_of_record_sets=None</em>, <em>name=None</em>, <em>name_servers=None</em>, <em>number_of_record_sets=None</em>, <em>registration_virtual_network_ids=None</em>, <em>resolution_virtual_network_ids=None</em>, <em>resource_group_name=None</em>, <em>tags=None</em>, <em>zone_type=None</em>, <em>id=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.dns.AwaitableGetZoneResult" title="Permalink to this definition">¶</a></dt>
<dd></dd></dl>

<dl class="class">
<dt id="pulumi_azure.dns.CNameRecord">
<em class="property">class </em><code class="descclassname">pulumi_azure.dns.</code><code class="descname">CNameRecord</code><span class="sig-paren">(</span><em>resource_name</em>, <em>opts=None</em>, <em>name=None</em>, <em>record=None</em>, <em>resource_group_name=None</em>, <em>tags=None</em>, <em>ttl=None</em>, <em>zone_name=None</em>, <em>__props__=None</em>, <em>__name__=None</em>, <em>__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.dns.CNameRecord" title="Permalink to this definition">¶</a></dt>
<dd><p>Enables you to manage DNS CNAME Records within Azure DNS.</p>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><ul class="first last simple">
<li><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</li>
<li><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</li>
<li><strong>name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The name of the DNS CNAME Record.</li>
<li><strong>record</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The target of the CNAME.</li>
<li><strong>resource_group_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Specifies the resource group where the resource exists. Changing this forces a new resource to be created.</li>
<li><strong>tags</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A mapping of tags to assign to the resource.</li>
<li><strong>zone_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Specifies the DNS Zone where the resource exists. Changing this forces a new resource to be created.</li>
</ul>
</td>
</tr>
</tbody>
</table>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/dns_cname_record.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/dns_cname_record.html.markdown</a>.</div></blockquote>
<dl class="attribute">
<dt id="pulumi_azure.dns.CNameRecord.name">
<code class="descname">name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.CNameRecord.name" title="Permalink to this definition">¶</a></dt>
<dd><p>The name of the DNS CNAME Record.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.dns.CNameRecord.record">
<code class="descname">record</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.CNameRecord.record" title="Permalink to this definition">¶</a></dt>
<dd><p>The target of the CNAME.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.dns.CNameRecord.resource_group_name">
<code class="descname">resource_group_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.CNameRecord.resource_group_name" title="Permalink to this definition">¶</a></dt>
<dd><p>Specifies the resource group where the resource exists. Changing this forces a new resource to be created.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.dns.CNameRecord.tags">
<code class="descname">tags</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.CNameRecord.tags" title="Permalink to this definition">¶</a></dt>
<dd><p>A mapping of tags to assign to the resource.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.dns.CNameRecord.zone_name">
<code class="descname">zone_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.CNameRecord.zone_name" title="Permalink to this definition">¶</a></dt>
<dd><p>Specifies the DNS Zone where the resource exists. Changing this forces a new resource to be created.</p>
</dd></dl>

<dl class="staticmethod">
<dt id="pulumi_azure.dns.CNameRecord.get">
<em class="property">static </em><code class="descname">get</code><span class="sig-paren">(</span><em>resource_name</em>, <em>id</em>, <em>opts=None</em>, <em>name=None</em>, <em>record=None</em>, <em>resource_group_name=None</em>, <em>tags=None</em>, <em>ttl=None</em>, <em>zone_name=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.dns.CNameRecord.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing CNameRecord resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.
:param str resource_name: The unique name of the resulting resource.
:param str id: The unique provider ID of the resource to lookup.
:param pulumi.ResourceOptions opts: Options for the resource.
:param pulumi.Input[str] name: The name of the DNS CNAME Record.
:param pulumi.Input[str] record: The target of the CNAME.
:param pulumi.Input[str] resource_group_name: Specifies the resource group where the resource exists. Changing this forces a new resource to be created.
:param pulumi.Input[dict] tags: A mapping of tags to assign to the resource.
:param pulumi.Input[str] zone_name: Specifies the DNS Zone where the resource exists. Changing this forces a new resource to be created.</p>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/dns_cname_record.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/dns_cname_record.html.markdown</a>.</div></blockquote>
</dd></dl>

<dl class="method">
<dt id="pulumi_azure.dns.CNameRecord.translate_output_property">
<code class="descname">translate_output_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.dns.CNameRecord.translate_output_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_azure.dns.CNameRecord.translate_input_property">
<code class="descname">translate_input_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.dns.CNameRecord.translate_input_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_azure.dns.CaaRecord">
<em class="property">class </em><code class="descclassname">pulumi_azure.dns.</code><code class="descname">CaaRecord</code><span class="sig-paren">(</span><em>resource_name</em>, <em>opts=None</em>, <em>name=None</em>, <em>records=None</em>, <em>resource_group_name=None</em>, <em>tags=None</em>, <em>ttl=None</em>, <em>zone_name=None</em>, <em>__props__=None</em>, <em>__name__=None</em>, <em>__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.dns.CaaRecord" title="Permalink to this definition">¶</a></dt>
<dd><p>Enables you to manage DNS CAA Records within Azure DNS.</p>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><ul class="first last simple">
<li><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</li>
<li><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</li>
<li><strong>name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The name of the DNS CAA Record.</li>
<li><strong>records</strong> (<em>pulumi.Input</em><em>[</em><em>list</em><em>]</em>) – A list of values that make up the CAA record. Each <code class="docutils literal notranslate"><span class="pre">record</span></code> block supports fields documented below.</li>
<li><strong>resource_group_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Specifies the resource group where the resource exists. Changing this forces a new resource to be created.</li>
<li><strong>tags</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A mapping of tags to assign to the resource.</li>
<li><strong>ttl</strong> (<em>pulumi.Input</em><em>[</em><em>float</em><em>]</em>) – The Time To Live (TTL) of the DNS record in seconds.</li>
<li><strong>zone_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Specifies the DNS Zone where the resource exists. Changing this forces a new resource to be created.</li>
</ul>
</td>
</tr>
</tbody>
</table>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/dns_caa_record.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/dns_caa_record.html.markdown</a>.</div></blockquote>
<dl class="attribute">
<dt id="pulumi_azure.dns.CaaRecord.name">
<code class="descname">name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.CaaRecord.name" title="Permalink to this definition">¶</a></dt>
<dd><p>The name of the DNS CAA Record.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.dns.CaaRecord.records">
<code class="descname">records</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.CaaRecord.records" title="Permalink to this definition">¶</a></dt>
<dd><p>A list of values that make up the CAA record. Each <code class="docutils literal notranslate"><span class="pre">record</span></code> block supports fields documented below.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.dns.CaaRecord.resource_group_name">
<code class="descname">resource_group_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.CaaRecord.resource_group_name" title="Permalink to this definition">¶</a></dt>
<dd><p>Specifies the resource group where the resource exists. Changing this forces a new resource to be created.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.dns.CaaRecord.tags">
<code class="descname">tags</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.CaaRecord.tags" title="Permalink to this definition">¶</a></dt>
<dd><p>A mapping of tags to assign to the resource.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.dns.CaaRecord.ttl">
<code class="descname">ttl</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.CaaRecord.ttl" title="Permalink to this definition">¶</a></dt>
<dd><p>The Time To Live (TTL) of the DNS record in seconds.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.dns.CaaRecord.zone_name">
<code class="descname">zone_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.CaaRecord.zone_name" title="Permalink to this definition">¶</a></dt>
<dd><p>Specifies the DNS Zone where the resource exists. Changing this forces a new resource to be created.</p>
</dd></dl>

<dl class="staticmethod">
<dt id="pulumi_azure.dns.CaaRecord.get">
<em class="property">static </em><code class="descname">get</code><span class="sig-paren">(</span><em>resource_name</em>, <em>id</em>, <em>opts=None</em>, <em>name=None</em>, <em>records=None</em>, <em>resource_group_name=None</em>, <em>tags=None</em>, <em>ttl=None</em>, <em>zone_name=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.dns.CaaRecord.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing CaaRecord resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.
:param str resource_name: The unique name of the resulting resource.
:param str id: The unique provider ID of the resource to lookup.
:param pulumi.ResourceOptions opts: Options for the resource.
:param pulumi.Input[str] name: The name of the DNS CAA Record.
:param pulumi.Input[list] records: A list of values that make up the CAA record. Each <code class="docutils literal notranslate"><span class="pre">record</span></code> block supports fields documented below.
:param pulumi.Input[str] resource_group_name: Specifies the resource group where the resource exists. Changing this forces a new resource to be created.
:param pulumi.Input[dict] tags: A mapping of tags to assign to the resource.
:param pulumi.Input[float] ttl: The Time To Live (TTL) of the DNS record in seconds.
:param pulumi.Input[str] zone_name: Specifies the DNS Zone where the resource exists. Changing this forces a new resource to be created.</p>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/dns_caa_record.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/dns_caa_record.html.markdown</a>.</div></blockquote>
</dd></dl>

<dl class="method">
<dt id="pulumi_azure.dns.CaaRecord.translate_output_property">
<code class="descname">translate_output_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.dns.CaaRecord.translate_output_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_azure.dns.CaaRecord.translate_input_property">
<code class="descname">translate_input_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.dns.CaaRecord.translate_input_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_azure.dns.GetZoneResult">
<em class="property">class </em><code class="descclassname">pulumi_azure.dns.</code><code class="descname">GetZoneResult</code><span class="sig-paren">(</span><em>max_number_of_record_sets=None</em>, <em>name=None</em>, <em>name_servers=None</em>, <em>number_of_record_sets=None</em>, <em>registration_virtual_network_ids=None</em>, <em>resolution_virtual_network_ids=None</em>, <em>resource_group_name=None</em>, <em>tags=None</em>, <em>zone_type=None</em>, <em>id=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.dns.GetZoneResult" title="Permalink to this definition">¶</a></dt>
<dd><p>A collection of values returned by getZone.</p>
<dl class="attribute">
<dt id="pulumi_azure.dns.GetZoneResult.max_number_of_record_sets">
<code class="descname">max_number_of_record_sets</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.GetZoneResult.max_number_of_record_sets" title="Permalink to this definition">¶</a></dt>
<dd><p>Maximum number of Records in the zone.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.dns.GetZoneResult.name_servers">
<code class="descname">name_servers</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.GetZoneResult.name_servers" title="Permalink to this definition">¶</a></dt>
<dd><p>A list of values that make up the NS record for the zone.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.dns.GetZoneResult.number_of_record_sets">
<code class="descname">number_of_record_sets</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.GetZoneResult.number_of_record_sets" title="Permalink to this definition">¶</a></dt>
<dd><p>The number of records already in the zone.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.dns.GetZoneResult.registration_virtual_network_ids">
<code class="descname">registration_virtual_network_ids</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.GetZoneResult.registration_virtual_network_ids" title="Permalink to this definition">¶</a></dt>
<dd><p>A list of Virtual Network ID’s that register hostnames in this DNS zone.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.dns.GetZoneResult.resolution_virtual_network_ids">
<code class="descname">resolution_virtual_network_ids</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.GetZoneResult.resolution_virtual_network_ids" title="Permalink to this definition">¶</a></dt>
<dd><p>A list of Virtual Network ID’s that resolve records in this DNS zone.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.dns.GetZoneResult.tags">
<code class="descname">tags</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.GetZoneResult.tags" title="Permalink to this definition">¶</a></dt>
<dd><p>A mapping of tags to assign to the EventHub Namespace.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.dns.GetZoneResult.zone_type">
<code class="descname">zone_type</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.GetZoneResult.zone_type" title="Permalink to this definition">¶</a></dt>
<dd><p>The type of this DNS zone, such as <code class="docutils literal notranslate"><span class="pre">Public</span></code> or <code class="docutils literal notranslate"><span class="pre">Private</span></code>.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.dns.GetZoneResult.id">
<code class="descname">id</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.GetZoneResult.id" title="Permalink to this definition">¶</a></dt>
<dd><p>id is the provider-assigned unique ID for this managed resource.</p>
</dd></dl>

</dd></dl>

<dl class="class">
<dt id="pulumi_azure.dns.MxRecord">
<em class="property">class </em><code class="descclassname">pulumi_azure.dns.</code><code class="descname">MxRecord</code><span class="sig-paren">(</span><em>resource_name</em>, <em>opts=None</em>, <em>name=None</em>, <em>records=None</em>, <em>resource_group_name=None</em>, <em>tags=None</em>, <em>ttl=None</em>, <em>zone_name=None</em>, <em>__props__=None</em>, <em>__name__=None</em>, <em>__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.dns.MxRecord" title="Permalink to this definition">¶</a></dt>
<dd><p>Enables you to manage DNS MX Records within Azure DNS.</p>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><ul class="first last simple">
<li><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</li>
<li><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</li>
<li><strong>name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The name of the DNS MX Record.</li>
<li><strong>records</strong> (<em>pulumi.Input</em><em>[</em><em>list</em><em>]</em>) – A list of values that make up the MX record. Each <code class="docutils literal notranslate"><span class="pre">record</span></code> block supports fields documented below.</li>
<li><strong>resource_group_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Specifies the resource group where the resource exists. Changing this forces a new resource to be created.</li>
<li><strong>tags</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A mapping of tags to assign to the resource.</li>
<li><strong>ttl</strong> (<em>pulumi.Input</em><em>[</em><em>float</em><em>]</em>) – The Time To Live (TTL) of the DNS record in seconds.</li>
<li><strong>zone_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Specifies the DNS Zone where the resource exists. Changing this forces a new resource to be created.</li>
</ul>
</td>
</tr>
</tbody>
</table>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/dns_mx_record.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/dns_mx_record.html.markdown</a>.</div></blockquote>
<dl class="attribute">
<dt id="pulumi_azure.dns.MxRecord.name">
<code class="descname">name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.MxRecord.name" title="Permalink to this definition">¶</a></dt>
<dd><p>The name of the DNS MX Record.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.dns.MxRecord.records">
<code class="descname">records</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.MxRecord.records" title="Permalink to this definition">¶</a></dt>
<dd><p>A list of values that make up the MX record. Each <code class="docutils literal notranslate"><span class="pre">record</span></code> block supports fields documented below.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.dns.MxRecord.resource_group_name">
<code class="descname">resource_group_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.MxRecord.resource_group_name" title="Permalink to this definition">¶</a></dt>
<dd><p>Specifies the resource group where the resource exists. Changing this forces a new resource to be created.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.dns.MxRecord.tags">
<code class="descname">tags</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.MxRecord.tags" title="Permalink to this definition">¶</a></dt>
<dd><p>A mapping of tags to assign to the resource.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.dns.MxRecord.ttl">
<code class="descname">ttl</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.MxRecord.ttl" title="Permalink to this definition">¶</a></dt>
<dd><p>The Time To Live (TTL) of the DNS record in seconds.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.dns.MxRecord.zone_name">
<code class="descname">zone_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.MxRecord.zone_name" title="Permalink to this definition">¶</a></dt>
<dd><p>Specifies the DNS Zone where the resource exists. Changing this forces a new resource to be created.</p>
</dd></dl>

<dl class="staticmethod">
<dt id="pulumi_azure.dns.MxRecord.get">
<em class="property">static </em><code class="descname">get</code><span class="sig-paren">(</span><em>resource_name</em>, <em>id</em>, <em>opts=None</em>, <em>name=None</em>, <em>records=None</em>, <em>resource_group_name=None</em>, <em>tags=None</em>, <em>ttl=None</em>, <em>zone_name=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.dns.MxRecord.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing MxRecord resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.
:param str resource_name: The unique name of the resulting resource.
:param str id: The unique provider ID of the resource to lookup.
:param pulumi.ResourceOptions opts: Options for the resource.
:param pulumi.Input[str] name: The name of the DNS MX Record.
:param pulumi.Input[list] records: A list of values that make up the MX record. Each <code class="docutils literal notranslate"><span class="pre">record</span></code> block supports fields documented below.
:param pulumi.Input[str] resource_group_name: Specifies the resource group where the resource exists. Changing this forces a new resource to be created.
:param pulumi.Input[dict] tags: A mapping of tags to assign to the resource.
:param pulumi.Input[float] ttl: The Time To Live (TTL) of the DNS record in seconds.
:param pulumi.Input[str] zone_name: Specifies the DNS Zone where the resource exists. Changing this forces a new resource to be created.</p>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/dns_mx_record.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/dns_mx_record.html.markdown</a>.</div></blockquote>
</dd></dl>

<dl class="method">
<dt id="pulumi_azure.dns.MxRecord.translate_output_property">
<code class="descname">translate_output_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.dns.MxRecord.translate_output_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_azure.dns.MxRecord.translate_input_property">
<code class="descname">translate_input_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.dns.MxRecord.translate_input_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_azure.dns.NsRecord">
<em class="property">class </em><code class="descclassname">pulumi_azure.dns.</code><code class="descname">NsRecord</code><span class="sig-paren">(</span><em>resource_name</em>, <em>opts=None</em>, <em>name=None</em>, <em>record=None</em>, <em>records=None</em>, <em>resource_group_name=None</em>, <em>tags=None</em>, <em>ttl=None</em>, <em>zone_name=None</em>, <em>__props__=None</em>, <em>__name__=None</em>, <em>__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.dns.NsRecord" title="Permalink to this definition">¶</a></dt>
<dd><p>Enables you to manage DNS NS Records within Azure DNS.</p>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><ul class="first last simple">
<li><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</li>
<li><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</li>
<li><strong>name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The name of the DNS NS Record.</li>
<li><strong>record</strong> (<em>pulumi.Input</em><em>[</em><em>list</em><em>]</em>) – A list of values that make up the NS record. Each <code class="docutils literal notranslate"><span class="pre">record</span></code> block supports fields documented below. This field has been deprecated and will be removed in a future release.</li>
<li><strong>records</strong> (<em>pulumi.Input</em><em>[</em><em>list</em><em>]</em>) – A list of values that make up the NS record. <em>WARNING</em>: Either <code class="docutils literal notranslate"><span class="pre">records</span></code> or <code class="docutils literal notranslate"><span class="pre">record</span></code> is required.</li>
<li><strong>resource_group_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Specifies the resource group where the resource exists. Changing this forces a new resource to be created.</li>
<li><strong>tags</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A mapping of tags to assign to the resource.</li>
<li><strong>ttl</strong> (<em>pulumi.Input</em><em>[</em><em>float</em><em>]</em>) – The Time To Live (TTL) of the DNS record in seconds.</li>
<li><strong>zone_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Specifies the DNS Zone where the resource exists. Changing this forces a new resource to be created.</li>
</ul>
</td>
</tr>
</tbody>
</table>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/dns_ns_record.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/dns_ns_record.html.markdown</a>.</div></blockquote>
<dl class="attribute">
<dt id="pulumi_azure.dns.NsRecord.name">
<code class="descname">name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.NsRecord.name" title="Permalink to this definition">¶</a></dt>
<dd><p>The name of the DNS NS Record.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.dns.NsRecord.record">
<code class="descname">record</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.NsRecord.record" title="Permalink to this definition">¶</a></dt>
<dd><p>A list of values that make up the NS record. Each <code class="docutils literal notranslate"><span class="pre">record</span></code> block supports fields documented below. This field has been deprecated and will be removed in a future release.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.dns.NsRecord.records">
<code class="descname">records</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.NsRecord.records" title="Permalink to this definition">¶</a></dt>
<dd><p>A list of values that make up the NS record. <em>WARNING</em>: Either <code class="docutils literal notranslate"><span class="pre">records</span></code> or <code class="docutils literal notranslate"><span class="pre">record</span></code> is required.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.dns.NsRecord.resource_group_name">
<code class="descname">resource_group_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.NsRecord.resource_group_name" title="Permalink to this definition">¶</a></dt>
<dd><p>Specifies the resource group where the resource exists. Changing this forces a new resource to be created.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.dns.NsRecord.tags">
<code class="descname">tags</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.NsRecord.tags" title="Permalink to this definition">¶</a></dt>
<dd><p>A mapping of tags to assign to the resource.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.dns.NsRecord.ttl">
<code class="descname">ttl</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.NsRecord.ttl" title="Permalink to this definition">¶</a></dt>
<dd><p>The Time To Live (TTL) of the DNS record in seconds.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.dns.NsRecord.zone_name">
<code class="descname">zone_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.NsRecord.zone_name" title="Permalink to this definition">¶</a></dt>
<dd><p>Specifies the DNS Zone where the resource exists. Changing this forces a new resource to be created.</p>
</dd></dl>

<dl class="staticmethod">
<dt id="pulumi_azure.dns.NsRecord.get">
<em class="property">static </em><code class="descname">get</code><span class="sig-paren">(</span><em>resource_name</em>, <em>id</em>, <em>opts=None</em>, <em>name=None</em>, <em>record=None</em>, <em>records=None</em>, <em>resource_group_name=None</em>, <em>tags=None</em>, <em>ttl=None</em>, <em>zone_name=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.dns.NsRecord.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing NsRecord resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.
:param str resource_name: The unique name of the resulting resource.
:param str id: The unique provider ID of the resource to lookup.
:param pulumi.ResourceOptions opts: Options for the resource.
:param pulumi.Input[str] name: The name of the DNS NS Record.
:param pulumi.Input[list] record: A list of values that make up the NS record. Each <code class="docutils literal notranslate"><span class="pre">record</span></code> block supports fields documented below. This field has been deprecated and will be removed in a future release.
:param pulumi.Input[list] records: A list of values that make up the NS record. <em>WARNING</em>: Either <code class="docutils literal notranslate"><span class="pre">records</span></code> or <code class="docutils literal notranslate"><span class="pre">record</span></code> is required.
:param pulumi.Input[str] resource_group_name: Specifies the resource group where the resource exists. Changing this forces a new resource to be created.
:param pulumi.Input[dict] tags: A mapping of tags to assign to the resource.
:param pulumi.Input[float] ttl: The Time To Live (TTL) of the DNS record in seconds.
:param pulumi.Input[str] zone_name: Specifies the DNS Zone where the resource exists. Changing this forces a new resource to be created.</p>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/dns_ns_record.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/dns_ns_record.html.markdown</a>.</div></blockquote>
</dd></dl>

<dl class="method">
<dt id="pulumi_azure.dns.NsRecord.translate_output_property">
<code class="descname">translate_output_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.dns.NsRecord.translate_output_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_azure.dns.NsRecord.translate_input_property">
<code class="descname">translate_input_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.dns.NsRecord.translate_input_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_azure.dns.PtrRecord">
<em class="property">class </em><code class="descclassname">pulumi_azure.dns.</code><code class="descname">PtrRecord</code><span class="sig-paren">(</span><em>resource_name</em>, <em>opts=None</em>, <em>name=None</em>, <em>records=None</em>, <em>resource_group_name=None</em>, <em>tags=None</em>, <em>ttl=None</em>, <em>zone_name=None</em>, <em>__props__=None</em>, <em>__name__=None</em>, <em>__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.dns.PtrRecord" title="Permalink to this definition">¶</a></dt>
<dd><p>Enables you to manage DNS PTR Records within Azure DNS.</p>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><ul class="first last simple">
<li><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</li>
<li><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</li>
<li><strong>name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The name of the DNS PTR Record.</li>
<li><strong>records</strong> (<em>pulumi.Input</em><em>[</em><em>list</em><em>]</em>) – List of Fully Qualified Domain Names.</li>
<li><strong>resource_group_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Specifies the resource group where the resource exists. Changing this forces a new resource to be created.</li>
<li><strong>tags</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A mapping of tags to assign to the resource.</li>
<li><strong>ttl</strong> (<em>pulumi.Input</em><em>[</em><em>float</em><em>]</em>) – The Time To Live (TTL) of the DNS record in seconds.</li>
<li><strong>zone_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Specifies the DNS Zone where the resource exists. Changing this forces a new resource to be created.</li>
</ul>
</td>
</tr>
</tbody>
</table>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/dns_ptr_record.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/dns_ptr_record.html.markdown</a>.</div></blockquote>
<dl class="attribute">
<dt id="pulumi_azure.dns.PtrRecord.name">
<code class="descname">name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.PtrRecord.name" title="Permalink to this definition">¶</a></dt>
<dd><p>The name of the DNS PTR Record.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.dns.PtrRecord.records">
<code class="descname">records</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.PtrRecord.records" title="Permalink to this definition">¶</a></dt>
<dd><p>List of Fully Qualified Domain Names.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.dns.PtrRecord.resource_group_name">
<code class="descname">resource_group_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.PtrRecord.resource_group_name" title="Permalink to this definition">¶</a></dt>
<dd><p>Specifies the resource group where the resource exists. Changing this forces a new resource to be created.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.dns.PtrRecord.tags">
<code class="descname">tags</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.PtrRecord.tags" title="Permalink to this definition">¶</a></dt>
<dd><p>A mapping of tags to assign to the resource.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.dns.PtrRecord.ttl">
<code class="descname">ttl</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.PtrRecord.ttl" title="Permalink to this definition">¶</a></dt>
<dd><p>The Time To Live (TTL) of the DNS record in seconds.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.dns.PtrRecord.zone_name">
<code class="descname">zone_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.PtrRecord.zone_name" title="Permalink to this definition">¶</a></dt>
<dd><p>Specifies the DNS Zone where the resource exists. Changing this forces a new resource to be created.</p>
</dd></dl>

<dl class="staticmethod">
<dt id="pulumi_azure.dns.PtrRecord.get">
<em class="property">static </em><code class="descname">get</code><span class="sig-paren">(</span><em>resource_name</em>, <em>id</em>, <em>opts=None</em>, <em>name=None</em>, <em>records=None</em>, <em>resource_group_name=None</em>, <em>tags=None</em>, <em>ttl=None</em>, <em>zone_name=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.dns.PtrRecord.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing PtrRecord resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.
:param str resource_name: The unique name of the resulting resource.
:param str id: The unique provider ID of the resource to lookup.
:param pulumi.ResourceOptions opts: Options for the resource.
:param pulumi.Input[str] name: The name of the DNS PTR Record.
:param pulumi.Input[list] records: List of Fully Qualified Domain Names.
:param pulumi.Input[str] resource_group_name: Specifies the resource group where the resource exists. Changing this forces a new resource to be created.
:param pulumi.Input[dict] tags: A mapping of tags to assign to the resource.
:param pulumi.Input[float] ttl: The Time To Live (TTL) of the DNS record in seconds.
:param pulumi.Input[str] zone_name: Specifies the DNS Zone where the resource exists. Changing this forces a new resource to be created.</p>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/dns_ptr_record.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/dns_ptr_record.html.markdown</a>.</div></blockquote>
</dd></dl>

<dl class="method">
<dt id="pulumi_azure.dns.PtrRecord.translate_output_property">
<code class="descname">translate_output_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.dns.PtrRecord.translate_output_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_azure.dns.PtrRecord.translate_input_property">
<code class="descname">translate_input_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.dns.PtrRecord.translate_input_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_azure.dns.SrvRecord">
<em class="property">class </em><code class="descclassname">pulumi_azure.dns.</code><code class="descname">SrvRecord</code><span class="sig-paren">(</span><em>resource_name</em>, <em>opts=None</em>, <em>name=None</em>, <em>records=None</em>, <em>resource_group_name=None</em>, <em>tags=None</em>, <em>ttl=None</em>, <em>zone_name=None</em>, <em>__props__=None</em>, <em>__name__=None</em>, <em>__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.dns.SrvRecord" title="Permalink to this definition">¶</a></dt>
<dd><p>Enables you to manage DNS SRV Records within Azure DNS.</p>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><ul class="first last simple">
<li><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</li>
<li><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</li>
<li><strong>name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The name of the DNS SRV Record.</li>
<li><strong>records</strong> (<em>pulumi.Input</em><em>[</em><em>list</em><em>]</em>) – A list of values that make up the SRV record. Each <code class="docutils literal notranslate"><span class="pre">record</span></code> block supports fields documented below.</li>
<li><strong>resource_group_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Specifies the resource group where the resource exists. Changing this forces a new resource to be created.</li>
<li><strong>tags</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A mapping of tags to assign to the resource.</li>
<li><strong>ttl</strong> (<em>pulumi.Input</em><em>[</em><em>float</em><em>]</em>) – The Time To Live (TTL) of the DNS record in seconds.</li>
<li><strong>zone_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Specifies the DNS Zone where the resource exists. Changing this forces a new resource to be created.</li>
</ul>
</td>
</tr>
</tbody>
</table>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/dns_srv_record.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/dns_srv_record.html.markdown</a>.</div></blockquote>
<dl class="attribute">
<dt id="pulumi_azure.dns.SrvRecord.name">
<code class="descname">name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.SrvRecord.name" title="Permalink to this definition">¶</a></dt>
<dd><p>The name of the DNS SRV Record.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.dns.SrvRecord.records">
<code class="descname">records</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.SrvRecord.records" title="Permalink to this definition">¶</a></dt>
<dd><p>A list of values that make up the SRV record. Each <code class="docutils literal notranslate"><span class="pre">record</span></code> block supports fields documented below.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.dns.SrvRecord.resource_group_name">
<code class="descname">resource_group_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.SrvRecord.resource_group_name" title="Permalink to this definition">¶</a></dt>
<dd><p>Specifies the resource group where the resource exists. Changing this forces a new resource to be created.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.dns.SrvRecord.tags">
<code class="descname">tags</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.SrvRecord.tags" title="Permalink to this definition">¶</a></dt>
<dd><p>A mapping of tags to assign to the resource.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.dns.SrvRecord.ttl">
<code class="descname">ttl</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.SrvRecord.ttl" title="Permalink to this definition">¶</a></dt>
<dd><p>The Time To Live (TTL) of the DNS record in seconds.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.dns.SrvRecord.zone_name">
<code class="descname">zone_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.SrvRecord.zone_name" title="Permalink to this definition">¶</a></dt>
<dd><p>Specifies the DNS Zone where the resource exists. Changing this forces a new resource to be created.</p>
</dd></dl>

<dl class="staticmethod">
<dt id="pulumi_azure.dns.SrvRecord.get">
<em class="property">static </em><code class="descname">get</code><span class="sig-paren">(</span><em>resource_name</em>, <em>id</em>, <em>opts=None</em>, <em>name=None</em>, <em>records=None</em>, <em>resource_group_name=None</em>, <em>tags=None</em>, <em>ttl=None</em>, <em>zone_name=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.dns.SrvRecord.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing SrvRecord resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.
:param str resource_name: The unique name of the resulting resource.
:param str id: The unique provider ID of the resource to lookup.
:param pulumi.ResourceOptions opts: Options for the resource.
:param pulumi.Input[str] name: The name of the DNS SRV Record.
:param pulumi.Input[list] records: A list of values that make up the SRV record. Each <code class="docutils literal notranslate"><span class="pre">record</span></code> block supports fields documented below.
:param pulumi.Input[str] resource_group_name: Specifies the resource group where the resource exists. Changing this forces a new resource to be created.
:param pulumi.Input[dict] tags: A mapping of tags to assign to the resource.
:param pulumi.Input[float] ttl: The Time To Live (TTL) of the DNS record in seconds.
:param pulumi.Input[str] zone_name: Specifies the DNS Zone where the resource exists. Changing this forces a new resource to be created.</p>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/dns_srv_record.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/dns_srv_record.html.markdown</a>.</div></blockquote>
</dd></dl>

<dl class="method">
<dt id="pulumi_azure.dns.SrvRecord.translate_output_property">
<code class="descname">translate_output_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.dns.SrvRecord.translate_output_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_azure.dns.SrvRecord.translate_input_property">
<code class="descname">translate_input_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.dns.SrvRecord.translate_input_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_azure.dns.TxtRecord">
<em class="property">class </em><code class="descclassname">pulumi_azure.dns.</code><code class="descname">TxtRecord</code><span class="sig-paren">(</span><em>resource_name</em>, <em>opts=None</em>, <em>name=None</em>, <em>records=None</em>, <em>resource_group_name=None</em>, <em>tags=None</em>, <em>ttl=None</em>, <em>zone_name=None</em>, <em>__props__=None</em>, <em>__name__=None</em>, <em>__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.dns.TxtRecord" title="Permalink to this definition">¶</a></dt>
<dd><p>Enables you to manage DNS TXT Records within Azure DNS.</p>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><ul class="first last simple">
<li><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</li>
<li><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</li>
<li><strong>name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The name of the DNS TXT Record.</li>
<li><strong>records</strong> (<em>pulumi.Input</em><em>[</em><em>list</em><em>]</em>) – A list of values that make up the txt record. Each <code class="docutils literal notranslate"><span class="pre">record</span></code> block supports fields documented below.</li>
<li><strong>resource_group_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Specifies the resource group where the resource exists. Changing this forces a new resource to be created.</li>
<li><strong>tags</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A mapping of tags to assign to the resource.</li>
<li><strong>ttl</strong> (<em>pulumi.Input</em><em>[</em><em>float</em><em>]</em>) – The Time To Live (TTL) of the DNS record in seconds.</li>
<li><strong>zone_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Specifies the DNS Zone where the resource exists. Changing this forces a new resource to be created.</li>
</ul>
</td>
</tr>
</tbody>
</table>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/dns_txt_record.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/dns_txt_record.html.markdown</a>.</div></blockquote>
<dl class="attribute">
<dt id="pulumi_azure.dns.TxtRecord.name">
<code class="descname">name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.TxtRecord.name" title="Permalink to this definition">¶</a></dt>
<dd><p>The name of the DNS TXT Record.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.dns.TxtRecord.records">
<code class="descname">records</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.TxtRecord.records" title="Permalink to this definition">¶</a></dt>
<dd><p>A list of values that make up the txt record. Each <code class="docutils literal notranslate"><span class="pre">record</span></code> block supports fields documented below.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.dns.TxtRecord.resource_group_name">
<code class="descname">resource_group_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.TxtRecord.resource_group_name" title="Permalink to this definition">¶</a></dt>
<dd><p>Specifies the resource group where the resource exists. Changing this forces a new resource to be created.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.dns.TxtRecord.tags">
<code class="descname">tags</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.TxtRecord.tags" title="Permalink to this definition">¶</a></dt>
<dd><p>A mapping of tags to assign to the resource.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.dns.TxtRecord.ttl">
<code class="descname">ttl</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.TxtRecord.ttl" title="Permalink to this definition">¶</a></dt>
<dd><p>The Time To Live (TTL) of the DNS record in seconds.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.dns.TxtRecord.zone_name">
<code class="descname">zone_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.TxtRecord.zone_name" title="Permalink to this definition">¶</a></dt>
<dd><p>Specifies the DNS Zone where the resource exists. Changing this forces a new resource to be created.</p>
</dd></dl>

<dl class="staticmethod">
<dt id="pulumi_azure.dns.TxtRecord.get">
<em class="property">static </em><code class="descname">get</code><span class="sig-paren">(</span><em>resource_name</em>, <em>id</em>, <em>opts=None</em>, <em>name=None</em>, <em>records=None</em>, <em>resource_group_name=None</em>, <em>tags=None</em>, <em>ttl=None</em>, <em>zone_name=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.dns.TxtRecord.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing TxtRecord resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.
:param str resource_name: The unique name of the resulting resource.
:param str id: The unique provider ID of the resource to lookup.
:param pulumi.ResourceOptions opts: Options for the resource.
:param pulumi.Input[str] name: The name of the DNS TXT Record.
:param pulumi.Input[list] records: A list of values that make up the txt record. Each <code class="docutils literal notranslate"><span class="pre">record</span></code> block supports fields documented below.
:param pulumi.Input[str] resource_group_name: Specifies the resource group where the resource exists. Changing this forces a new resource to be created.
:param pulumi.Input[dict] tags: A mapping of tags to assign to the resource.
:param pulumi.Input[float] ttl: The Time To Live (TTL) of the DNS record in seconds.
:param pulumi.Input[str] zone_name: Specifies the DNS Zone where the resource exists. Changing this forces a new resource to be created.</p>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/dns_txt_record.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/dns_txt_record.html.markdown</a>.</div></blockquote>
</dd></dl>

<dl class="method">
<dt id="pulumi_azure.dns.TxtRecord.translate_output_property">
<code class="descname">translate_output_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.dns.TxtRecord.translate_output_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_azure.dns.TxtRecord.translate_input_property">
<code class="descname">translate_input_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.dns.TxtRecord.translate_input_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_azure.dns.Zone">
<em class="property">class </em><code class="descclassname">pulumi_azure.dns.</code><code class="descname">Zone</code><span class="sig-paren">(</span><em>resource_name</em>, <em>opts=None</em>, <em>name=None</em>, <em>registration_virtual_network_ids=None</em>, <em>resolution_virtual_network_ids=None</em>, <em>resource_group_name=None</em>, <em>tags=None</em>, <em>zone_type=None</em>, <em>__props__=None</em>, <em>__name__=None</em>, <em>__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.dns.Zone" title="Permalink to this definition">¶</a></dt>
<dd><p>Enables you to manage DNS zones within Azure DNS. These zones are hosted on Azure’s name servers to which you can delegate the zone from the parent domain.</p>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><ul class="first last simple">
<li><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</li>
<li><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</li>
<li><strong>name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The name of the DNS Zone. Must be a valid domain name.</li>
<li><strong>registration_virtual_network_ids</strong> (<em>pulumi.Input</em><em>[</em><em>list</em><em>]</em>) – A list of Virtual Network ID’s that register hostnames in this DNS zone. This field can only be set when <code class="docutils literal notranslate"><span class="pre">zone_type</span></code> is set to <code class="docutils literal notranslate"><span class="pre">Private</span></code>.</li>
<li><strong>resolution_virtual_network_ids</strong> (<em>pulumi.Input</em><em>[</em><em>list</em><em>]</em>) – A list of Virtual Network ID’s that resolve records in this DNS zone. This field can only be set when <code class="docutils literal notranslate"><span class="pre">zone_type</span></code> is set to <code class="docutils literal notranslate"><span class="pre">Private</span></code>.</li>
<li><strong>resource_group_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Specifies the resource group where the resource exists. Changing this forces a new resource to be created.</li>
<li><strong>tags</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A mapping of tags to assign to the resource.</li>
<li><strong>zone_type</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Specifies the type of this DNS zone. Possible values are <code class="docutils literal notranslate"><span class="pre">Public</span></code> or <code class="docutils literal notranslate"><span class="pre">Private</span></code> (Defaults to <code class="docutils literal notranslate"><span class="pre">Public</span></code>).</li>
</ul>
</td>
</tr>
</tbody>
</table>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/dns_zone.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/dns_zone.html.markdown</a>.</div></blockquote>
<dl class="attribute">
<dt id="pulumi_azure.dns.Zone.max_number_of_record_sets">
<code class="descname">max_number_of_record_sets</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.Zone.max_number_of_record_sets" title="Permalink to this definition">¶</a></dt>
<dd><p>(Optional) Maximum number of Records in the zone. Defaults to <code class="docutils literal notranslate"><span class="pre">1000</span></code>.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.dns.Zone.name">
<code class="descname">name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.Zone.name" title="Permalink to this definition">¶</a></dt>
<dd><p>The name of the DNS Zone. Must be a valid domain name.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.dns.Zone.name_servers">
<code class="descname">name_servers</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.Zone.name_servers" title="Permalink to this definition">¶</a></dt>
<dd><p>(Optional) A list of values that make up the NS record for the zone.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.dns.Zone.number_of_record_sets">
<code class="descname">number_of_record_sets</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.Zone.number_of_record_sets" title="Permalink to this definition">¶</a></dt>
<dd><p>(Optional) The number of records already in the zone.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.dns.Zone.registration_virtual_network_ids">
<code class="descname">registration_virtual_network_ids</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.Zone.registration_virtual_network_ids" title="Permalink to this definition">¶</a></dt>
<dd><p>A list of Virtual Network ID’s that register hostnames in this DNS zone. This field can only be set when <code class="docutils literal notranslate"><span class="pre">zone_type</span></code> is set to <code class="docutils literal notranslate"><span class="pre">Private</span></code>.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.dns.Zone.resolution_virtual_network_ids">
<code class="descname">resolution_virtual_network_ids</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.Zone.resolution_virtual_network_ids" title="Permalink to this definition">¶</a></dt>
<dd><p>A list of Virtual Network ID’s that resolve records in this DNS zone. This field can only be set when <code class="docutils literal notranslate"><span class="pre">zone_type</span></code> is set to <code class="docutils literal notranslate"><span class="pre">Private</span></code>.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.dns.Zone.resource_group_name">
<code class="descname">resource_group_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.Zone.resource_group_name" title="Permalink to this definition">¶</a></dt>
<dd><p>Specifies the resource group where the resource exists. Changing this forces a new resource to be created.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.dns.Zone.tags">
<code class="descname">tags</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.Zone.tags" title="Permalink to this definition">¶</a></dt>
<dd><p>A mapping of tags to assign to the resource.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.dns.Zone.zone_type">
<code class="descname">zone_type</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.dns.Zone.zone_type" title="Permalink to this definition">¶</a></dt>
<dd><p>Specifies the type of this DNS zone. Possible values are <code class="docutils literal notranslate"><span class="pre">Public</span></code> or <code class="docutils literal notranslate"><span class="pre">Private</span></code> (Defaults to <code class="docutils literal notranslate"><span class="pre">Public</span></code>).</p>
</dd></dl>

<dl class="staticmethod">
<dt id="pulumi_azure.dns.Zone.get">
<em class="property">static </em><code class="descname">get</code><span class="sig-paren">(</span><em>resource_name</em>, <em>id</em>, <em>opts=None</em>, <em>max_number_of_record_sets=None</em>, <em>name=None</em>, <em>name_servers=None</em>, <em>number_of_record_sets=None</em>, <em>registration_virtual_network_ids=None</em>, <em>resolution_virtual_network_ids=None</em>, <em>resource_group_name=None</em>, <em>tags=None</em>, <em>zone_type=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.dns.Zone.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing Zone resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.
:param str resource_name: The unique name of the resulting resource.
:param str id: The unique provider ID of the resource to lookup.
:param pulumi.ResourceOptions opts: Options for the resource.
:param pulumi.Input[float] max_number_of_record_sets: (Optional) Maximum number of Records in the zone. Defaults to <code class="docutils literal notranslate"><span class="pre">1000</span></code>.
:param pulumi.Input[str] name: The name of the DNS Zone. Must be a valid domain name.
:param pulumi.Input[list] name_servers: (Optional) A list of values that make up the NS record for the zone.
:param pulumi.Input[float] number_of_record_sets: (Optional) The number of records already in the zone.
:param pulumi.Input[list] registration_virtual_network_ids: A list of Virtual Network ID’s that register hostnames in this DNS zone. This field can only be set when <code class="docutils literal notranslate"><span class="pre">zone_type</span></code> is set to <code class="docutils literal notranslate"><span class="pre">Private</span></code>.
:param pulumi.Input[list] resolution_virtual_network_ids: A list of Virtual Network ID’s that resolve records in this DNS zone. This field can only be set when <code class="docutils literal notranslate"><span class="pre">zone_type</span></code> is set to <code class="docutils literal notranslate"><span class="pre">Private</span></code>.
:param pulumi.Input[str] resource_group_name: Specifies the resource group where the resource exists. Changing this forces a new resource to be created.
:param pulumi.Input[dict] tags: A mapping of tags to assign to the resource.
:param pulumi.Input[str] zone_type: Specifies the type of this DNS zone. Possible values are <code class="docutils literal notranslate"><span class="pre">Public</span></code> or <code class="docutils literal notranslate"><span class="pre">Private</span></code> (Defaults to <code class="docutils literal notranslate"><span class="pre">Public</span></code>).</p>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/dns_zone.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/dns_zone.html.markdown</a>.</div></blockquote>
</dd></dl>

<dl class="method">
<dt id="pulumi_azure.dns.Zone.translate_output_property">
<code class="descname">translate_output_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.dns.Zone.translate_output_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_azure.dns.Zone.translate_input_property">
<code class="descname">translate_input_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.dns.Zone.translate_input_property" title="Permalink to this definition">¶</a></dt>
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

<dl class="function">
<dt id="pulumi_azure.dns.get_zone">
<code class="descclassname">pulumi_azure.dns.</code><code class="descname">get_zone</code><span class="sig-paren">(</span><em>name=None</em>, <em>resource_group_name=None</em>, <em>opts=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.dns.get_zone" title="Permalink to this definition">¶</a></dt>
<dd><p>Use this data source to access information about an existing DNS Zone.</p>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/d/dns_zone.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/d/dns_zone.html.markdown</a>.</div></blockquote>
</dd></dl>

</div>
