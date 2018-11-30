---
title: permissionScope リソースの種類
description: OAuth 2.0 を表しますは、アクセス許可のスコープを委任します。 (Application オブジェクトの**requiredResourceAccess**コレクション) をクライアント アプリケーションで、委任されたアクセス許可のスコープを要求することが指定された OAuth 2.0 リソース アプリケーションを呼び出すときにします。 ServicePrincipal エンティティおよびアプリケーション エンティティの**oauth2Permissions**プロパティは、 **OAuth2Permission**のコレクションです。
ms.openlocfilehash: b15ee9901632fca113d944000847c953e85be58c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071975"
---
# <a name="permissionscope-resource-type"></a><span data-ttu-id="bd14c-105">permissionScope リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bd14c-105">permissionScope resource type</span></span>

> <span data-ttu-id="bd14c-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="bd14c-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bd14c-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bd14c-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bd14c-108">OAuth 2.0 を表しますは、アクセス許可のスコープを委任します。</span><span class="sxs-lookup"><span data-stu-id="bd14c-108">Represents an OAuth 2.0 delegated permission scope.</span></span> <span data-ttu-id="bd14c-109">( [Application](application.md)オブジェクトの**requiredResourceAccess**コレクション) をクライアント アプリケーションで、委任されたアクセス許可のスコープを要求することが指定された OAuth 2.0 リソース アプリケーションを呼び出すときにします。</span><span class="sxs-lookup"><span data-stu-id="bd14c-109">The specified OAuth 2.0 delegated permission scopes may be requested by client applications (through the **requiredResourceAccess** collection on the [Application](application.md) object) when calling a resource application.</span></span> <span data-ttu-id="bd14c-110">[ServicePrincipal](serviceprincipal.md)エンティティおよび[アプリケーション](application.md)エンティティの**oauth2Permissions**プロパティは、 **OAuth2Permission**のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="bd14c-110">The **oauth2Permissions** property of the [ServicePrincipal](serviceprincipal.md) entity and of the [Application](application.md) entity is a collection of **OAuth2Permission**.</span></span>

## <a name="properties"></a><span data-ttu-id="bd14c-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bd14c-111">Properties</span></span>

