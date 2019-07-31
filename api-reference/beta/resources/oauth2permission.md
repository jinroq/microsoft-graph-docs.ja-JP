---
title: oAuth2Permission リソースの種類
description: OAuth 2.0 委任されたアクセス許可スコープを表します。 指定した OAuth 2.0 委任されたアクセス許可スコープは、リソースアプリケーションを呼び出すときに (application オブジェクトの**Requiredresourceaccess**コレクションを通じて) クライアントアプリケーションによって要求されることがあります。 ServicePrincipal エンティティおよび application エンティティの**approles**プロパティは、 **oAuth2Permission**のコレクションです。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 16dfa93d13127d585cd5b56a56987bb22ab39d8f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009574"
---
# <a name="oauth2permission-resource-type"></a><span data-ttu-id="b1246-105">oAuth2Permission リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b1246-105">oAuth2Permission resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1246-106">OAuth 2.0 委任されたアクセス許可スコープを表します。</span><span class="sxs-lookup"><span data-stu-id="b1246-106">Represents an OAuth 2.0 delegated permission scope.</span></span> <span data-ttu-id="b1246-107">指定した OAuth 2.0 委任されたアクセス許可スコープは、リソースアプリケーションを呼び出すときに ( [application](application.md)オブジェクトの**requiredresourceaccess**コレクションを通じて) クライアントアプリケーションによって要求されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b1246-107">The specified OAuth 2.0 delegated permission scopes may be requested by client applications (through the **requiredResourceAccess** collection on the [application](application.md) object) when calling a resource application.</span></span> <span data-ttu-id="b1246-108">[Serviceprincipal](serviceprincipal.md)エンティティおよび[Application](application.md)エンティティの**Approles**プロパティは、 **oAuth2Permission**のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="b1246-108">The **appRoles** property of the [servicePrincipal](serviceprincipal.md) entity and of the [application](application.md) entity is a collection of **oAuth2Permission**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="b1246-109">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b1246-109">JSON representation</span></span>

<span data-ttu-id="b1246-110">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="b1246-110">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="b1246-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b1246-111">Properties</span></span>
| <span data-ttu-id="b1246-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b1246-112">Property</span></span>     | <span data-ttu-id="b1246-113">型</span><span class="sxs-lookup"><span data-stu-id="b1246-113">Type</span></span>   |<span data-ttu-id="b1246-114">説明</span><span class="sxs-lookup"><span data-stu-id="b1246-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b1246-115">Admincon/説明</span><span class="sxs-lookup"><span data-stu-id="b1246-115">adminConsentDescription</span></span>|<span data-ttu-id="b1246-116">String</span><span class="sxs-lookup"><span data-stu-id="b1246-116">String</span></span>|<span data-ttu-id="b1246-117">管理者の同意とアプリの割り当てエクスペリエンスに表示されるアクセス許可ヘルプテキスト。</span><span class="sxs-lookup"><span data-stu-id="b1246-117">Permission help text that appears in the admin consent and app assignment experiences.</span></span>|
|<span data-ttu-id="b1246-118">Admincon/表示 Displayname</span><span class="sxs-lookup"><span data-stu-id="b1246-118">adminConsentDisplayName</span></span>|<span data-ttu-id="b1246-119">String</span><span class="sxs-lookup"><span data-stu-id="b1246-119">String</span></span>|<span data-ttu-id="b1246-120">管理者の同意とアプリの割り当てエクスペリエンスに表示されるアクセス許可の表示名。</span><span class="sxs-lookup"><span data-stu-id="b1246-120">Display name for the permission that appears in the admin consent and app assignment experiences.</span></span>|
|<span data-ttu-id="b1246-121">id</span><span class="sxs-lookup"><span data-stu-id="b1246-121">id</span></span>|<span data-ttu-id="b1246-122">Guid</span><span class="sxs-lookup"><span data-stu-id="b1246-122">Guid</span></span>|<span data-ttu-id="b1246-123">Oauth2Permissions コレクション内の一意のスコープアクセス許可識別子。</span><span class="sxs-lookup"><span data-stu-id="b1246-123">Unique scope permission identifier inside the oauth2Permissions collection.</span></span>|
|<span data-ttu-id="b1246-124">isEnabled</span><span class="sxs-lookup"><span data-stu-id="b1246-124">isEnabled</span></span>|<span data-ttu-id="b1246-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1246-125">Boolean</span></span>|<span data-ttu-id="b1246-126">アクセス許可を作成または更新する場合は、このプロパティを**true**に設定する必要があります (これは既定値です)。</span><span class="sxs-lookup"><span data-stu-id="b1246-126">When creating or updating a permission, this property must be set to **true** (which is the default).</span></span> <span data-ttu-id="b1246-127">権限を削除するには、最初にこのプロパティを**false**に設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b1246-127">To delete a permission, this property must first be set to **false**.</span></span>  <span data-ttu-id="b1246-128">その時点で、以降の呼び出しでは、アクセス許可が削除されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b1246-128">At that point, in a subsequent call, the permission may be removed.</span></span>|
|<span data-ttu-id="b1246-129">type</span><span class="sxs-lookup"><span data-stu-id="b1246-129">type</span></span>|<span data-ttu-id="b1246-130">String</span><span class="sxs-lookup"><span data-stu-id="b1246-130">String</span></span>|<span data-ttu-id="b1246-131">この範囲のアクセス許可をエンドユーザーが同意することができるかどうか、または会社の管理者が同意する必要があるテナント全体のアクセス許可であるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="b1246-131">Specifies whether this scope permission can be consented to by an end user, or whether it is a tenant-wide permission that must be consented to by a Company Administrator.</span></span>  <span data-ttu-id="b1246-132">可能な値は、"User" または "Admin" です。</span><span class="sxs-lookup"><span data-stu-id="b1246-132">Possible values are "User" or "Admin".</span></span>|
|<span data-ttu-id="b1246-133">Usercondescription の説明</span><span class="sxs-lookup"><span data-stu-id="b1246-133">userConsentDescription</span></span>|<span data-ttu-id="b1246-134">String</span><span class="sxs-lookup"><span data-stu-id="b1246-134">String</span></span>|<span data-ttu-id="b1246-135">エンドユーザーの同意画面に表示されるアクセス許可ヘルプテキスト。</span><span class="sxs-lookup"><span data-stu-id="b1246-135">Permission help text that appears in the end user consent experience.</span></span>|
|<span data-ttu-id="b1246-136">Usercon使い方 Displayname</span><span class="sxs-lookup"><span data-stu-id="b1246-136">userConsentDisplayName</span></span>|<span data-ttu-id="b1246-137">String</span><span class="sxs-lookup"><span data-stu-id="b1246-137">String</span></span>|<span data-ttu-id="b1246-138">エンドユーザーの同意画面に表示されるアクセス許可の表示名。</span><span class="sxs-lookup"><span data-stu-id="b1246-138">Display name for the permission that appears in the end user consent experience.</span></span>|
|<span data-ttu-id="b1246-139">value</span><span class="sxs-lookup"><span data-stu-id="b1246-139">value</span></span>|<span data-ttu-id="b1246-140">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="b1246-140">String</span></span>|<span data-ttu-id="b1246-141">OAuth 2.0 アクセストークンで想定されるリソースアプリケーションのスコープ要求の値。</span><span class="sxs-lookup"><span data-stu-id="b1246-141">The value of the scope claim that the resource application should expect in the OAuth 2.0 access token.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oAuth2Permission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
