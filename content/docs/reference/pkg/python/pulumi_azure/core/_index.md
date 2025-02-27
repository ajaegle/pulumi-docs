---
title: Module core
---

<div class="section" id="core">
<h1>core<a class="headerlink" href="#core" title="Permalink to this headline">¶</a></h1>
<blockquote>
<div>This provider is a derived work of the <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm">Terraform Provider</a> distributed under
<a class="reference external" href="https://www.mozilla.org/en-US/MPL/2.0/">MPL 2.0</a>. If you encounter a bug or missing feature, first check the
<a class="reference external" href="https://github.com/pulumi/pulumi-azure/issues">pulumi/pulumi-azure repo</a>; however, if that doesn’t turn up
anything, please consult the source <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/issues">terraform-providers/terraform-provider-azurerm repo</a>.</div></blockquote>
<span class="target" id="module-pulumi_azure.core"></span><dl class="class">
<dt id="pulumi_azure.core.AwaitableGetClientConfigResult">
<em class="property">class </em><code class="descclassname">pulumi_azure.core.</code><code class="descname">AwaitableGetClientConfigResult</code><span class="sig-paren">(</span><em>client_id=None</em>, <em>service_principal_application_id=None</em>, <em>service_principal_object_id=None</em>, <em>subscription_id=None</em>, <em>tenant_id=None</em>, <em>id=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.core.AwaitableGetClientConfigResult" title="Permalink to this definition">¶</a></dt>
<dd></dd></dl>

<dl class="class">
<dt id="pulumi_azure.core.AwaitableGetResourceGroupResult">
<em class="property">class </em><code class="descclassname">pulumi_azure.core.</code><code class="descname">AwaitableGetResourceGroupResult</code><span class="sig-paren">(</span><em>location=None</em>, <em>name=None</em>, <em>tags=None</em>, <em>id=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.core.AwaitableGetResourceGroupResult" title="Permalink to this definition">¶</a></dt>
<dd></dd></dl>

<dl class="class">
<dt id="pulumi_azure.core.AwaitableGetSubscriptionResult">
<em class="property">class </em><code class="descclassname">pulumi_azure.core.</code><code class="descname">AwaitableGetSubscriptionResult</code><span class="sig-paren">(</span><em>display_name=None</em>, <em>location_placement_id=None</em>, <em>quota_id=None</em>, <em>spending_limit=None</em>, <em>state=None</em>, <em>subscription_id=None</em>, <em>id=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.core.AwaitableGetSubscriptionResult" title="Permalink to this definition">¶</a></dt>
<dd></dd></dl>

<dl class="class">
<dt id="pulumi_azure.core.AwaitableGetSubscriptionsResult">
<em class="property">class </em><code class="descclassname">pulumi_azure.core.</code><code class="descname">AwaitableGetSubscriptionsResult</code><span class="sig-paren">(</span><em>display_name_contains=None</em>, <em>display_name_prefix=None</em>, <em>subscriptions=None</em>, <em>id=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.core.AwaitableGetSubscriptionsResult" title="Permalink to this definition">¶</a></dt>
<dd></dd></dl>

<dl class="class">
<dt id="pulumi_azure.core.AwaitableGetUserAssignedIdentityResult">
<em class="property">class </em><code class="descclassname">pulumi_azure.core.</code><code class="descname">AwaitableGetUserAssignedIdentityResult</code><span class="sig-paren">(</span><em>client_id=None</em>, <em>location=None</em>, <em>name=None</em>, <em>principal_id=None</em>, <em>resource_group_name=None</em>, <em>tags=None</em>, <em>id=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.core.AwaitableGetUserAssignedIdentityResult" title="Permalink to this definition">¶</a></dt>
<dd></dd></dl>

<dl class="class">
<dt id="pulumi_azure.core.GetClientConfigResult">
<em class="property">class </em><code class="descclassname">pulumi_azure.core.</code><code class="descname">GetClientConfigResult</code><span class="sig-paren">(</span><em>client_id=None</em>, <em>service_principal_application_id=None</em>, <em>service_principal_object_id=None</em>, <em>subscription_id=None</em>, <em>tenant_id=None</em>, <em>id=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.core.GetClientConfigResult" title="Permalink to this definition">¶</a></dt>
<dd><p>A collection of values returned by getClientConfig.</p>
<dl class="attribute">
<dt id="pulumi_azure.core.GetClientConfigResult.id">
<code class="descname">id</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.core.GetClientConfigResult.id" title="Permalink to this definition">¶</a></dt>
<dd><p>id is the provider-assigned unique ID for this managed resource.</p>
</dd></dl>

</dd></dl>

<dl class="class">
<dt id="pulumi_azure.core.GetResourceGroupResult">
<em class="property">class </em><code class="descclassname">pulumi_azure.core.</code><code class="descname">GetResourceGroupResult</code><span class="sig-paren">(</span><em>location=None</em>, <em>name=None</em>, <em>tags=None</em>, <em>id=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.core.GetResourceGroupResult" title="Permalink to this definition">¶</a></dt>
<dd><p>A collection of values returned by getResourceGroup.</p>
<dl class="attribute">
<dt id="pulumi_azure.core.GetResourceGroupResult.location">
<code class="descname">location</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.core.GetResourceGroupResult.location" title="Permalink to this definition">¶</a></dt>
<dd><p>The location of the resource group.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.core.GetResourceGroupResult.tags">
<code class="descname">tags</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.core.GetResourceGroupResult.tags" title="Permalink to this definition">¶</a></dt>
<dd><p>A mapping of tags assigned to the resource group.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.core.GetResourceGroupResult.id">
<code class="descname">id</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.core.GetResourceGroupResult.id" title="Permalink to this definition">¶</a></dt>
<dd><p>id is the provider-assigned unique ID for this managed resource.</p>
</dd></dl>

</dd></dl>

<dl class="class">
<dt id="pulumi_azure.core.GetSubscriptionResult">
<em class="property">class </em><code class="descclassname">pulumi_azure.core.</code><code class="descname">GetSubscriptionResult</code><span class="sig-paren">(</span><em>display_name=None</em>, <em>location_placement_id=None</em>, <em>quota_id=None</em>, <em>spending_limit=None</em>, <em>state=None</em>, <em>subscription_id=None</em>, <em>id=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.core.GetSubscriptionResult" title="Permalink to this definition">¶</a></dt>
<dd><p>A collection of values returned by getSubscription.</p>
<dl class="attribute">
<dt id="pulumi_azure.core.GetSubscriptionResult.display_name">
<code class="descname">display_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.core.GetSubscriptionResult.display_name" title="Permalink to this definition">¶</a></dt>
<dd><p>The subscription display name.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.core.GetSubscriptionResult.location_placement_id">
<code class="descname">location_placement_id</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.core.GetSubscriptionResult.location_placement_id" title="Permalink to this definition">¶</a></dt>
<dd><p>The subscription location placement ID.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.core.GetSubscriptionResult.quota_id">
<code class="descname">quota_id</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.core.GetSubscriptionResult.quota_id" title="Permalink to this definition">¶</a></dt>
<dd><p>The subscription quota ID.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.core.GetSubscriptionResult.spending_limit">
<code class="descname">spending_limit</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.core.GetSubscriptionResult.spending_limit" title="Permalink to this definition">¶</a></dt>
<dd><p>The subscription spending limit.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.core.GetSubscriptionResult.state">
<code class="descname">state</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.core.GetSubscriptionResult.state" title="Permalink to this definition">¶</a></dt>
<dd><p>The subscription state. Possible values are Enabled, Warned, PastDue, Disabled, and Deleted.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.core.GetSubscriptionResult.subscription_id">
<code class="descname">subscription_id</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.core.GetSubscriptionResult.subscription_id" title="Permalink to this definition">¶</a></dt>
<dd><p>The subscription GUID.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.core.GetSubscriptionResult.id">
<code class="descname">id</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.core.GetSubscriptionResult.id" title="Permalink to this definition">¶</a></dt>
<dd><p>id is the provider-assigned unique ID for this managed resource.</p>
</dd></dl>

</dd></dl>

<dl class="class">
<dt id="pulumi_azure.core.GetSubscriptionsResult">
<em class="property">class </em><code class="descclassname">pulumi_azure.core.</code><code class="descname">GetSubscriptionsResult</code><span class="sig-paren">(</span><em>display_name_contains=None</em>, <em>display_name_prefix=None</em>, <em>subscriptions=None</em>, <em>id=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.core.GetSubscriptionsResult" title="Permalink to this definition">¶</a></dt>
<dd><p>A collection of values returned by getSubscriptions.</p>
<dl class="attribute">
<dt id="pulumi_azure.core.GetSubscriptionsResult.subscriptions">
<code class="descname">subscriptions</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.core.GetSubscriptionsResult.subscriptions" title="Permalink to this definition">¶</a></dt>
<dd><p>One or more <code class="docutils literal notranslate"><span class="pre">subscription</span></code> blocks as defined below.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.core.GetSubscriptionsResult.id">
<code class="descname">id</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.core.GetSubscriptionsResult.id" title="Permalink to this definition">¶</a></dt>
<dd><p>id is the provider-assigned unique ID for this managed resource.</p>
</dd></dl>

</dd></dl>

<dl class="class">
<dt id="pulumi_azure.core.GetUserAssignedIdentityResult">
<em class="property">class </em><code class="descclassname">pulumi_azure.core.</code><code class="descname">GetUserAssignedIdentityResult</code><span class="sig-paren">(</span><em>client_id=None</em>, <em>location=None</em>, <em>name=None</em>, <em>principal_id=None</em>, <em>resource_group_name=None</em>, <em>tags=None</em>, <em>id=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.core.GetUserAssignedIdentityResult" title="Permalink to this definition">¶</a></dt>
<dd><p>A collection of values returned by getUserAssignedIdentity.</p>
<dl class="attribute">
<dt id="pulumi_azure.core.GetUserAssignedIdentityResult.client_id">
<code class="descname">client_id</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.core.GetUserAssignedIdentityResult.client_id" title="Permalink to this definition">¶</a></dt>
<dd><p>The Client ID of the User Assigned Identity.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.core.GetUserAssignedIdentityResult.location">
<code class="descname">location</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.core.GetUserAssignedIdentityResult.location" title="Permalink to this definition">¶</a></dt>
<dd><p>The Azure location where the User Assigned Identity exists.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.core.GetUserAssignedIdentityResult.principal_id">
<code class="descname">principal_id</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.core.GetUserAssignedIdentityResult.principal_id" title="Permalink to this definition">¶</a></dt>
<dd><p>The Service Principal ID of the User Assigned Identity.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.core.GetUserAssignedIdentityResult.tags">
<code class="descname">tags</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.core.GetUserAssignedIdentityResult.tags" title="Permalink to this definition">¶</a></dt>
<dd><p>A mapping of tags assigned to the User Assigned Identity.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.core.GetUserAssignedIdentityResult.id">
<code class="descname">id</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.core.GetUserAssignedIdentityResult.id" title="Permalink to this definition">¶</a></dt>
<dd><p>id is the provider-assigned unique ID for this managed resource.</p>
</dd></dl>

</dd></dl>

<dl class="class">
<dt id="pulumi_azure.core.ResourceGroup">
<em class="property">class </em><code class="descclassname">pulumi_azure.core.</code><code class="descname">ResourceGroup</code><span class="sig-paren">(</span><em>resource_name</em>, <em>opts=None</em>, <em>location=None</em>, <em>name=None</em>, <em>tags=None</em>, <em>__props__=None</em>, <em>__name__=None</em>, <em>__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.core.ResourceGroup" title="Permalink to this definition">¶</a></dt>
<dd><p>Manages a resource group on Azure.</p>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><ul class="first last simple">
<li><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</li>
<li><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</li>
<li><strong>location</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The location where the resource group should be created.
For a list of all Azure locations, please consult <a class="reference external" href="http://azure.microsoft.com/en-us/regions/">this link</a> or run <code class="docutils literal notranslate"><span class="pre">az</span> <span class="pre">account</span> <span class="pre">list-locations</span> <span class="pre">--output</span> <span class="pre">table</span></code>.</li>
<li><strong>name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The name of the resource group. Must be unique on your
Azure subscription.</li>
<li><strong>tags</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A mapping of tags to assign to the resource.</li>
</ul>
</td>
</tr>
</tbody>
</table>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/resource_group.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/resource_group.html.markdown</a>.</div></blockquote>
<dl class="attribute">
<dt id="pulumi_azure.core.ResourceGroup.location">
<code class="descname">location</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.core.ResourceGroup.location" title="Permalink to this definition">¶</a></dt>
<dd><p>The location where the resource group should be created.
For a list of all Azure locations, please consult <a class="reference external" href="http://azure.microsoft.com/en-us/regions/">this link</a> or run <code class="docutils literal notranslate"><span class="pre">az</span> <span class="pre">account</span> <span class="pre">list-locations</span> <span class="pre">--output</span> <span class="pre">table</span></code>.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.core.ResourceGroup.name">
<code class="descname">name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.core.ResourceGroup.name" title="Permalink to this definition">¶</a></dt>
<dd><p>The name of the resource group. Must be unique on your
Azure subscription.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.core.ResourceGroup.tags">
<code class="descname">tags</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.core.ResourceGroup.tags" title="Permalink to this definition">¶</a></dt>
<dd><p>A mapping of tags to assign to the resource.</p>
</dd></dl>

<dl class="staticmethod">
<dt id="pulumi_azure.core.ResourceGroup.get">
<em class="property">static </em><code class="descname">get</code><span class="sig-paren">(</span><em>resource_name</em>, <em>id</em>, <em>opts=None</em>, <em>location=None</em>, <em>name=None</em>, <em>tags=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.core.ResourceGroup.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing ResourceGroup resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.
:param str resource_name: The unique name of the resulting resource.
:param str id: The unique provider ID of the resource to lookup.
:param pulumi.ResourceOptions opts: Options for the resource.
:param pulumi.Input[str] location: The location where the resource group should be created.</p>
<blockquote>
<div>For a list of all Azure locations, please consult <a class="reference external" href="http://azure.microsoft.com/en-us/regions/">this link</a> or run <code class="docutils literal notranslate"><span class="pre">az</span> <span class="pre">account</span> <span class="pre">list-locations</span> <span class="pre">--output</span> <span class="pre">table</span></code>.</div></blockquote>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><ul class="first last simple">
<li><strong>name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The name of the resource group. Must be unique on your
Azure subscription.</li>
<li><strong>tags</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A mapping of tags to assign to the resource.</li>
</ul>
</td>
</tr>
</tbody>
</table>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/resource_group.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/resource_group.html.markdown</a>.</div></blockquote>
</dd></dl>

<dl class="method">
<dt id="pulumi_azure.core.ResourceGroup.translate_output_property">
<code class="descname">translate_output_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.core.ResourceGroup.translate_output_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_azure.core.ResourceGroup.translate_input_property">
<code class="descname">translate_input_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.core.ResourceGroup.translate_input_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_azure.core.TemplateDeployment">
<em class="property">class </em><code class="descclassname">pulumi_azure.core.</code><code class="descname">TemplateDeployment</code><span class="sig-paren">(</span><em>resource_name</em>, <em>opts=None</em>, <em>deployment_mode=None</em>, <em>name=None</em>, <em>parameters=None</em>, <em>parameters_body=None</em>, <em>resource_group_name=None</em>, <em>template_body=None</em>, <em>__props__=None</em>, <em>__name__=None</em>, <em>__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.core.TemplateDeployment" title="Permalink to this definition">¶</a></dt>
<dd><p>Manage a template deployment of resources</p>
<blockquote>
<div><strong>Note on ARM Template Deployments:</strong> Due to the way the underlying Azure API is designed, this provider can only manage the deployment of the ARM Template - and not any resources which are created by it.
This means that when deleting the <code class="docutils literal notranslate"><span class="pre">core.TemplateDeployment</span></code> resource, this provider will only remove the reference to the deployment, whilst leaving any resources created by that ARM Template Deployment.
One workaround for this is to use a unique Resource Group for each ARM Template Deployment, which means deleting the Resource Group would contain any resources created within it - however this isn’t ideal. <a class="reference external" href="https://docs.microsoft.com/en-us/rest/api/resources/deployments#Deployments_Delete">More information</a>.</div></blockquote>
<p>This provider does not know about the individual resources created by Azure using a deployment template and therefore cannot delete these resources during a destroy. Destroying a template deployment removes the associated deployment operations, but will not delete the Azure resources created by the deployment. In order to delete these resources, the containing resource group must also be destroyed. <a class="reference external" href="https://docs.microsoft.com/en-us/rest/api/resources/deployments#Deployments_Delete">More information</a>.</p>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><ul class="first last simple">
<li><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</li>
<li><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</li>
<li><strong>deployment_mode</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Specifies the mode that is used to deploy resources. This value could be either <code class="docutils literal notranslate"><span class="pre">Incremental</span></code> or <code class="docutils literal notranslate"><span class="pre">Complete</span></code>.
Note that you will almost <em>always</em> want this to be set to <code class="docutils literal notranslate"><span class="pre">Incremental</span></code> otherwise the deployment will destroy all infrastructure not
specified within the template, and this provider will not be aware of this.</li>
<li><strong>name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Specifies the name of the template deployment. Changing this forces a
new resource to be created.</li>
<li><strong>parameters</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – Specifies the name and value pairs that define the deployment parameters for the template.</li>
<li><strong>parameters_body</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Specifies a valid Azure JSON parameters file that define the deployment parameters. It can contain KeyVault references</li>
<li><strong>resource_group_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The name of the resource group in which to
create the template deployment.</li>
<li><strong>template_body</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Specifies the JSON definition for the template.</li>
</ul>
</td>
</tr>
</tbody>
</table>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/template_deployment.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/template_deployment.html.markdown</a>.</div></blockquote>
<dl class="attribute">
<dt id="pulumi_azure.core.TemplateDeployment.deployment_mode">
<code class="descname">deployment_mode</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.core.TemplateDeployment.deployment_mode" title="Permalink to this definition">¶</a></dt>
<dd><p>Specifies the mode that is used to deploy resources. This value could be either <code class="docutils literal notranslate"><span class="pre">Incremental</span></code> or <code class="docutils literal notranslate"><span class="pre">Complete</span></code>.
Note that you will almost <em>always</em> want this to be set to <code class="docutils literal notranslate"><span class="pre">Incremental</span></code> otherwise the deployment will destroy all infrastructure not
specified within the template, and this provider will not be aware of this.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.core.TemplateDeployment.name">
<code class="descname">name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.core.TemplateDeployment.name" title="Permalink to this definition">¶</a></dt>
<dd><p>Specifies the name of the template deployment. Changing this forces a
new resource to be created.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.core.TemplateDeployment.outputs">
<code class="descname">outputs</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.core.TemplateDeployment.outputs" title="Permalink to this definition">¶</a></dt>
<dd><p>A map of supported scalar output types returned from the deployment (currently, Azure Template Deployment outputs of type String, Int and Bool are supported, and are converted to strings - others will be ignored) and can be accessed using <code class="docutils literal notranslate"><span class="pre">.outputs[&quot;name&quot;]</span></code>.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.core.TemplateDeployment.parameters">
<code class="descname">parameters</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.core.TemplateDeployment.parameters" title="Permalink to this definition">¶</a></dt>
<dd><p>Specifies the name and value pairs that define the deployment parameters for the template.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.core.TemplateDeployment.parameters_body">
<code class="descname">parameters_body</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.core.TemplateDeployment.parameters_body" title="Permalink to this definition">¶</a></dt>
<dd><p>Specifies a valid Azure JSON parameters file that define the deployment parameters. It can contain KeyVault references</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.core.TemplateDeployment.resource_group_name">
<code class="descname">resource_group_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.core.TemplateDeployment.resource_group_name" title="Permalink to this definition">¶</a></dt>
<dd><p>The name of the resource group in which to
create the template deployment.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.core.TemplateDeployment.template_body">
<code class="descname">template_body</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.core.TemplateDeployment.template_body" title="Permalink to this definition">¶</a></dt>
<dd><p>Specifies the JSON definition for the template.</p>
</dd></dl>

<dl class="staticmethod">
<dt id="pulumi_azure.core.TemplateDeployment.get">
<em class="property">static </em><code class="descname">get</code><span class="sig-paren">(</span><em>resource_name</em>, <em>id</em>, <em>opts=None</em>, <em>deployment_mode=None</em>, <em>name=None</em>, <em>outputs=None</em>, <em>parameters=None</em>, <em>parameters_body=None</em>, <em>resource_group_name=None</em>, <em>template_body=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.core.TemplateDeployment.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing TemplateDeployment resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.
:param str resource_name: The unique name of the resulting resource.
:param str id: The unique provider ID of the resource to lookup.
:param pulumi.ResourceOptions opts: Options for the resource.
:param pulumi.Input[str] deployment_mode: Specifies the mode that is used to deploy resources. This value could be either <code class="docutils literal notranslate"><span class="pre">Incremental</span></code> or <code class="docutils literal notranslate"><span class="pre">Complete</span></code>.</p>
<blockquote>
<div>Note that you will almost <em>always</em> want this to be set to <code class="docutils literal notranslate"><span class="pre">Incremental</span></code> otherwise the deployment will destroy all infrastructure not
specified within the template, and this provider will not be aware of this.</div></blockquote>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><ul class="first last simple">
<li><strong>name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Specifies the name of the template deployment. Changing this forces a
new resource to be created.</li>
<li><strong>outputs</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A map of supported scalar output types returned from the deployment (currently, Azure Template Deployment outputs of type String, Int and Bool are supported, and are converted to strings - others will be ignored) and can be accessed using <code class="docutils literal notranslate"><span class="pre">.outputs[&quot;name&quot;]</span></code>.</li>
<li><strong>parameters</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – Specifies the name and value pairs that define the deployment parameters for the template.</li>
<li><strong>parameters_body</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Specifies a valid Azure JSON parameters file that define the deployment parameters. It can contain KeyVault references</li>
<li><strong>resource_group_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The name of the resource group in which to
create the template deployment.</li>
<li><strong>template_body</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Specifies the JSON definition for the template.</li>
</ul>
</td>
</tr>
</tbody>
</table>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/template_deployment.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/template_deployment.html.markdown</a>.</div></blockquote>
</dd></dl>

<dl class="method">
<dt id="pulumi_azure.core.TemplateDeployment.translate_output_property">
<code class="descname">translate_output_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.core.TemplateDeployment.translate_output_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_azure.core.TemplateDeployment.translate_input_property">
<code class="descname">translate_input_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.core.TemplateDeployment.translate_input_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_azure.core.get_client_config">
<code class="descclassname">pulumi_azure.core.</code><code class="descname">get_client_config</code><span class="sig-paren">(</span><em>opts=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.core.get_client_config" title="Permalink to this definition">¶</a></dt>
<dd><p>Use this data source to access the configuration of the AzureRM provider.</p>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/d/client_config.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/d/client_config.html.markdown</a>.</div></blockquote>
</dd></dl>

<dl class="function">
<dt id="pulumi_azure.core.get_resource_group">
<code class="descclassname">pulumi_azure.core.</code><code class="descname">get_resource_group</code><span class="sig-paren">(</span><em>name=None</em>, <em>opts=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.core.get_resource_group" title="Permalink to this definition">¶</a></dt>
<dd><p>Use this data source to access information about an existing Resource Group.</p>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/d/resource_group.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/d/resource_group.html.markdown</a>.</div></blockquote>
</dd></dl>

<dl class="function">
<dt id="pulumi_azure.core.get_subscription">
<code class="descclassname">pulumi_azure.core.</code><code class="descname">get_subscription</code><span class="sig-paren">(</span><em>subscription_id=None</em>, <em>opts=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.core.get_subscription" title="Permalink to this definition">¶</a></dt>
<dd><p>Use this data source to access information about an existing Subscription.</p>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/d/subscription.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/d/subscription.html.markdown</a>.</div></blockquote>
</dd></dl>

<dl class="function">
<dt id="pulumi_azure.core.get_subscriptions">
<code class="descclassname">pulumi_azure.core.</code><code class="descname">get_subscriptions</code><span class="sig-paren">(</span><em>display_name_contains=None</em>, <em>display_name_prefix=None</em>, <em>opts=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.core.get_subscriptions" title="Permalink to this definition">¶</a></dt>
<dd><p>Use this data source to access information about all the Subscriptions currently available.</p>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/d/subscriptions.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/d/subscriptions.html.markdown</a>.</div></blockquote>
</dd></dl>

<dl class="function">
<dt id="pulumi_azure.core.get_user_assigned_identity">
<code class="descclassname">pulumi_azure.core.</code><code class="descname">get_user_assigned_identity</code><span class="sig-paren">(</span><em>name=None</em>, <em>resource_group_name=None</em>, <em>opts=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.core.get_user_assigned_identity" title="Permalink to this definition">¶</a></dt>
<dd><p>Use this data source to access information about an existing User Assigned Identity.</p>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/d/user_assigned_identity.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/d/user_assigned_identity.html.markdown</a>.</div></blockquote>
</dd></dl>

</div>
