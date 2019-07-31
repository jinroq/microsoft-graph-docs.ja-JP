---
title: permissionScope リソースの種類
description: OAuth 2.0 委任されたアクセス許可スコープを表します。 指定した OAuth 2.0 委任されたアクセス許可スコープは、リソースアプリケーションを呼び出すときに (Application オブジェクトの**Requiredresourceaccess**コレクションを通じて) クライアントアプリケーションによって要求されることがあります。 ServicePrincipal エンティティおよび Application エンティティの**oauth2Permissions**プロパティは、 **OAuth2Permission**のコレクションです。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 59770460b8fbc3c0a8946eeed94adfbe027f20cc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966168"
---
# <a name="permissionscope-resource-type"></a><span data-ttu-id="0ec09-105">permissionScope リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0ec09-105">permissionScope resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ec09-106">OAuth 2.0 委任されたアクセス許可スコープを表します。</span><span class="sxs-lookup"><span data-stu-id="0ec09-106">Represents an OAuth 2.0 delegated permission scope.</span></span> <span data-ttu-id="0ec09-107">指定した OAuth 2.0 委任されたアクセス許可スコープは、リソースアプリケーションを呼び出すときに ( [application](application.md)オブジェクトの**requiredresourceaccess**コレクションを通じて) クライアントアプリケーションによって要求されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0ec09-107">The specified OAuth 2.0 delegated permission scopes may be requested by client applications (through the **requiredResourceAccess** collection on the [application](application.md) object) when calling a resource application.</span></span> <span data-ttu-id="0ec09-108">[Serviceprincipal](serviceprincipal.md)エンティティおよび[Application](application.md)エンティティの**oauth2Permissions**プロパティは、 **OAuth2Permission**のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="0ec09-108">The **oauth2Permissions** property of the [servicePrincipal](serviceprincipal.md) entity and of the [Application](application.md) entity is a collection of **OAuth2Permission**.</span></span>

## <a name="properties"></a><span data-ttu-id="0ec09-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0ec09-109">Properties</span></span>

