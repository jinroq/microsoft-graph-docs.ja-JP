---
title: permissionscope リソースの種類
description: OAuth 2.0 委任されたアクセス許可スコープを表します。 指定した OAuth 2.0 委任されたアクセス許可スコープは、リソースアプリケーションを呼び出すときに (Application オブジェクトの**requiredresourceaccess**コレクションを通じて) クライアントアプリケーションによって要求されることがあります。 serviceprincipal エンティティおよび Application エンティティの**oauth2Permissions**プロパティは、 **OAuth2Permission**のコレクションです。
localization_priority: Normal
ms.openlocfilehash: 6f45d2eb0645991eb55db8ef3338e3b6fcf300a7
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344995"
---
# <a name="permissionscope-resource-type"></a><span data-ttu-id="0837f-105">permissionscope リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0837f-105">permissionScope resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0837f-106">OAuth 2.0 委任されたアクセス許可スコープを表します。</span><span class="sxs-lookup"><span data-stu-id="0837f-106">Represents an OAuth 2.0 delegated permission scope.</span></span> <span data-ttu-id="0837f-107">指定した OAuth 2.0 委任されたアクセス許可スコープは、リソースアプリケーションを呼び出すときに ( [application](application.md)オブジェクトの**requiredresourceaccess**コレクションを通じて) クライアントアプリケーションによって要求されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0837f-107">The specified OAuth 2.0 delegated permission scopes may be requested by client applications (through the **requiredResourceAccess** collection on the [application](application.md) object) when calling a resource application.</span></span> <span data-ttu-id="0837f-108">[serviceprincipal](serviceprincipal.md)エンティティおよび[Application](application.md)エンティティの**oauth2Permissions**プロパティは、 **OAuth2Permission**のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="0837f-108">The **oauth2Permissions** property of the [servicePrincipal](serviceprincipal.md) entity and of the [Application](application.md) entity is a collection of **OAuth2Permission**.</span></span>

## <a name="properties"></a><span data-ttu-id="0837f-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0837f-109">Properties</span></span>

