---
title: Azure AD Graph と Microsoft Graph の間の相違を要求する
description: Microsoft Graph 要求と Azure AD 要求との相違について説明します。これは、アプリを新しいサービスに移行する際に役に立ちます。.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f046043b6a30d66cef96bb6eb6192bddd90d2f5f
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33630210"
---
# <a name="request-differences-between-azure-ad-graph-and-microsoft-graph"></a><span data-ttu-id="bfa8b-103">Azure AD Graph と Microsoft Graph の間の相違を要求する</span><span class="sxs-lookup"><span data-stu-id="bfa8b-103">Request differences between Azure AD Graph and Microsoft Graph</span></span>

<span data-ttu-id="bfa8b-104">この記事は、*手順 1:* [アプリを移行するプロセス](migrate-azure-ad-graph-planning-checklist.md)の API の相違点を確認します。</span><span class="sxs-lookup"><span data-stu-id="bfa8b-104">This article is part of *step 1: review API differences* of the [process to migrate apps](migrate-azure-ad-graph-planning-checklist.md).</span></span>

<span data-ttu-id="bfa8b-105">Microsoft Graph および Azure AD Graph API はどちらも REST Api であり、それぞれがクエリパラメーターの ODATA 規則をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="bfa8b-105">Microsoft Graph and the Azure AD Graph API are both REST APIs and they each support ODATA conventions for query parameters.</span></span> <span data-ttu-id="bfa8b-106">ただし、この2つの Api の構文は異なります。</span><span class="sxs-lookup"><span data-stu-id="bfa8b-106">However, the syntax varies between these two APIs.</span></span>

