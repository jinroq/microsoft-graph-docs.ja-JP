---
title: oAuth2Permission リソースの種類
description: OAuth 2.0 を表しますは、アクセス許可のスコープを委任します。 (Application オブジェクトの**requiredResourceAccess**コレクション) をクライアント アプリケーションで、委任されたアクセス許可のスコープを要求することが指定された OAuth 2.0 リソース アプリケーションを呼び出すときにします。 ServicePrincipal エンティティおよびアプリケーション エンティティの**appRoles**プロパティは、 **oAuth2Permission**のコレクションです。
ms.openlocfilehash: 4a790c935dd84fb7bd4e1422ca59914d9a319ae9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071967"
---
# <a name="oauth2permission-resource-type"></a><span data-ttu-id="4845a-105">oAuth2Permission リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4845a-105">oAuth2Permission resource type</span></span>

> <span data-ttu-id="4845a-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4845a-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4845a-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4845a-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4845a-108">OAuth 2.0 を表しますは、アクセス許可のスコープを委任します。</span><span class="sxs-lookup"><span data-stu-id="4845a-108">Represents an OAuth 2.0 delegated permission scope.</span></span> <span data-ttu-id="4845a-109">( [Application](application.md)オブジェクトの**requiredResourceAccess**コレクション) をクライアント アプリケーションで、委任されたアクセス許可のスコープを要求することが指定された OAuth 2.0 リソース アプリケーションを呼び出すときにします。</span><span class="sxs-lookup"><span data-stu-id="4845a-109">The specified OAuth 2.0 delegated permission scopes may be requested by client applications (through the **requiredResourceAccess** collection on the [application](application.md) object) when calling a resource application.</span></span> <span data-ttu-id="4845a-110">[ServicePrincipal](serviceprincipal.md)エンティティおよび[アプリケーション](application.md)エンティティの**appRoles**プロパティは、 **oAuth2Permission**のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="4845a-110">The **appRoles** property of the [servicePrincipal](serviceprincipal.md) entity and of the [application](application.md) entity is a collection of **oAuth2Permission**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="4845a-111">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4845a-111">JSON representation</span></span>

<span data-ttu-id="4845a-112">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="4845a-112">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.oAuth2Permission"
}-->