| <span data-ttu-id="0837f-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0837f-110">Property</span></span> | <span data-ttu-id="0837f-111">型</span><span class="sxs-lookup"><span data-stu-id="0837f-111">Type</span></span> | <span data-ttu-id="0837f-112">説明</span><span class="sxs-lookup"><span data-stu-id="0837f-112">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="0837f-113">admincon/説明</span><span class="sxs-lookup"><span data-stu-id="0837f-113">adminConsentDescription</span></span>|<span data-ttu-id="0837f-114">String</span><span class="sxs-lookup"><span data-stu-id="0837f-114">String</span></span>| <span data-ttu-id="0837f-115">管理者の同意とアプリの割り当てエクスペリエンスに表示されるアクセス許可ヘルプテキスト。</span><span class="sxs-lookup"><span data-stu-id="0837f-115">Permission help text that appears in the admin consent and app assignment experiences.</span></span> |
|<span data-ttu-id="0837f-116">admincon/表示 displayname</span><span class="sxs-lookup"><span data-stu-id="0837f-116">adminConsentDisplayName</span></span>|<span data-ttu-id="0837f-117">String</span><span class="sxs-lookup"><span data-stu-id="0837f-117">String</span></span>| <span data-ttu-id="0837f-118">管理者の同意とアプリの割り当てエクスペリエンスに表示されるアクセス許可の表示名。</span><span class="sxs-lookup"><span data-stu-id="0837f-118">Display name for the permission that appears in the admin consent and app assignment experiences.</span></span> |
|<span data-ttu-id="0837f-119">id</span><span class="sxs-lookup"><span data-stu-id="0837f-119">id</span></span>|<span data-ttu-id="0837f-120">Guid</span><span class="sxs-lookup"><span data-stu-id="0837f-120">Guid</span></span>| <span data-ttu-id="0837f-121">oauth2Permissions コレクション内の一意のスコープアクセス許可識別子。</span><span class="sxs-lookup"><span data-stu-id="0837f-121">Unique scope permission identifier inside the oauth2Permissions collection.</span></span> |
|<span data-ttu-id="0837f-122">isEnabled</span><span class="sxs-lookup"><span data-stu-id="0837f-122">isEnabled</span></span>|<span data-ttu-id="0837f-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="0837f-123">Boolean</span></span>| <span data-ttu-id="0837f-124">アクセス許可を作成または更新する場合は、このプロパティを**true**に設定する必要があります (これは既定値です)。</span><span class="sxs-lookup"><span data-stu-id="0837f-124">When creating or updating a permission, this property must be set to **true** (which is the default).</span></span> <span data-ttu-id="0837f-125">権限を削除するには、最初にこのプロパティを**false**に設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="0837f-125">To delete a permission, this property must first be set to **false**.</span></span> <span data-ttu-id="0837f-126">その時点で、以降の呼び出しでは、アクセス許可が削除されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0837f-126">At that point, in a subsequent call, the permission may be removed.</span></span> |
|<span data-ttu-id="0837f-127">戻す</span><span class="sxs-lookup"><span data-stu-id="0837f-127">origin</span></span>|<span data-ttu-id="0837f-128">String</span><span class="sxs-lookup"><span data-stu-id="0837f-128">String</span></span>| <span data-ttu-id="0837f-129">内部使用用。</span><span class="sxs-lookup"><span data-stu-id="0837f-129">For internal use.</span></span> |
|<span data-ttu-id="0837f-130">type</span><span class="sxs-lookup"><span data-stu-id="0837f-130">type</span></span>|<span data-ttu-id="0837f-131">String</span><span class="sxs-lookup"><span data-stu-id="0837f-131">String</span></span>| <span data-ttu-id="0837f-132">この範囲のアクセス許可をエンドユーザーが同意することができるかどうか、または会社の管理者が同意する必要があるテナント全体のアクセス許可であるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="0837f-132">Specifies whether this scope permission can be consented to by an end user, or whether it is a tenant-wide permission that must be consented to by a company administrator.</span></span> <span data-ttu-id="0837f-133">使用可能な値は、*ユーザー*または*管理者*です。</span><span class="sxs-lookup"><span data-stu-id="0837f-133">Possible values are *User* or *Admin*.</span></span> |
|<span data-ttu-id="0837f-134">usercondescription の説明</span><span class="sxs-lookup"><span data-stu-id="0837f-134">userConsentDescription</span></span>|<span data-ttu-id="0837f-135">String</span><span class="sxs-lookup"><span data-stu-id="0837f-135">String</span></span>| <span data-ttu-id="0837f-136">エンドユーザーの同意に表示されるアクセス許可ヘルプテキスト。</span><span class="sxs-lookup"><span data-stu-id="0837f-136">Permission help text that appears in the end-user consent experience.</span></span> |
|<span data-ttu-id="0837f-137">usercon使い方 displayname</span><span class="sxs-lookup"><span data-stu-id="0837f-137">userConsentDisplayName</span></span>|<span data-ttu-id="0837f-138">String</span><span class="sxs-lookup"><span data-stu-id="0837f-138">String</span></span>| <span data-ttu-id="0837f-139">エンドユーザーの同意に表示されるアクセス許可の表示名。</span><span class="sxs-lookup"><span data-stu-id="0837f-139">Display name for the permission that appears in the end-user consent experience.</span></span> |
|<span data-ttu-id="0837f-140">value</span><span class="sxs-lookup"><span data-stu-id="0837f-140">value</span></span>|<span data-ttu-id="0837f-141">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="0837f-141">String</span></span>| <span data-ttu-id="0837f-142">OAuth 2.0 アクセストークンで想定されるリソースアプリケーションのスコープ要求の値。</span><span class="sxs-lookup"><span data-stu-id="0837f-142">The value of the scope claim that the resource application should expect in the OAuth 2.0 access token.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0837f-143">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0837f-143">JSON representation</span></span>
<span data-ttu-id="0837f-144">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0837f-144">Here is a JSON representation of the resource.</span></span>

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