| <span data-ttu-id="0ec09-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0ec09-110">Property</span></span> | <span data-ttu-id="0ec09-111">型</span><span class="sxs-lookup"><span data-stu-id="0ec09-111">Type</span></span> | <span data-ttu-id="0ec09-112">説明</span><span class="sxs-lookup"><span data-stu-id="0ec09-112">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="0ec09-113">Admincon/説明</span><span class="sxs-lookup"><span data-stu-id="0ec09-113">adminConsentDescription</span></span>|<span data-ttu-id="0ec09-114">String</span><span class="sxs-lookup"><span data-stu-id="0ec09-114">String</span></span>| <span data-ttu-id="0ec09-115">管理者の同意とアプリの割り当てエクスペリエンスに表示されるアクセス許可ヘルプテキスト。</span><span class="sxs-lookup"><span data-stu-id="0ec09-115">Permission help text that appears in the admin consent and app assignment experiences.</span></span> |
|<span data-ttu-id="0ec09-116">Admincon/表示 Displayname</span><span class="sxs-lookup"><span data-stu-id="0ec09-116">adminConsentDisplayName</span></span>|<span data-ttu-id="0ec09-117">String</span><span class="sxs-lookup"><span data-stu-id="0ec09-117">String</span></span>| <span data-ttu-id="0ec09-118">管理者の同意とアプリの割り当てエクスペリエンスに表示されるアクセス許可の表示名。</span><span class="sxs-lookup"><span data-stu-id="0ec09-118">Display name for the permission that appears in the admin consent and app assignment experiences.</span></span> |
|<span data-ttu-id="0ec09-119">id</span><span class="sxs-lookup"><span data-stu-id="0ec09-119">id</span></span>|<span data-ttu-id="0ec09-120">Guid</span><span class="sxs-lookup"><span data-stu-id="0ec09-120">Guid</span></span>| <span data-ttu-id="0ec09-121">Oauth2Permissions コレクション内の一意のスコープアクセス許可識別子。</span><span class="sxs-lookup"><span data-stu-id="0ec09-121">Unique scope permission identifier inside the oauth2Permissions collection.</span></span> |
|<span data-ttu-id="0ec09-122">isEnabled</span><span class="sxs-lookup"><span data-stu-id="0ec09-122">isEnabled</span></span>|<span data-ttu-id="0ec09-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ec09-123">Boolean</span></span>| <span data-ttu-id="0ec09-124">アクセス許可を作成または更新する場合は、このプロパティを**true**に設定する必要があります (これは既定値です)。</span><span class="sxs-lookup"><span data-stu-id="0ec09-124">When creating or updating a permission, this property must be set to **true** (which is the default).</span></span> <span data-ttu-id="0ec09-125">権限を削除するには、最初にこのプロパティを**false**に設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="0ec09-125">To delete a permission, this property must first be set to **false**.</span></span> <span data-ttu-id="0ec09-126">その時点で、以降の呼び出しでは、アクセス許可が削除されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0ec09-126">At that point, in a subsequent call, the permission may be removed.</span></span> |
|<span data-ttu-id="0ec09-127">戻す</span><span class="sxs-lookup"><span data-stu-id="0ec09-127">origin</span></span>|<span data-ttu-id="0ec09-128">String</span><span class="sxs-lookup"><span data-stu-id="0ec09-128">String</span></span>| <span data-ttu-id="0ec09-129">内部使用用。</span><span class="sxs-lookup"><span data-stu-id="0ec09-129">For internal use.</span></span> |
|<span data-ttu-id="0ec09-130">type</span><span class="sxs-lookup"><span data-stu-id="0ec09-130">type</span></span>|<span data-ttu-id="0ec09-131">String</span><span class="sxs-lookup"><span data-stu-id="0ec09-131">String</span></span>| <span data-ttu-id="0ec09-132">この範囲のアクセス許可をエンドユーザーが同意することができるかどうか、または会社の管理者が同意する必要があるテナント全体のアクセス許可であるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="0ec09-132">Specifies whether this scope permission can be consented to by an end user, or whether it is a tenant-wide permission that must be consented to by a company administrator.</span></span> <span data-ttu-id="0ec09-133">使用可能な値は、*ユーザー*または*管理者*です。</span><span class="sxs-lookup"><span data-stu-id="0ec09-133">Possible values are *User* or *Admin*.</span></span> |
|<span data-ttu-id="0ec09-134">Usercondescription の説明</span><span class="sxs-lookup"><span data-stu-id="0ec09-134">userConsentDescription</span></span>|<span data-ttu-id="0ec09-135">String</span><span class="sxs-lookup"><span data-stu-id="0ec09-135">String</span></span>| <span data-ttu-id="0ec09-136">エンドユーザーの同意に表示されるアクセス許可ヘルプテキスト。</span><span class="sxs-lookup"><span data-stu-id="0ec09-136">Permission help text that appears in the end-user consent experience.</span></span> |
|<span data-ttu-id="0ec09-137">Usercon使い方 Displayname</span><span class="sxs-lookup"><span data-stu-id="0ec09-137">userConsentDisplayName</span></span>|<span data-ttu-id="0ec09-138">String</span><span class="sxs-lookup"><span data-stu-id="0ec09-138">String</span></span>| <span data-ttu-id="0ec09-139">エンドユーザーの同意に表示されるアクセス許可の表示名。</span><span class="sxs-lookup"><span data-stu-id="0ec09-139">Display name for the permission that appears in the end-user consent experience.</span></span> |
|<span data-ttu-id="0ec09-140">value</span><span class="sxs-lookup"><span data-stu-id="0ec09-140">value</span></span>|<span data-ttu-id="0ec09-141">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="0ec09-141">String</span></span>| <span data-ttu-id="0ec09-142">OAuth 2.0 アクセストークンで想定されるリソースアプリケーションのスコープ要求の値。</span><span class="sxs-lookup"><span data-stu-id="0ec09-142">The value of the scope claim that the resource application should expect in the OAuth 2.0 access token.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0ec09-143">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0ec09-143">JSON representation</span></span>
<span data-ttu-id="0ec09-144">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0ec09-144">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
