---
title: oAuth2Permission リソースの種類
description: OAuth 2.0 を表しますは、アクセス許可のスコープを委任します。 (Application オブジェクトの**requiredResourceAccess**コレクション) をクライアント アプリケーションで、委任されたアクセス許可のスコープを要求することが指定された OAuth 2.0 リソース アプリケーションを呼び出すときにします。 ServicePrincipal エンティティおよびアプリケーション エンティティの**appRoles**プロパティは、 **oAuth2Permission**のコレクションです。
localization_priority: Normal
ms.openlocfilehash: 8d8bb0bb5af17b7322bd6be37ac48ae9edbeba42
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510814"
---
# <a name="oauth2permission-resource-type"></a><span data-ttu-id="24541-105">oAuth2Permission リソースの種類</span><span class="sxs-lookup"><span data-stu-id="24541-105">oAuth2Permission resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24541-106">OAuth 2.0 を表しますは、アクセス許可のスコープを委任します。</span><span class="sxs-lookup"><span data-stu-id="24541-106">Represents an OAuth 2.0 delegated permission scope.</span></span> <span data-ttu-id="24541-107">( [Application](application.md)オブジェクトの**requiredResourceAccess**コレクション) をクライアント アプリケーションで、委任されたアクセス許可のスコープを要求することが指定された OAuth 2.0 リソース アプリケーションを呼び出すときにします。</span><span class="sxs-lookup"><span data-stu-id="24541-107">The specified OAuth 2.0 delegated permission scopes may be requested by client applications (through the **requiredResourceAccess** collection on the [application](application.md) object) when calling a resource application.</span></span> <span data-ttu-id="24541-108">[ServicePrincipal](serviceprincipal.md)エンティティおよび[アプリケーション](application.md)エンティティの**appRoles**プロパティは、 **oAuth2Permission**のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="24541-108">The **appRoles** property of the [servicePrincipal](serviceprincipal.md) entity and of the [application](application.md) entity is a collection of **oAuth2Permission**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="24541-109">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="24541-109">JSON representation</span></span>

<span data-ttu-id="24541-110">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="24541-110">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="24541-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="24541-111">Properties</span></span>
| <span data-ttu-id="24541-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="24541-112">Property</span></span>     | <span data-ttu-id="24541-113">型</span><span class="sxs-lookup"><span data-stu-id="24541-113">Type</span></span>   |<span data-ttu-id="24541-114">説明</span><span class="sxs-lookup"><span data-stu-id="24541-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="24541-115">adminConsentDescription</span><span class="sxs-lookup"><span data-stu-id="24541-115">adminConsentDescription</span></span>|<span data-ttu-id="24541-116">String</span><span class="sxs-lookup"><span data-stu-id="24541-116">String</span></span>|<span data-ttu-id="24541-117">管理者同意し、アプリケーションの割り当てのエクスペリエンスに表示されるアクセス許可のヘルプ テキストです。</span><span class="sxs-lookup"><span data-stu-id="24541-117">Permission help text that appears in the admin consent and app assignment experiences.</span></span>|
|<span data-ttu-id="24541-118">adminConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="24541-118">adminConsentDisplayName</span></span>|<span data-ttu-id="24541-119">String</span><span class="sxs-lookup"><span data-stu-id="24541-119">String</span></span>|<span data-ttu-id="24541-120">管理者同意し、アプリケーションの割り当ての経験で表示されるアクセス許可の名前を表示します。</span><span class="sxs-lookup"><span data-stu-id="24541-120">Display name for the permission that appears in the admin consent and app assignment experiences.</span></span>|
|<span data-ttu-id="24541-121">ID</span><span class="sxs-lookup"><span data-stu-id="24541-121">id</span></span>|<span data-ttu-id="24541-122">Guid</span><span class="sxs-lookup"><span data-stu-id="24541-122">Guid</span></span>|<span data-ttu-id="24541-123">Oauth2Permissions コレクション内の一意のスコープ権限識別子です。</span><span class="sxs-lookup"><span data-stu-id="24541-123">Unique scope permission identifier inside the oauth2Permissions collection.</span></span>|
|<span data-ttu-id="24541-124">isEnabled</span><span class="sxs-lookup"><span data-stu-id="24541-124">isEnabled</span></span>|<span data-ttu-id="24541-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="24541-125">Boolean</span></span>|<span data-ttu-id="24541-126">を作成またはアクセス許可を更新するとき、このプロパティは**true** (既定値) に設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="24541-126">When creating or updating a permission, this property must be set to **true** (which is the default).</span></span> <span data-ttu-id="24541-127">アクセス許可を削除するには、このプロパティを**false**に設定最初する必要があります。</span><span class="sxs-lookup"><span data-stu-id="24541-127">To delete a permission, this property must first be set to **false**.</span></span>  <span data-ttu-id="24541-128">その時点で、後続の呼び出しでアクセス許可が削除されます。</span><span class="sxs-lookup"><span data-stu-id="24541-128">At that point, in a subsequent call, the permission may be removed.</span></span>|
|<span data-ttu-id="24541-129">type</span><span class="sxs-lookup"><span data-stu-id="24541-129">type</span></span>|<span data-ttu-id="24541-130">String</span><span class="sxs-lookup"><span data-stu-id="24541-130">String</span></span>|<span data-ttu-id="24541-131">、エンドユーザーがこのスコープの権限に同意するかどうか、または必要があることに同意した企業の管理者によって、テナント全体のアクセス許可があるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="24541-131">Specifies whether this scope permission can be consented to by an end user, or whether it is a tenant-wide permission that must be consented to by a Company Administrator.</span></span>  <span data-ttu-id="24541-132">使用可能な値は、「ユーザー」または"Admin"です。</span><span class="sxs-lookup"><span data-stu-id="24541-132">Possible values are "User" or "Admin".</span></span>|
|<span data-ttu-id="24541-133">userConsentDescription</span><span class="sxs-lookup"><span data-stu-id="24541-133">userConsentDescription</span></span>|<span data-ttu-id="24541-134">String</span><span class="sxs-lookup"><span data-stu-id="24541-134">String</span></span>|<span data-ttu-id="24541-135">エンド ・ ユーザーの同意の経験では表示されているアクセス許可のヘルプ テキストです。</span><span class="sxs-lookup"><span data-stu-id="24541-135">Permission help text that appears in the end user consent experience.</span></span>|
|<span data-ttu-id="24541-136">userConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="24541-136">userConsentDisplayName</span></span>|<span data-ttu-id="24541-137">String</span><span class="sxs-lookup"><span data-stu-id="24541-137">String</span></span>|<span data-ttu-id="24541-138">エンド ・ ユーザーの同意の経験では、アクセス許可が表示されるの名前を表示します。</span><span class="sxs-lookup"><span data-stu-id="24541-138">Display name for the permission that appears in the end user consent experience.</span></span>|
|<span data-ttu-id="24541-139">value</span><span class="sxs-lookup"><span data-stu-id="24541-139">value</span></span>|<span data-ttu-id="24541-140">文字列</span><span class="sxs-lookup"><span data-stu-id="24541-140">String</span></span>|<span data-ttu-id="24541-141">スコープの値は、OAuth 2.0 のアクセス トークンにリソース アプリケーションが予想されることを要求します。</span><span class="sxs-lookup"><span data-stu-id="24541-141">The value of the scope claim that the resource application should expect in the OAuth 2.0 access token.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oAuth2Permission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/oauth2permission.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
