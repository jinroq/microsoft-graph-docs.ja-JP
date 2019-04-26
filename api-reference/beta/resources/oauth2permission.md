---
title: oAuth2Permission リソースの種類
description: OAuth 2.0 委任されたアクセス許可スコープを表します。 指定した OAuth 2.0 委任されたアクセス許可スコープは、リソースアプリケーションを呼び出すときに (application オブジェクトの**requiredresourceaccess**コレクションを通じて) クライアントアプリケーションによって要求されることがあります。 serviceprincipal エンティティおよび application エンティティの**approles**プロパティは、 **oAuth2Permission**のコレクションです。
localization_priority: Normal
ms.openlocfilehash: a76e3ccfc5afa79b145242d2c07e45ff3335587c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342108"
---
# <a name="oauth2permission-resource-type"></a><span data-ttu-id="767b1-105">oAuth2Permission リソースの種類</span><span class="sxs-lookup"><span data-stu-id="767b1-105">oAuth2Permission resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="767b1-106">OAuth 2.0 委任されたアクセス許可スコープを表します。</span><span class="sxs-lookup"><span data-stu-id="767b1-106">Represents an OAuth 2.0 delegated permission scope.</span></span> <span data-ttu-id="767b1-107">指定した OAuth 2.0 委任されたアクセス許可スコープは、リソースアプリケーションを呼び出すときに ( [application](application.md)オブジェクトの**requiredresourceaccess**コレクションを通じて) クライアントアプリケーションによって要求されることがあります。</span><span class="sxs-lookup"><span data-stu-id="767b1-107">The specified OAuth 2.0 delegated permission scopes may be requested by client applications (through the **requiredResourceAccess** collection on the [application](application.md) object) when calling a resource application.</span></span> <span data-ttu-id="767b1-108">[serviceprincipal](serviceprincipal.md)エンティティおよび[application](application.md)エンティティの**approles**プロパティは、 **oAuth2Permission**のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="767b1-108">The **appRoles** property of the [servicePrincipal](serviceprincipal.md) entity and of the [application](application.md) entity is a collection of **oAuth2Permission**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="767b1-109">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="767b1-109">JSON representation</span></span>