<span data-ttu-id="bfa8b-107">[グラフエクスプローラー](https://aka.ms/ge)を使用して、要求と応答の違いについて理解するための最適な方法として、自分のデータに対してこれらの要求パターンを試してみてください。</span><span class="sxs-lookup"><span data-stu-id="bfa8b-107">Use the [Graph Explorer](https://aka.ms/ge) to try these request patterns against your own data, as it's a great way to learn about the request and response differences.</span></span>

## <a name="basic-requests"></a><span data-ttu-id="bfa8b-108">基本的な要求</span><span class="sxs-lookup"><span data-stu-id="bfa8b-108">Basic requests</span></span>

<span data-ttu-id="bfa8b-109">次の表は、2つの Api の主な要求の違いを示しています。</span><span class="sxs-lookup"><span data-stu-id="bfa8b-109">The following table highlights the main request differences between the two APIs:</span></span>

|| <span data-ttu-id="bfa8b-110">Azure AD Graph</span><span class="sxs-lookup"><span data-stu-id="bfa8b-110">Azure AD Graph</span></span> | <span data-ttu-id="bfa8b-111">Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="bfa8b-111">Microsoft Graph</span></span> |
|---|---|---|
|<span data-ttu-id="bfa8b-112">要求の構文</span><span class="sxs-lookup"><span data-stu-id="bfa8b-112">Request syntax</span></span>| `https://graph.windows.net/{tenant_id}/` <br> `{resource}?{version}&query-parameters` | `https://graph.microsoft.com/`<br>`{version}/{resource}?query-parameters`|
|<span data-ttu-id="bfa8b-113">サービス&nbsp;エンドポイント:</span><span class="sxs-lookup"><span data-stu-id="bfa8b-113">Service&nbsp;endpoints:</span></span>||
|<span data-ttu-id="bfa8b-114">-&nbsp;全体</span><span class="sxs-lookup"><span data-stu-id="bfa8b-114">-&nbsp;Global</span></span>|`https://graph.windows.net`|`https://graph.microsoft.com`|
|<span data-ttu-id="bfa8b-115">-&nbsp;US&nbsp;Gov&nbsp;L4</span><span class="sxs-lookup"><span data-stu-id="bfa8b-115">-&nbsp;US&nbsp;Gov&nbsp;L4</span></span>|`https://graph.microsoftazure.us`|`https://graph.microsoft.us`|
|<span data-ttu-id="bfa8b-116">-&nbsp;US&nbsp;Gov&nbsp;L5&nbsp;(DOD)</span><span class="sxs-lookup"><span data-stu-id="bfa8b-116">-&nbsp;US&nbsp;Gov&nbsp;L5&nbsp;(DOD)</span></span>|`https://graph.microsoftazure.us`|`https://dod-graph.microsoft.us`|
|<span data-ttu-id="bfa8b-117">-&nbsp;ドイツ</span><span class="sxs-lookup"><span data-stu-id="bfa8b-117">-&nbsp;Germany</span></span>|`https://graph.cloudapi.de`|`https://graph.microsoft.de`|
|<span data-ttu-id="bfa8b-118">-&nbsp;中国&nbsp;(21vianet)</span><span class="sxs-lookup"><span data-stu-id="bfa8b-118">-&nbsp;China&nbsp;(21Vianet)</span></span>| `https://graph.chinacloudapi.cn`|`https://microsoftgraph.chinacloudapi.cn`|
|<span data-ttu-id="bfa8b-119">{tenant_id}</span><span class="sxs-lookup"><span data-stu-id="bfa8b-119">{tenant_id}</span></span>|<span data-ttu-id="bfa8b-120">要求内のテナントの ID を指定します。</span><span class="sxs-lookup"><span data-stu-id="bfa8b-120">Specify the ID of the tenant in the request.</span></span>|<span data-ttu-id="bfa8b-121">要求では、アクセストークンから推論されるときに、テナント ID を指定することはオプションです。</span><span class="sxs-lookup"><span data-stu-id="bfa8b-121">It's optional to specify a tenant ID in the request as it is inferred from the access token.</span></span><br><br><span data-ttu-id="bfa8b-122">テナント ID を指定する`{version}`と、はとの間`{resource}`で要求 URL になります。</span><span class="sxs-lookup"><span data-stu-id="bfa8b-122">If you specify the tenant ID, it goes between the `{version}` and the `{resource}` in the request URL.</span></span>|
|<span data-ttu-id="bfa8b-123">4.0</span><span class="sxs-lookup"><span data-stu-id="bfa8b-123">{version}</span></span>|<span data-ttu-id="bfa8b-124">必要なクエリパラメーターを使用して、要求に Azure AD Graph のリリースバージョンを指定します。</span><span class="sxs-lookup"><span data-stu-id="bfa8b-124">Specify the release version of Azure AD Graph in the request using a required query parameter.</span></span>|<span data-ttu-id="bfa8b-125">要求では、サービスエンドポイントの直後の URL パスの一部として、Microsoft Graph のリリースバージョンを指定します。</span><span class="sxs-lookup"><span data-stu-id="bfa8b-125">Specify the release version of Microsoft Graph in the request as part of the URL path just after the service endpoint.</span></span>|

<span data-ttu-id="bfa8b-126">Microsoft Graph では、Azure AD Graph と同じクエリパラメーターを引き続き使用できます。</span><span class="sxs-lookup"><span data-stu-id="bfa8b-126">You can continue to use the same query parameters in Microsoft Graph as Azure AD Graph.</span></span>

### <a name="example-request-comparison"></a><span data-ttu-id="bfa8b-127">要求の比較の例</span><span class="sxs-lookup"><span data-stu-id="bfa8b-127">Example request comparison</span></span>

<span data-ttu-id="bfa8b-128">"Dan" で始まる名前を持つすべてのユーザーの一覧を作成するとします。</span><span class="sxs-lookup"><span data-stu-id="bfa8b-128">Suppose you want a list of all users with names beginning with "Dan".</span></span>

<span data-ttu-id="bfa8b-129">Azure AD Graph では、次の要求を使用できます。</span><span class="sxs-lookup"><span data-stu-id="bfa8b-129">In Azure AD Graph, you might use this request:</span></span>

`https://graph.windows.net/contoso.com/users?$filter=startswith(givenName,'Dan')&api-version=1.6`

<span data-ttu-id="bfa8b-130">この要求:</span><span class="sxs-lookup"><span data-stu-id="bfa8b-130">This request:</span></span>

- <span data-ttu-id="bfa8b-131">Azure AD Graph のバージョン1.6 を対象としています。</span><span class="sxs-lookup"><span data-stu-id="bfa8b-131">Targets version 1.6 of Azure AD Graph.</span></span>  
- <span data-ttu-id="bfa8b-132">テナント`contoso.com` ID としてを指定します。</span><span class="sxs-lookup"><span data-stu-id="bfa8b-132">Specifies `contoso.com` as the tenant ID.</span></span>  
- <span data-ttu-id="bfa8b-133">ユーザーリソースを呼び出します。</span><span class="sxs-lookup"><span data-stu-id="bfa8b-133">Calls the users resource.</span></span>  
- <span data-ttu-id="bfa8b-134">は、 `$filter`クエリパラメーターを使用して、指定された名前`Dan`ので始まる応答を制限します。</span><span class="sxs-lookup"><span data-stu-id="bfa8b-134">Uses the `$filter` query parameter to limit the response to given names that begin with `Dan`.</span></span>  

<span data-ttu-id="bfa8b-135">結果には、Daniel、Danforth、Danielle、Danerys などの名前を持つユーザーが含まれます。</span><span class="sxs-lookup"><span data-stu-id="bfa8b-135">Results include users with names like Daniel, Danforth, Danielle, Danerys, and so on.</span></span>

<span data-ttu-id="bfa8b-136">Microsoft Graph については、次のような要求があります。</span><span class="sxs-lookup"><span data-stu-id="bfa8b-136">A similar request for Microsoft Graph would be:</span></span>

`https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName,'Dan')`

<span data-ttu-id="bfa8b-137">ここは：</span><span class="sxs-lookup"><span data-stu-id="bfa8b-137">Here:</span></span>

- <span data-ttu-id="bfa8b-138">バージョンは`v1.0`です。</span><span class="sxs-lookup"><span data-stu-id="bfa8b-138">The version is `v1.0`.</span></span>  
- <span data-ttu-id="bfa8b-139">テナント ID は、アクセストークンから推論されます (ここでは示されていません)。</span><span class="sxs-lookup"><span data-stu-id="bfa8b-139">The tenant ID is inferred from the access token (not shown).</span></span>  
- <span data-ttu-id="bfa8b-140">Resource パラメーターと`$filter` query パラメーターは Azure AD クエリと同じです。</span><span class="sxs-lookup"><span data-stu-id="bfa8b-140">The resource and `$filter` query parameter are the same as the Azure AD query.</span></span>  

> <span data-ttu-id="bfa8b-141">**注**: Azure AD Graph .net クライアントライブラリを使用している場合は、詳細については「 [.net クライアントライブラリ](migrate-azure-ad-graph-client-libraries.md)」を参照し、Microsoft Graph .net クライアントライブラリに移動する方法について参照してください。</span><span class="sxs-lookup"><span data-stu-id="bfa8b-141">**NOTE**: If you're using the Azure AD Graph .NET client library, see [.NET client libraries](migrate-azure-ad-graph-client-libraries.md) for more specific strategies and assistance to move to the Microsoft Graph .NET client library.</span></span>

### <a name="key-identifiers-objectid-vs-id"></a><span data-ttu-id="bfa8b-142">キー識別子: objectId vs id</span><span class="sxs-lookup"><span data-stu-id="bfa8b-142">Key identifiers: objectId vs id</span></span>

<span data-ttu-id="bfa8b-143">Azure AD Graph では、すべてのエンティティのリソース型には、 **objectId**という一意の識別子 (またはキー) があります。</span><span class="sxs-lookup"><span data-stu-id="bfa8b-143">In Azure AD Graph, all entity resource types have a unique identifier (or key) called **objectId**.</span></span>  <span data-ttu-id="bfa8b-144">ほとんどの場合 (特に明記されていない限り)、同じ識別子が Microsoft Graph では**id**と呼ばれます。</span><span class="sxs-lookup"><span data-stu-id="bfa8b-144">For the most part (unless otherwise stated) this same identifier is called **id** in Microsoft Graph.</span></span>

## <a name="default-properties-and-select"></a><span data-ttu-id="bfa8b-145">既定のプロパティと $select</span><span class="sxs-lookup"><span data-stu-id="bfa8b-145">Default properties and $select</span></span>

<span data-ttu-id="bfa8b-146">GET 要求`$select`でクエリパラメーターを使用して、アプリが必要とするすべてのプロパティを含むように応答をカスタマイズします。</span><span class="sxs-lookup"><span data-stu-id="bfa8b-146">Use the `$select` query parameter, in GET requests, to customize the response to include all the properties that your app requires.</span></span>

<span data-ttu-id="bfa8b-147">Microsoft Graph の**get**または**list**操作ユーザーまたはグループのリソースは、すべてのプロパティのサブセットを返します (_既定のプロパティ_と呼ばれます)。</span><span class="sxs-lookup"><span data-stu-id="bfa8b-147">Microsoft Graph **get** or **list** operations for user or group resources returns only a subset of all properties, known as the _default properties_.</span></span> <span data-ttu-id="bfa8b-148">既定のプロパティは、リソースでよく使用されるプロパティを表します。</span><span class="sxs-lookup"><span data-stu-id="bfa8b-148">The default properties represent the most commonly-used properties for a resource.</span></span> <span data-ttu-id="bfa8b-149">一方、Azure AD Graph は、それぞれのリソースのすべてのプロパティの完全なセットを返します。</span><span class="sxs-lookup"><span data-stu-id="bfa8b-149">On the other hand, Azure AD Graph returns the full set of all properties for the respective resource.</span></span>

<span data-ttu-id="bfa8b-150">V 1.0 のその他のプロパティを取得するには、 `$select`クエリパラメーターを使用して、アプリで明示的に要求する必要があります。</span><span class="sxs-lookup"><span data-stu-id="bfa8b-150">To get other properties in v1.0, your app needs to explicitly request them, using the `$select` query parameter.</span></span> <span data-ttu-id="bfa8b-151">これには、アプリが使用している可能性のあるディレクトリスキーマの拡張機能が含まれます。</span><span class="sxs-lookup"><span data-stu-id="bfa8b-151">This includes any directory schema extensions your app might be using.</span></span> <span data-ttu-id="bfa8b-152">アプリに実際に必要なプロパティのみを要求することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="bfa8b-152">It's a best practice to only request the properties your app really needs.</span></span>

<span data-ttu-id="bfa8b-153">違いを説明するために、Graph エクスプローラーを使用して次の要求を実行し、異なる応答を比較します。</span><span class="sxs-lookup"><span data-stu-id="bfa8b-153">To illustrate the difference, use Graph Explorer to run the following requests and compare the different responses.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/
GET https://graph.microsoft.com/beta/me/
```

<span data-ttu-id="bfa8b-154">各クエリからの応答を確認します。</span><span class="sxs-lookup"><span data-stu-id="bfa8b-154">Review the responses from each query.</span></span> <span data-ttu-id="bfa8b-155">アドレス情報は、ベータ版では返されますが、/v1.0 のバージョンでは返されないことに注意してください。</span><span class="sxs-lookup"><span data-stu-id="bfa8b-155">You'll notice that address information is returned by the /beta version, but not the /v1.0 version.</span></span>  <span data-ttu-id="bfa8b-156">これは、アドレスプロパティが既定のプロパティセットに含まれていないためです。</span><span class="sxs-lookup"><span data-stu-id="bfa8b-156">That's because the address properties aren't in the default property set.</span></span>

<span data-ttu-id="bfa8b-157">アプリがアドレスプロパティに依存している場合は、次の`$select`ように、version 1.0 要求を更新してクエリパラメーターを含める必要があります。</span><span class="sxs-lookup"><span data-stu-id="bfa8b-157">If your app relies on the address properties, you need to update your v1.0 requests to include the `$select` query parameter:</span></span>

```http
https://graph.microsoft.com/v1.0/me/?$select=displayName,streetAddress,city,state,postalCode
```

<span data-ttu-id="bfa8b-158">この要求に対する応答には、アドレスのプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="bfa8b-158">The response for this request would include the address properties.</span></span>  <span data-ttu-id="bfa8b-159">**DisplayName**プロパティも含まれていますが、クエリパラメーターで指定されているためです。</span><span class="sxs-lookup"><span data-stu-id="bfa8b-159">It also includes the **displayName** property, but only because it was specified by the query parameter.</span></span>

<span data-ttu-id="bfa8b-160">詳細については、次の情報を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bfa8b-160">To learn more about:</span></span>

- <span data-ttu-id="bfa8b-161">ユーザーの既定のプロパティ。「[ユーザー](/graph/api/resources/users?view=graph-rest-1.0) 」を参照</span><span class="sxs-lookup"><span data-stu-id="bfa8b-161">Default properties on user, see [users](/graph/api/resources/users?view=graph-rest-1.0)</span></span>
- <span data-ttu-id="bfa8b-162">`$select`パラメーターおよびその他のサポートされる ODATA クエリパラメーターについては、「[クエリパラメーターを使用して応答をカスタマイズする](/graph/query-parameters)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bfa8b-162">The `$select` parameter and other supported ODATA query parameters, see [Use query parameters to customize responses](/graph/query-parameters).</span></span>
- <span data-ttu-id="bfa8b-163">この他の推奨される最適化については、「[ベストプラクティス](/graph/best-practices-concept)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bfa8b-163">This and other recommended optimizations, see [Best practices](/graph/best-practices-concept).</span></span>

## <a name="relationships-and-navigation-properties"></a><span data-ttu-id="bfa8b-164">リレーションシップとナビゲーションプロパティ</span><span class="sxs-lookup"><span data-stu-id="bfa8b-164">Relationships and navigation properties</span></span>

<span data-ttu-id="bfa8b-165">リレーションシップ (またはナビゲーションプロパティ) は、Azure AD Graph と Microsoft Graph の重要な概念であり、関連するリソースのネットワークを作成します。</span><span class="sxs-lookup"><span data-stu-id="bfa8b-165">Relationships (or navigation properties) are a key concept in Azure AD Graph and Microsoft Graph, creating a network of related resources.</span></span> <span data-ttu-id="bfa8b-166">たとえば、**マネージャー**および**directreports**プロパティは、ユーザーリソースを拡張して組織階層を提供します。</span><span class="sxs-lookup"><span data-stu-id="bfa8b-166">For example, the **manager** and **directReports** properties extend the user resource to provide organizational hierarchy.</span></span>  

<span data-ttu-id="bfa8b-167">また、関係は、ユーザーが属するグループ、グループまたはディレクトリの役割に属するメンバーなどのメンバーシップも定義します。</span><span class="sxs-lookup"><span data-stu-id="bfa8b-167">Relationships also define memberships, such as the groups a user belongs to, the members belonging to a group or a directory role, and so on.</span></span>

<span data-ttu-id="bfa8b-168">Azure AD Graph 要求は`$link` 、リソース間の関係を示すために使用します。</span><span class="sxs-lookup"><span data-stu-id="bfa8b-168">Azure AD Graph requests use `$link` to indicate relationships between resources.</span></span>  <span data-ttu-id="bfa8b-169">Microsoft Graph では、代わりに ODATA 4.01 `$ref`表記を使用します。</span><span class="sxs-lookup"><span data-stu-id="bfa8b-169">In Microsoft Graph this uses the ODATA 4.01 `$ref` notation instead.</span></span>

<span data-ttu-id="bfa8b-170">次の表は、いくつかの例を示しています。</span><span class="sxs-lookup"><span data-stu-id="bfa8b-170">The following table shows several examples:</span></span>

| <span data-ttu-id="bfa8b-171">タスク</span><span class="sxs-lookup"><span data-stu-id="bfa8b-171">Task</span></span> | <span data-ttu-id="bfa8b-172">Azure AD Graph</span><span class="sxs-lookup"><span data-stu-id="bfa8b-172">Azure AD Graph</span></span> | <span data-ttu-id="bfa8b-173">Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="bfa8b-173">Microsoft Graph</span></span> |
|------|----------------|-----------------|
| <span data-ttu-id="bfa8b-174">メンバーを追加する</span><span class="sxs-lookup"><span data-stu-id="bfa8b-174">Add member</span></span>        | ```POST /groups/{id}/$link/members```        | ```POST /groups/{id}/members/$ref```        |
| <span data-ttu-id="bfa8b-175">メンバーリンクの一覧表示</span><span class="sxs-lookup"><span data-stu-id="bfa8b-175">List member links</span></span> | ```GET /groups/{id}/$link/members```         | ```GET /groups/{id}/members/$ref```         |
| <span data-ttu-id="bfa8b-176">メンバーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="bfa8b-176">List members</span></span>      | ```GET /groups/{id}/members```                | ```GET /groups/{id}/members```               |
| <span data-ttu-id="bfa8b-177">メンバーを削除する</span><span class="sxs-lookup"><span data-stu-id="bfa8b-177">Remove member</span></span>     | ```DELETE /groups/{id}/$link/members/{id}``` | ```DELETE /groups/{id}/members/{id}/$ref``` |

<span data-ttu-id="bfa8b-178">アプリを Microsoft Graph に移行する場合は、リソースの関連付け`$link`に使用する要求を探します。代わりにを使用`$ref`するように変更します。</span><span class="sxs-lookup"><span data-stu-id="bfa8b-178">When migrating your apps to Microsoft Graph, look for requests that use `$link` to associate resources; change these to use `$ref` instead.</span></span>

## <a name="next-steps"></a><span data-ttu-id="bfa8b-179">次のステップ</span><span class="sxs-lookup"><span data-stu-id="bfa8b-179">Next Steps</span></span>

- <span data-ttu-id="bfa8b-180">Azure AD Graph と Microsoft Graph の[サービス機能の違い](migrate-azure-ad-graph-feature-differences.md)について説明します。</span><span class="sxs-lookup"><span data-stu-id="bfa8b-180">Learn about [service feature differences](migrate-azure-ad-graph-feature-differences.md) between Azure AD Graph and Microsoft Graph.</span></span>
- <span data-ttu-id="bfa8b-181">[Microsoft Graph](/graph/overview)の概念とプラクティスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="bfa8b-181">Explore [Microsoft Graph](/graph/overview) concepts and practices.</span></span>
- <span data-ttu-id="bfa8b-182">[Graph エクスプローラー](https://aka.ms/ge)を使用して、Microsoft graph を試してみてください。</span><span class="sxs-lookup"><span data-stu-id="bfa8b-182">Use [Graph Explorer](https://aka.ms/ge) to experiment with Microsoft Graph.</span></span>