| <span data-ttu-id="bd14c-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bd14c-112">Property</span></span> | <span data-ttu-id="bd14c-113">型</span><span class="sxs-lookup"><span data-stu-id="bd14c-113">Type</span></span> | <span data-ttu-id="bd14c-114">説明</span><span class="sxs-lookup"><span data-stu-id="bd14c-114">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="bd14c-115">adminConsentDescription</span><span class="sxs-lookup"><span data-stu-id="bd14c-115">adminConsentDescription</span></span>|<span data-ttu-id="bd14c-116">String</span><span class="sxs-lookup"><span data-stu-id="bd14c-116">String</span></span>| <span data-ttu-id="bd14c-117">管理者同意し、アプリケーションの割り当てのエクスペリエンスに表示されるアクセス許可のヘルプ テキストです。</span><span class="sxs-lookup"><span data-stu-id="bd14c-117">Permission help text that appears in the admin consent and app assignment experiences.</span></span> |
|<span data-ttu-id="bd14c-118">adminConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="bd14c-118">adminConsentDisplayName</span></span>|<span data-ttu-id="bd14c-119">String</span><span class="sxs-lookup"><span data-stu-id="bd14c-119">String</span></span>| <span data-ttu-id="bd14c-120">管理者同意し、アプリケーションの割り当ての経験で表示されるアクセス許可の名前を表示します。</span><span class="sxs-lookup"><span data-stu-id="bd14c-120">Display name for the permission that appears in the admin consent and app assignment experiences.</span></span> |
|<span data-ttu-id="bd14c-121">ID</span><span class="sxs-lookup"><span data-stu-id="bd14c-121">id</span></span>|<span data-ttu-id="bd14c-122">Guid</span><span class="sxs-lookup"><span data-stu-id="bd14c-122">Guid</span></span>| <span data-ttu-id="bd14c-123">Oauth2Permissions コレクション内の一意のスコープ権限識別子です。</span><span class="sxs-lookup"><span data-stu-id="bd14c-123">Unique scope permission identifier inside the oauth2Permissions collection.</span></span> |
|<span data-ttu-id="bd14c-124">isEnabled</span><span class="sxs-lookup"><span data-stu-id="bd14c-124">isEnabled</span></span>|<span data-ttu-id="bd14c-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd14c-125">Boolean</span></span>| <span data-ttu-id="bd14c-126">を作成またはアクセス許可を更新するとき、このプロパティは**true** (既定値) に設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="bd14c-126">When creating or updating a permission, this property must be set to **true** (which is the default).</span></span> <span data-ttu-id="bd14c-127">アクセス許可を削除するには、このプロパティを**false**に設定最初する必要があります。</span><span class="sxs-lookup"><span data-stu-id="bd14c-127">To delete a permission, this property must first be set to **false**.</span></span> <span data-ttu-id="bd14c-128">その時点で、後続の呼び出しでアクセス許可が削除されます。</span><span class="sxs-lookup"><span data-stu-id="bd14c-128">At that point, in a subsequent call, the permission may be removed.</span></span> |
|<span data-ttu-id="bd14c-129">原点</span><span class="sxs-lookup"><span data-stu-id="bd14c-129">origin</span></span>|<span data-ttu-id="bd14c-130">String</span><span class="sxs-lookup"><span data-stu-id="bd14c-130">String</span></span>| <span data-ttu-id="bd14c-131">内部で使用します。</span><span class="sxs-lookup"><span data-stu-id="bd14c-131">For internal use.</span></span> |
|<span data-ttu-id="bd14c-132">type</span><span class="sxs-lookup"><span data-stu-id="bd14c-132">type</span></span>|<span data-ttu-id="bd14c-133">String</span><span class="sxs-lookup"><span data-stu-id="bd14c-133">String</span></span>| <span data-ttu-id="bd14c-134">、エンドユーザーがこのスコープの権限に同意するかどうか、または企業の管理者によって、に同意する必要があります、テナント全体のアクセス許可があるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="bd14c-134">Specifies whether this scope permission can be consented to by an end user, or whether it is a tenant-wide permission that must be consented to by a company administrator.</span></span> <span data-ttu-id="bd14c-135">使用可能な値は、*ユーザー*または*管理者*です。</span><span class="sxs-lookup"><span data-stu-id="bd14c-135">Possible values are *User* or *Admin*.</span></span> |
|<span data-ttu-id="bd14c-136">userConsentDescription</span><span class="sxs-lookup"><span data-stu-id="bd14c-136">userConsentDescription</span></span>|<span data-ttu-id="bd14c-137">String</span><span class="sxs-lookup"><span data-stu-id="bd14c-137">String</span></span>| <span data-ttu-id="bd14c-138">エンドユーザーの同意に表示されるアクセス許可のヘルプ テキストです。</span><span class="sxs-lookup"><span data-stu-id="bd14c-138">Permission help text that appears in the end-user consent experience.</span></span> |
|<span data-ttu-id="bd14c-139">userConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="bd14c-139">userConsentDisplayName</span></span>|<span data-ttu-id="bd14c-140">String</span><span class="sxs-lookup"><span data-stu-id="bd14c-140">String</span></span>| <span data-ttu-id="bd14c-141">エンドユーザーの同意で表示されるアクセス許可の名前を表示します。</span><span class="sxs-lookup"><span data-stu-id="bd14c-141">Display name for the permission that appears in the end-user consent experience.</span></span> |
|<span data-ttu-id="bd14c-142">value</span><span class="sxs-lookup"><span data-stu-id="bd14c-142">value</span></span>|<span data-ttu-id="bd14c-143">文字列</span><span class="sxs-lookup"><span data-stu-id="bd14c-143">String</span></span>| <span data-ttu-id="bd14c-144">スコープの値は、OAuth 2.0 のアクセス トークンにリソース アプリケーションが予想されることを要求します。</span><span class="sxs-lookup"><span data-stu-id="bd14c-144">The value of the scope claim that the resource application should expect in the OAuth 2.0 access token.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="bd14c-145">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bd14c-145">JSON representation</span></span>
<span data-ttu-id="bd14c-146">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bd14c-146">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.permissionScope"
}-->

```json
{
  "adminConsentDescription": "String",
  "adminConsentDisplayName": "String",
  "id": "Guid",
  "isEnabled": true,
  "origin": "String",
  "type": "String",
  "userConsentDescription": "String",
  "userConsentDisplayName": "String",
  "value": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "permissionScope resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->