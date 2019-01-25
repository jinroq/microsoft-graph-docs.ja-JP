---
title: permissionScope リソースの種類
description: OAuth 2.0 を表しますは、アクセス許可のスコープを委任します。 (Application オブジェクトの**requiredResourceAccess**コレクション) をクライアント アプリケーションで、委任されたアクセス許可のスコープを要求することが指定された OAuth 2.0 リソース アプリケーションを呼び出すときにします。 ServicePrincipal エンティティおよびアプリケーション エンティティの**oauth2Permissions**プロパティは、 **OAuth2Permission**のコレクションです。
localization_priority: Normal
ms.openlocfilehash: 00629a6e123ef19290d3c1bd4797e4bab3ce95c0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517079"
---
# <a name="permissionscope-resource-type"></a><span data-ttu-id="bdbd6-105">permissionScope リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bdbd6-105">permissionScope resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bdbd6-106">OAuth 2.0 を表しますは、アクセス許可のスコープを委任します。</span><span class="sxs-lookup"><span data-stu-id="bdbd6-106">Represents an OAuth 2.0 delegated permission scope.</span></span> <span data-ttu-id="bdbd6-107">( [Application](application.md)オブジェクトの**requiredResourceAccess**コレクション) をクライアント アプリケーションで、委任されたアクセス許可のスコープを要求することが指定された OAuth 2.0 リソース アプリケーションを呼び出すときにします。</span><span class="sxs-lookup"><span data-stu-id="bdbd6-107">The specified OAuth 2.0 delegated permission scopes may be requested by client applications (through the **requiredResourceAccess** collection on the [Application](application.md) object) when calling a resource application.</span></span> <span data-ttu-id="bdbd6-108">[ServicePrincipal](serviceprincipal.md)エンティティおよび[アプリケーション](application.md)エンティティの**oauth2Permissions**プロパティは、 **OAuth2Permission**のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="bdbd6-108">The **oauth2Permissions** property of the [ServicePrincipal](serviceprincipal.md) entity and of the [Application](application.md) entity is a collection of **OAuth2Permission**.</span></span>

## <a name="properties"></a><span data-ttu-id="bdbd6-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bdbd6-109">Properties</span></span>

