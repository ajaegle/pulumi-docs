---
title: Module ad
---

<div class="section" id="ad">
<h1>ad<a class="headerlink" href="#ad" title="Permalink to this headline">¶</a></h1>
<blockquote>
<div>This provider is a derived work of the <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm">Terraform Provider</a> distributed under
<a class="reference external" href="https://www.mozilla.org/en-US/MPL/2.0/">MPL 2.0</a>. If you encounter a bug or missing feature, first check the
<a class="reference external" href="https://github.com/pulumi/pulumi-azure/issues">pulumi/pulumi-azure repo</a>; however, if that doesn’t turn up
anything, please consult the source <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/issues">terraform-providers/terraform-provider-azurerm repo</a>.</div></blockquote>
<span class="target" id="module-pulumi_azure.ad"></span><dl class="class">
<dt id="pulumi_azure.ad.Application">
<em class="property">class </em><code class="descclassname">pulumi_azure.ad.</code><code class="descname">Application</code><span class="sig-paren">(</span><em>resource_name</em>, <em>opts=None</em>, <em>available_to_other_tenants=None</em>, <em>homepage=None</em>, <em>identifier_uris=None</em>, <em>name=None</em>, <em>oauth2_allow_implicit_flow=None</em>, <em>reply_urls=None</em>, <em>__props__=None</em>, <em>__name__=None</em>, <em>__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.ad.Application" title="Permalink to this definition">¶</a></dt>
<dd><p>Create a Application resource with the given unique name, props, and options.</p>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><ul class="first last simple">
<li><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</li>
<li><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</li>
<li><strong>available_to_other_tenants</strong> (<em>pulumi.Input</em><em>[</em><em>bool</em><em>]</em>) – Is this Azure AD Application available to other tenants? Defaults to <code class="docutils literal notranslate"><span class="pre">false</span></code>.</li>
<li><strong>homepage</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The URL to the application’s home page. If no homepage is specified this defaults to <code class="docutils literal notranslate"><span class="pre">https://{name}</span></code>.</li>
<li><strong>identifier_uris</strong> (<em>pulumi.Input</em><em>[</em><em>list</em><em>]</em>) – A list of user-defined URI(s) that uniquely identify a Web application within it’s Azure AD tenant, or within a verified custom domain if the application is multi-tenant.</li>
<li><strong>name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The display name for the application.</li>
<li><strong>oauth2_allow_implicit_flow</strong> (<em>pulumi.Input</em><em>[</em><em>bool</em><em>]</em>) – Does this Azure AD Application allow OAuth2.0 implicit flow tokens? Defaults to <code class="docutils literal notranslate"><span class="pre">false</span></code>.</li>
<li><strong>reply_urls</strong> (<em>pulumi.Input</em><em>[</em><em>list</em><em>]</em>) – A list of URLs that user tokens are sent to for sign in, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to.</li>
</ul>
</td>
</tr>
</tbody>
</table>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/azuread_application.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/azuread_application.html.markdown</a>.</div></blockquote>
<dl class="attribute">
<dt id="pulumi_azure.ad.Application.application_id">
<code class="descname">application_id</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.ad.Application.application_id" title="Permalink to this definition">¶</a></dt>
<dd><p>The Application ID.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.ad.Application.available_to_other_tenants">
<code class="descname">available_to_other_tenants</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.ad.Application.available_to_other_tenants" title="Permalink to this definition">¶</a></dt>
<dd><p>Is this Azure AD Application available to other tenants? Defaults to <code class="docutils literal notranslate"><span class="pre">false</span></code>.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.ad.Application.homepage">
<code class="descname">homepage</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.ad.Application.homepage" title="Permalink to this definition">¶</a></dt>
<dd><p>The URL to the application’s home page. If no homepage is specified this defaults to <code class="docutils literal notranslate"><span class="pre">https://{name}</span></code>.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.ad.Application.identifier_uris">
<code class="descname">identifier_uris</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.ad.Application.identifier_uris" title="Permalink to this definition">¶</a></dt>
<dd><p>A list of user-defined URI(s) that uniquely identify a Web application within it’s Azure AD tenant, or within a verified custom domain if the application is multi-tenant.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.ad.Application.name">
<code class="descname">name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.ad.Application.name" title="Permalink to this definition">¶</a></dt>
<dd><p>The display name for the application.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.ad.Application.oauth2_allow_implicit_flow">
<code class="descname">oauth2_allow_implicit_flow</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.ad.Application.oauth2_allow_implicit_flow" title="Permalink to this definition">¶</a></dt>
<dd><p>Does this Azure AD Application allow OAuth2.0 implicit flow tokens? Defaults to <code class="docutils literal notranslate"><span class="pre">false</span></code>.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.ad.Application.reply_urls">
<code class="descname">reply_urls</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.ad.Application.reply_urls" title="Permalink to this definition">¶</a></dt>
<dd><p>A list of URLs that user tokens are sent to for sign in, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to.</p>
</dd></dl>

<dl class="staticmethod">
<dt id="pulumi_azure.ad.Application.get">
<em class="property">static </em><code class="descname">get</code><span class="sig-paren">(</span><em>resource_name</em>, <em>id</em>, <em>opts=None</em>, <em>application_id=None</em>, <em>available_to_other_tenants=None</em>, <em>homepage=None</em>, <em>identifier_uris=None</em>, <em>name=None</em>, <em>oauth2_allow_implicit_flow=None</em>, <em>reply_urls=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.ad.Application.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing Application resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.
:param str resource_name: The unique name of the resulting resource.
:param str id: The unique provider ID of the resource to lookup.
:param pulumi.ResourceOptions opts: Options for the resource.
:param pulumi.Input[str] application_id: The Application ID.
:param pulumi.Input[bool] available_to_other_tenants: Is this Azure AD Application available to other tenants? Defaults to <code class="docutils literal notranslate"><span class="pre">false</span></code>.
:param pulumi.Input[str] homepage: The URL to the application’s home page. If no homepage is specified this defaults to <code class="docutils literal notranslate"><span class="pre">https://{name}</span></code>.
:param pulumi.Input[list] identifier_uris: A list of user-defined URI(s) that uniquely identify a Web application within it’s Azure AD tenant, or within a verified custom domain if the application is multi-tenant.
:param pulumi.Input[str] name: The display name for the application.
:param pulumi.Input[bool] oauth2_allow_implicit_flow: Does this Azure AD Application allow OAuth2.0 implicit flow tokens? Defaults to <code class="docutils literal notranslate"><span class="pre">false</span></code>.
:param pulumi.Input[list] reply_urls: A list of URLs that user tokens are sent to for sign in, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to.</p>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/azuread_application.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/azuread_application.html.markdown</a>.</div></blockquote>
</dd></dl>

<dl class="method">
<dt id="pulumi_azure.ad.Application.translate_output_property">
<code class="descname">translate_output_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.ad.Application.translate_output_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_azure.ad.Application.translate_input_property">
<code class="descname">translate_input_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.ad.Application.translate_input_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_azure.ad.AwaitableGetApplicationResult">
<em class="property">class </em><code class="descclassname">pulumi_azure.ad.</code><code class="descname">AwaitableGetApplicationResult</code><span class="sig-paren">(</span><em>application_id=None</em>, <em>available_to_other_tenants=None</em>, <em>homepage=None</em>, <em>identifier_uris=None</em>, <em>name=None</em>, <em>oauth2_allow_implicit_flow=None</em>, <em>object_id=None</em>, <em>reply_urls=None</em>, <em>id=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.ad.AwaitableGetApplicationResult" title="Permalink to this definition">¶</a></dt>
<dd></dd></dl>

<dl class="class">
<dt id="pulumi_azure.ad.AwaitableGetServicePrincipalResult">
<em class="property">class </em><code class="descclassname">pulumi_azure.ad.</code><code class="descname">AwaitableGetServicePrincipalResult</code><span class="sig-paren">(</span><em>application_id=None</em>, <em>display_name=None</em>, <em>object_id=None</em>, <em>id=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.ad.AwaitableGetServicePrincipalResult" title="Permalink to this definition">¶</a></dt>
<dd></dd></dl>

<dl class="class">
<dt id="pulumi_azure.ad.GetApplicationResult">
<em class="property">class </em><code class="descclassname">pulumi_azure.ad.</code><code class="descname">GetApplicationResult</code><span class="sig-paren">(</span><em>application_id=None</em>, <em>available_to_other_tenants=None</em>, <em>homepage=None</em>, <em>identifier_uris=None</em>, <em>name=None</em>, <em>oauth2_allow_implicit_flow=None</em>, <em>object_id=None</em>, <em>reply_urls=None</em>, <em>id=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.ad.GetApplicationResult" title="Permalink to this definition">¶</a></dt>
<dd><p>A collection of values returned by getApplication.</p>
<dl class="attribute">
<dt id="pulumi_azure.ad.GetApplicationResult.application_id">
<code class="descname">application_id</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.ad.GetApplicationResult.application_id" title="Permalink to this definition">¶</a></dt>
<dd><p>the Application ID of the Azure Active Directory Application.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.ad.GetApplicationResult.available_to_other_tenants">
<code class="descname">available_to_other_tenants</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.ad.GetApplicationResult.available_to_other_tenants" title="Permalink to this definition">¶</a></dt>
<dd><p>Is this Azure AD Application available to other tenants?</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.ad.GetApplicationResult.identifier_uris">
<code class="descname">identifier_uris</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.ad.GetApplicationResult.identifier_uris" title="Permalink to this definition">¶</a></dt>
<dd><p>A list of user-defined URI(s) that uniquely identify a Web application within it’s Azure AD tenant, or within a verified custom domain if the application is multi-tenant.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.ad.GetApplicationResult.oauth2_allow_implicit_flow">
<code class="descname">oauth2_allow_implicit_flow</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.ad.GetApplicationResult.oauth2_allow_implicit_flow" title="Permalink to this definition">¶</a></dt>
<dd><p>Does this Azure AD Application allow OAuth2.0 implicit flow tokens?</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.ad.GetApplicationResult.object_id">
<code class="descname">object_id</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.ad.GetApplicationResult.object_id" title="Permalink to this definition">¶</a></dt>
<dd><p>the Object ID of the Azure Active Directory Application.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.ad.GetApplicationResult.reply_urls">
<code class="descname">reply_urls</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.ad.GetApplicationResult.reply_urls" title="Permalink to this definition">¶</a></dt>
<dd><p>A list of URLs that user tokens are sent to for sign in, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.ad.GetApplicationResult.id">
<code class="descname">id</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.ad.GetApplicationResult.id" title="Permalink to this definition">¶</a></dt>
<dd><p>id is the provider-assigned unique ID for this managed resource.</p>
</dd></dl>

</dd></dl>

<dl class="class">
<dt id="pulumi_azure.ad.GetServicePrincipalResult">
<em class="property">class </em><code class="descclassname">pulumi_azure.ad.</code><code class="descname">GetServicePrincipalResult</code><span class="sig-paren">(</span><em>application_id=None</em>, <em>display_name=None</em>, <em>object_id=None</em>, <em>id=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.ad.GetServicePrincipalResult" title="Permalink to this definition">¶</a></dt>
<dd><p>A collection of values returned by getServicePrincipal.</p>
<dl class="attribute">
<dt id="pulumi_azure.ad.GetServicePrincipalResult.id">
<code class="descname">id</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.ad.GetServicePrincipalResult.id" title="Permalink to this definition">¶</a></dt>
<dd><p>id is the provider-assigned unique ID for this managed resource.</p>
</dd></dl>

</dd></dl>

<dl class="class">
<dt id="pulumi_azure.ad.ServicePrincipal">
<em class="property">class </em><code class="descclassname">pulumi_azure.ad.</code><code class="descname">ServicePrincipal</code><span class="sig-paren">(</span><em>resource_name</em>, <em>opts=None</em>, <em>application_id=None</em>, <em>__props__=None</em>, <em>__name__=None</em>, <em>__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.ad.ServicePrincipal" title="Permalink to this definition">¶</a></dt>
<dd><p>Create a ServicePrincipal resource with the given unique name, props, and options.</p>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><ul class="first last simple">
<li><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</li>
<li><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</li>
<li><strong>application_id</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The ID of the Azure AD Application for which to create a Service Principal.</li>
</ul>
</td>
</tr>
</tbody>
</table>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/azuread_service_principal.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/azuread_service_principal.html.markdown</a>.</div></blockquote>
<dl class="attribute">
<dt id="pulumi_azure.ad.ServicePrincipal.application_id">
<code class="descname">application_id</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.ad.ServicePrincipal.application_id" title="Permalink to this definition">¶</a></dt>
<dd><p>The ID of the Azure AD Application for which to create a Service Principal.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.ad.ServicePrincipal.display_name">
<code class="descname">display_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.ad.ServicePrincipal.display_name" title="Permalink to this definition">¶</a></dt>
<dd><p>The Display Name of the Azure Active Directory Application associated with this Service Principal.</p>
</dd></dl>

<dl class="staticmethod">
<dt id="pulumi_azure.ad.ServicePrincipal.get">
<em class="property">static </em><code class="descname">get</code><span class="sig-paren">(</span><em>resource_name</em>, <em>id</em>, <em>opts=None</em>, <em>application_id=None</em>, <em>display_name=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.ad.ServicePrincipal.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing ServicePrincipal resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.
:param str resource_name: The unique name of the resulting resource.
:param str id: The unique provider ID of the resource to lookup.
:param pulumi.ResourceOptions opts: Options for the resource.
:param pulumi.Input[str] application_id: The ID of the Azure AD Application for which to create a Service Principal.
:param pulumi.Input[str] display_name: The Display Name of the Azure Active Directory Application associated with this Service Principal.</p>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/azuread_service_principal.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/azuread_service_principal.html.markdown</a>.</div></blockquote>
</dd></dl>

<dl class="method">
<dt id="pulumi_azure.ad.ServicePrincipal.translate_output_property">
<code class="descname">translate_output_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.ad.ServicePrincipal.translate_output_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_azure.ad.ServicePrincipal.translate_input_property">
<code class="descname">translate_input_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.ad.ServicePrincipal.translate_input_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_azure.ad.ServicePrincipalPassword">
<em class="property">class </em><code class="descclassname">pulumi_azure.ad.</code><code class="descname">ServicePrincipalPassword</code><span class="sig-paren">(</span><em>resource_name</em>, <em>opts=None</em>, <em>end_date=None</em>, <em>key_id=None</em>, <em>service_principal_id=None</em>, <em>start_date=None</em>, <em>value=None</em>, <em>__props__=None</em>, <em>__name__=None</em>, <em>__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.ad.ServicePrincipalPassword" title="Permalink to this definition">¶</a></dt>
<dd><p>Create a ServicePrincipalPassword resource with the given unique name, props, and options.</p>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><ul class="first last simple">
<li><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</li>
<li><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</li>
<li><strong>end_date</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The End Date which the Password is valid until, formatted as a RFC3339 date string (e.g. <code class="docutils literal notranslate"><span class="pre">2018-01-01T01:02:03Z</span></code>). Changing this field forces a new resource to be created.</li>
<li><strong>key_id</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – A GUID used to uniquely identify this Key. If not specified a GUID will be created. Changing this field forces a new resource to be created.</li>
<li><strong>service_principal_id</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The ID of the Service Principal for which this password should be created. Changing this field forces a new resource to be created.</li>
<li><strong>start_date</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The Start Date which the Password is valid from, formatted as a RFC3339 date string (e.g. <code class="docutils literal notranslate"><span class="pre">2018-01-01T01:02:03Z</span></code>). If this isn’t specified, the current date is used.  Changing this field forces a new resource to be created.</li>
<li><strong>value</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The Password for this Service Principal.</li>
</ul>
</td>
</tr>
</tbody>
</table>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/azuread_service_principal_password.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/azuread_service_principal_password.html.markdown</a>.</div></blockquote>
<dl class="attribute">
<dt id="pulumi_azure.ad.ServicePrincipalPassword.end_date">
<code class="descname">end_date</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.ad.ServicePrincipalPassword.end_date" title="Permalink to this definition">¶</a></dt>
<dd><p>The End Date which the Password is valid until, formatted as a RFC3339 date string (e.g. <code class="docutils literal notranslate"><span class="pre">2018-01-01T01:02:03Z</span></code>). Changing this field forces a new resource to be created.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.ad.ServicePrincipalPassword.key_id">
<code class="descname">key_id</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.ad.ServicePrincipalPassword.key_id" title="Permalink to this definition">¶</a></dt>
<dd><p>A GUID used to uniquely identify this Key. If not specified a GUID will be created. Changing this field forces a new resource to be created.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.ad.ServicePrincipalPassword.service_principal_id">
<code class="descname">service_principal_id</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.ad.ServicePrincipalPassword.service_principal_id" title="Permalink to this definition">¶</a></dt>
<dd><p>The ID of the Service Principal for which this password should be created. Changing this field forces a new resource to be created.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.ad.ServicePrincipalPassword.start_date">
<code class="descname">start_date</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.ad.ServicePrincipalPassword.start_date" title="Permalink to this definition">¶</a></dt>
<dd><p>The Start Date which the Password is valid from, formatted as a RFC3339 date string (e.g. <code class="docutils literal notranslate"><span class="pre">2018-01-01T01:02:03Z</span></code>). If this isn’t specified, the current date is used.  Changing this field forces a new resource to be created.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.ad.ServicePrincipalPassword.value">
<code class="descname">value</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.ad.ServicePrincipalPassword.value" title="Permalink to this definition">¶</a></dt>
<dd><p>The Password for this Service Principal.</p>
</dd></dl>

<dl class="staticmethod">
<dt id="pulumi_azure.ad.ServicePrincipalPassword.get">
<em class="property">static </em><code class="descname">get</code><span class="sig-paren">(</span><em>resource_name</em>, <em>id</em>, <em>opts=None</em>, <em>end_date=None</em>, <em>key_id=None</em>, <em>service_principal_id=None</em>, <em>start_date=None</em>, <em>value=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.ad.ServicePrincipalPassword.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing ServicePrincipalPassword resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.
:param str resource_name: The unique name of the resulting resource.
:param str id: The unique provider ID of the resource to lookup.
:param pulumi.ResourceOptions opts: Options for the resource.
:param pulumi.Input[str] end_date: The End Date which the Password is valid until, formatted as a RFC3339 date string (e.g. <code class="docutils literal notranslate"><span class="pre">2018-01-01T01:02:03Z</span></code>). Changing this field forces a new resource to be created.
:param pulumi.Input[str] key_id: A GUID used to uniquely identify this Key. If not specified a GUID will be created. Changing this field forces a new resource to be created.
:param pulumi.Input[str] service_principal_id: The ID of the Service Principal for which this password should be created. Changing this field forces a new resource to be created.
:param pulumi.Input[str] start_date: The Start Date which the Password is valid from, formatted as a RFC3339 date string (e.g. <code class="docutils literal notranslate"><span class="pre">2018-01-01T01:02:03Z</span></code>). If this isn’t specified, the current date is used.  Changing this field forces a new resource to be created.
:param pulumi.Input[str] value: The Password for this Service Principal.</p>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/azuread_service_principal_password.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/azuread_service_principal_password.html.markdown</a>.</div></blockquote>
</dd></dl>

<dl class="method">
<dt id="pulumi_azure.ad.ServicePrincipalPassword.translate_output_property">
<code class="descname">translate_output_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.ad.ServicePrincipalPassword.translate_output_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_azure.ad.ServicePrincipalPassword.translate_input_property">
<code class="descname">translate_input_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.ad.ServicePrincipalPassword.translate_input_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_azure.ad.get_application">
<code class="descclassname">pulumi_azure.ad.</code><code class="descname">get_application</code><span class="sig-paren">(</span><em>name=None</em>, <em>object_id=None</em>, <em>opts=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.ad.get_application" title="Permalink to this definition">¶</a></dt>
<dd><blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/d/azuread_application.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/d/azuread_application.html.markdown</a>.</div></blockquote>
</dd></dl>

<dl class="function">
<dt id="pulumi_azure.ad.get_service_principal">
<code class="descclassname">pulumi_azure.ad.</code><code class="descname">get_service_principal</code><span class="sig-paren">(</span><em>application_id=None</em>, <em>display_name=None</em>, <em>object_id=None</em>, <em>opts=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.ad.get_service_principal" title="Permalink to this definition">¶</a></dt>
<dd><blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/d/azuread_service_principal.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/d/azuread_service_principal.html.markdown</a>.</div></blockquote>
</dd></dl>

</div>