```json
{
  "adminConsentDescription": "string",
  "adminConsentDisplayName": "string",
  "id": "guid",
  "isEnabled": true,
  "origin": "string",
  "type": "string",
  "userConsentDescription": "string",
  "userConsentDisplayName": "string",
  "value": "string"
}

```
## <a name="properties"></a><span data-ttu-id="4845a-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4845a-113">Properties</span></span>
| <span data-ttu-id="4845a-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4845a-114">Property</span></span>     | <span data-ttu-id="4845a-115">型</span><span class="sxs-lookup"><span data-stu-id="4845a-115">Type</span></span>   |<span data-ttu-id="4845a-116">説明</span><span class="sxs-lookup"><span data-stu-id="4845a-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4845a-117">adminConsentDescription</span><span class="sxs-lookup"><span data-stu-id="4845a-117">adminConsentDescription</span></span>|<span data-ttu-id="4845a-118">String</span><span class="sxs-lookup"><span data-stu-id="4845a-118">String</span></span>|<span data-ttu-id="4845a-119">管理者同意し、アプリケーションの割り当てのエクスペリエンスに表示されるアクセス許可のヘルプ テキストです。</span><span class="sxs-lookup"><span data-stu-id="4845a-119">Permission help text that appears in the admin consent and app assignment experiences.</span></span>|
|<span data-ttu-id="4845a-120">adminConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="4845a-120">adminConsentDisplayName</span></span>|<span data-ttu-id="4845a-121">String</span><span class="sxs-lookup"><span data-stu-id="4845a-121">String</span></span>|<span data-ttu-id="4845a-122">管理者同意し、アプリケーションの割り当ての経験で表示されるアクセス許可の名前を表示します。</span><span class="sxs-lookup"><span data-stu-id="4845a-122">Display name for the permission that appears in the admin consent and app assignment experiences.</span></span>|
|<span data-ttu-id="4845a-123">ID</span><span class="sxs-lookup"><span data-stu-id="4845a-123">id</span></span>|<span data-ttu-id="4845a-124">Guid</span><span class="sxs-lookup"><span data-stu-id="4845a-124">Guid</span></span>|<span data-ttu-id="4845a-125">Oauth2Permissions コレクション内の一意のスコープ権限識別子です。</span><span class="sxs-lookup"><span data-stu-id="4845a-125">Unique scope permission identifier inside the oauth2Permissions collection.</span></span>|
|<span data-ttu-id="4845a-126">isEnabled</span><span class="sxs-lookup"><span data-stu-id="4845a-126">isEnabled</span></span>|<span data-ttu-id="4845a-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="4845a-127">Boolean</span></span>|<span data-ttu-id="4845a-128">を作成またはアクセス許可を更新するとき、このプロパティは**true** (既定値) に設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="4845a-128">When creating or updating a permission, this property must be set to **true** (which is the default).</span></span> <span data-ttu-id="4845a-129">アクセス許可を削除するには、このプロパティを**false**に設定最初する必要があります。</span><span class="sxs-lookup"><span data-stu-id="4845a-129">To delete a permission, this property must first be set to **false**.</span></span>  <span data-ttu-id="4845a-130">その時点で、後続の呼び出しでアクセス許可が削除されます。</span><span class="sxs-lookup"><span data-stu-id="4845a-130">At that point, in a subsequent call, the permission may be removed.</span></span>|
|<span data-ttu-id="4845a-131">type</span><span class="sxs-lookup"><span data-stu-id="4845a-131">type</span></span>|<span data-ttu-id="4845a-132">String</span><span class="sxs-lookup"><span data-stu-id="4845a-132">String</span></span>|<span data-ttu-id="4845a-133">、エンドユーザーがこのスコープの権限に同意するかどうか、または必要があることに同意した企業の管理者によって、テナント全体のアクセス許可があるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="4845a-133">Specifies whether this scope permission can be consented to by an end user, or whether it is a tenant-wide permission that must be consented to by a Company Administrator.</span></span>  <span data-ttu-id="4845a-134">使用可能な値は、「ユーザー」または"Admin"です。</span><span class="sxs-lookup"><span data-stu-id="4845a-134">Possible values are "User" or "Admin".</span></span>|
|<span data-ttu-id="4845a-135">userConsentDescription</span><span class="sxs-lookup"><span data-stu-id="4845a-135">userConsentDescription</span></span>|<span data-ttu-id="4845a-136">String</span><span class="sxs-lookup"><span data-stu-id="4845a-136">String</span></span>|<span data-ttu-id="4845a-137">エンド ・ ユーザーの同意の経験では表示されているアクセス許可のヘルプ テキストです。</span><span class="sxs-lookup"><span data-stu-id="4845a-137">Permission help text that appears in the end user consent experience.</span></span>|
|<span data-ttu-id="4845a-138">userConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="4845a-138">userConsentDisplayName</span></span>|<span data-ttu-id="4845a-139">String</span><span class="sxs-lookup"><span data-stu-id="4845a-139">String</span></span>|<span data-ttu-id="4845a-140">エンド ・ ユーザーの同意の経験では、アクセス許可が表示されるの名前を表示します。</span><span class="sxs-lookup"><span data-stu-id="4845a-140">Display name for the permission that appears in the end user consent experience.</span></span>|
|<span data-ttu-id="4845a-141">value</span><span class="sxs-lookup"><span data-stu-id="4845a-141">value</span></span>|<span data-ttu-id="4845a-142">文字列</span><span class="sxs-lookup"><span data-stu-id="4845a-142">String</span></span>|<span data-ttu-id="4845a-143">スコープの値は、OAuth 2.0 のアクセス トークンにリソース アプリケーションが予想されることを要求します。</span><span class="sxs-lookup"><span data-stu-id="4845a-143">The value of the scope claim that the resource application should expect in the OAuth 2.0 access token.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "oAuth2Permission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