<span data-ttu-id="767b1-110">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="767b1-110">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="767b1-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="767b1-111">Properties</span></span>
| <span data-ttu-id="767b1-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="767b1-112">Property</span></span>     | <span data-ttu-id="767b1-113">型</span><span class="sxs-lookup"><span data-stu-id="767b1-113">Type</span></span>   |<span data-ttu-id="767b1-114">説明</span><span class="sxs-lookup"><span data-stu-id="767b1-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="767b1-115">admincon/説明</span><span class="sxs-lookup"><span data-stu-id="767b1-115">adminConsentDescription</span></span>|<span data-ttu-id="767b1-116">String</span><span class="sxs-lookup"><span data-stu-id="767b1-116">String</span></span>|<span data-ttu-id="767b1-117">管理者の同意とアプリの割り当てエクスペリエンスに表示されるアクセス許可ヘルプテキスト。</span><span class="sxs-lookup"><span data-stu-id="767b1-117">Permission help text that appears in the admin consent and app assignment experiences.</span></span>|
|<span data-ttu-id="767b1-118">admincon/表示 displayname</span><span class="sxs-lookup"><span data-stu-id="767b1-118">adminConsentDisplayName</span></span>|<span data-ttu-id="767b1-119">String</span><span class="sxs-lookup"><span data-stu-id="767b1-119">String</span></span>|<span data-ttu-id="767b1-120">管理者の同意とアプリの割り当てエクスペリエンスに表示されるアクセス許可の表示名。</span><span class="sxs-lookup"><span data-stu-id="767b1-120">Display name for the permission that appears in the admin consent and app assignment experiences.</span></span>|
|<span data-ttu-id="767b1-121">id</span><span class="sxs-lookup"><span data-stu-id="767b1-121">id</span></span>|<span data-ttu-id="767b1-122">Guid</span><span class="sxs-lookup"><span data-stu-id="767b1-122">Guid</span></span>|<span data-ttu-id="767b1-123">oauth2Permissions コレクション内の一意のスコープアクセス許可識別子。</span><span class="sxs-lookup"><span data-stu-id="767b1-123">Unique scope permission identifier inside the oauth2Permissions collection.</span></span>|
|<span data-ttu-id="767b1-124">isEnabled</span><span class="sxs-lookup"><span data-stu-id="767b1-124">isEnabled</span></span>|<span data-ttu-id="767b1-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="767b1-125">Boolean</span></span>|<span data-ttu-id="767b1-126">アクセス許可を作成または更新する場合は、このプロパティを**true**に設定する必要があります (これは既定値です)。</span><span class="sxs-lookup"><span data-stu-id="767b1-126">When creating or updating a permission, this property must be set to **true** (which is the default).</span></span> <span data-ttu-id="767b1-127">権限を削除するには、最初にこのプロパティを**false**に設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="767b1-127">To delete a permission, this property must first be set to **false**.</span></span>  <span data-ttu-id="767b1-128">その時点で、以降の呼び出しでは、アクセス許可が削除されることがあります。</span><span class="sxs-lookup"><span data-stu-id="767b1-128">At that point, in a subsequent call, the permission may be removed.</span></span>|
|<span data-ttu-id="767b1-129">type</span><span class="sxs-lookup"><span data-stu-id="767b1-129">type</span></span>|<span data-ttu-id="767b1-130">String</span><span class="sxs-lookup"><span data-stu-id="767b1-130">String</span></span>|<span data-ttu-id="767b1-131">この範囲のアクセス許可をエンドユーザーが同意することができるかどうか、または会社の管理者が同意する必要があるテナント全体のアクセス許可であるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="767b1-131">Specifies whether this scope permission can be consented to by an end user, or whether it is a tenant-wide permission that must be consented to by a Company Administrator.</span></span>  <span data-ttu-id="767b1-132">可能な値は、"User" または "Admin" です。</span><span class="sxs-lookup"><span data-stu-id="767b1-132">Possible values are "User" or "Admin".</span></span>|
|<span data-ttu-id="767b1-133">usercondescription の説明</span><span class="sxs-lookup"><span data-stu-id="767b1-133">userConsentDescription</span></span>|<span data-ttu-id="767b1-134">String</span><span class="sxs-lookup"><span data-stu-id="767b1-134">String</span></span>|<span data-ttu-id="767b1-135">エンドユーザーの同意画面に表示されるアクセス許可ヘルプテキスト。</span><span class="sxs-lookup"><span data-stu-id="767b1-135">Permission help text that appears in the end user consent experience.</span></span>|
|<span data-ttu-id="767b1-136">usercon使い方 displayname</span><span class="sxs-lookup"><span data-stu-id="767b1-136">userConsentDisplayName</span></span>|<span data-ttu-id="767b1-137">String</span><span class="sxs-lookup"><span data-stu-id="767b1-137">String</span></span>|<span data-ttu-id="767b1-138">エンドユーザーの同意画面に表示されるアクセス許可の表示名。</span><span class="sxs-lookup"><span data-stu-id="767b1-138">Display name for the permission that appears in the end user consent experience.</span></span>|
|<span data-ttu-id="767b1-139">value</span><span class="sxs-lookup"><span data-stu-id="767b1-139">value</span></span>|<span data-ttu-id="767b1-140">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="767b1-140">String</span></span>|<span data-ttu-id="767b1-141">OAuth 2.0 アクセストークンで想定されるリソースアプリケーションのスコープ要求の値。</span><span class="sxs-lookup"><span data-stu-id="767b1-141">The value of the scope claim that the resource application should expect in the OAuth 2.0 access token.</span></span>|

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