| <span data-ttu-id="bdbd6-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bdbd6-110">Property</span></span> | <span data-ttu-id="bdbd6-111">型</span><span class="sxs-lookup"><span data-stu-id="bdbd6-111">Type</span></span> | <span data-ttu-id="bdbd6-112">説明</span><span class="sxs-lookup"><span data-stu-id="bdbd6-112">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="bdbd6-113">adminConsentDescription</span><span class="sxs-lookup"><span data-stu-id="bdbd6-113">adminConsentDescription</span></span>|<span data-ttu-id="bdbd6-114">String</span><span class="sxs-lookup"><span data-stu-id="bdbd6-114">String</span></span>| <span data-ttu-id="bdbd6-115">管理者同意し、アプリケーションの割り当てのエクスペリエンスに表示されるアクセス許可のヘルプ テキストです。</span><span class="sxs-lookup"><span data-stu-id="bdbd6-115">Permission help text that appears in the admin consent and app assignment experiences.</span></span> |
|<span data-ttu-id="bdbd6-116">adminConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="bdbd6-116">adminConsentDisplayName</span></span>|<span data-ttu-id="bdbd6-117">String</span><span class="sxs-lookup"><span data-stu-id="bdbd6-117">String</span></span>| <span data-ttu-id="bdbd6-118">管理者同意し、アプリケーションの割り当ての経験で表示されるアクセス許可の名前を表示します。</span><span class="sxs-lookup"><span data-stu-id="bdbd6-118">Display name for the permission that appears in the admin consent and app assignment experiences.</span></span> |
|<span data-ttu-id="bdbd6-119">ID</span><span class="sxs-lookup"><span data-stu-id="bdbd6-119">id</span></span>|<span data-ttu-id="bdbd6-120">Guid</span><span class="sxs-lookup"><span data-stu-id="bdbd6-120">Guid</span></span>| <span data-ttu-id="bdbd6-121">Oauth2Permissions コレクション内の一意のスコープ権限識別子です。</span><span class="sxs-lookup"><span data-stu-id="bdbd6-121">Unique scope permission identifier inside the oauth2Permissions collection.</span></span> |
|<span data-ttu-id="bdbd6-122">isEnabled</span><span class="sxs-lookup"><span data-stu-id="bdbd6-122">isEnabled</span></span>|<span data-ttu-id="bdbd6-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="bdbd6-123">Boolean</span></span>| <span data-ttu-id="bdbd6-124">を作成またはアクセス許可を更新するとき、このプロパティは**true** (既定値) に設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="bdbd6-124">When creating or updating a permission, this property must be set to **true** (which is the default).</span></span> <span data-ttu-id="bdbd6-125">アクセス許可を削除するには、このプロパティを**false**に設定最初する必要があります。</span><span class="sxs-lookup"><span data-stu-id="bdbd6-125">To delete a permission, this property must first be set to **false**.</span></span> <span data-ttu-id="bdbd6-126">その時点で、後続の呼び出しでアクセス許可が削除されます。</span><span class="sxs-lookup"><span data-stu-id="bdbd6-126">At that point, in a subsequent call, the permission may be removed.</span></span> |
|<span data-ttu-id="bdbd6-127">始点</span><span class="sxs-lookup"><span data-stu-id="bdbd6-127">origin</span></span>|<span data-ttu-id="bdbd6-128">String</span><span class="sxs-lookup"><span data-stu-id="bdbd6-128">String</span></span>| <span data-ttu-id="bdbd6-129">内部で使用します。</span><span class="sxs-lookup"><span data-stu-id="bdbd6-129">For internal use.</span></span> |
|<span data-ttu-id="bdbd6-130">type</span><span class="sxs-lookup"><span data-stu-id="bdbd6-130">type</span></span>|<span data-ttu-id="bdbd6-131">String</span><span class="sxs-lookup"><span data-stu-id="bdbd6-131">String</span></span>| <span data-ttu-id="bdbd6-132">、エンドユーザーがこのスコープの権限に同意するかどうか、または企業の管理者によって、に同意する必要があります、テナント全体のアクセス許可があるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="bdbd6-132">Specifies whether this scope permission can be consented to by an end user, or whether it is a tenant-wide permission that must be consented to by a company administrator.</span></span> <span data-ttu-id="bdbd6-133">使用可能な値は、*ユーザー*または*管理者*です。</span><span class="sxs-lookup"><span data-stu-id="bdbd6-133">Possible values are *User* or *Admin*.</span></span> |
|<span data-ttu-id="bdbd6-134">userConsentDescription</span><span class="sxs-lookup"><span data-stu-id="bdbd6-134">userConsentDescription</span></span>|<span data-ttu-id="bdbd6-135">String</span><span class="sxs-lookup"><span data-stu-id="bdbd6-135">String</span></span>| <span data-ttu-id="bdbd6-136">エンドユーザーの同意に表示されるアクセス許可のヘルプ テキストです。</span><span class="sxs-lookup"><span data-stu-id="bdbd6-136">Permission help text that appears in the end-user consent experience.</span></span> |
|<span data-ttu-id="bdbd6-137">userConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="bdbd6-137">userConsentDisplayName</span></span>|<span data-ttu-id="bdbd6-138">String</span><span class="sxs-lookup"><span data-stu-id="bdbd6-138">String</span></span>| <span data-ttu-id="bdbd6-139">エンドユーザーの同意で表示されるアクセス許可の名前を表示します。</span><span class="sxs-lookup"><span data-stu-id="bdbd6-139">Display name for the permission that appears in the end-user consent experience.</span></span> |
|<span data-ttu-id="bdbd6-140">value</span><span class="sxs-lookup"><span data-stu-id="bdbd6-140">value</span></span>|<span data-ttu-id="bdbd6-141">文字列</span><span class="sxs-lookup"><span data-stu-id="bdbd6-141">String</span></span>| <span data-ttu-id="bdbd6-142">スコープの値は、OAuth 2.0 のアクセス トークンにリソース アプリケーションが予想されることを要求します。</span><span class="sxs-lookup"><span data-stu-id="bdbd6-142">The value of the scope claim that the resource application should expect in the OAuth 2.0 access token.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="bdbd6-143">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bdbd6-143">JSON representation</span></span>
<span data-ttu-id="bdbd6-144">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bdbd6-144">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "permissionScope resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/permissionscope.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
