---
title: oAuth2Permission リソースの種類
description: OAuth 2.0 委任されたアクセス許可スコープを表します。 指定した OAuth 2.0 委任されたアクセス許可スコープは、リソースアプリケーションを呼び出すときに (application オブジェクトの**requiredresourceaccess**コレクションを通じて) クライアントアプリケーションによって要求されることがあります。 serviceprincipal エンティティおよび application エンティティの**approles**プロパティは、 **oAuth2Permission**のコレクションです。
localization_priority: Normal
ms.openlocfilehash: 8d8bb0bb5af17b7322bd6be37ac48ae9edbeba42
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581689"
---
# <a name="oauth2permission-resource-type"></a><span data-ttu-id="0e9a5-105">oAuth2Permission リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0e9a5-105">oAuth2Permission resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e9a5-106">OAuth 2.0 委任されたアクセス許可スコープを表します。</span><span class="sxs-lookup"><span data-stu-id="0e9a5-106">Represents an OAuth 2.0 delegated permission scope.</span></span> <span data-ttu-id="0e9a5-107">指定した OAuth 2.0 委任されたアクセス許可スコープは、リソースアプリケーションを呼び出すときに ( [application](application.md)オブジェクトの**requiredresourceaccess**コレクションを通じて) クライアントアプリケーションによって要求されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0e9a5-107">The specified OAuth 2.0 delegated permission scopes may be requested by client applications (through the **requiredResourceAccess** collection on the [application](application.md) object) when calling a resource application.</span></span> <span data-ttu-id="0e9a5-108">[serviceprincipal](serviceprincipal.md)エンティティおよび[application](application.md)エンティティの**approles**プロパティは、 **oAuth2Permission**のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="0e9a5-108">The **appRoles** property of the [servicePrincipal](serviceprincipal.md) entity and of the [application](application.md) entity is a collection of **oAuth2Permission**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="0e9a5-109">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0e9a5-109">JSON representation</span></span>

<span data-ttu-id="0e9a5-110">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="0e9a5-110">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="0e9a5-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0e9a5-111">Properties</span></span>
| <span data-ttu-id="0e9a5-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0e9a5-112">Property</span></span>     | <span data-ttu-id="0e9a5-113">型</span><span class="sxs-lookup"><span data-stu-id="0e9a5-113">Type</span></span>   |<span data-ttu-id="0e9a5-114">説明</span><span class="sxs-lookup"><span data-stu-id="0e9a5-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0e9a5-115">admincon/説明</span><span class="sxs-lookup"><span data-stu-id="0e9a5-115">adminConsentDescription</span></span>|<span data-ttu-id="0e9a5-116">String</span><span class="sxs-lookup"><span data-stu-id="0e9a5-116">String</span></span>|<span data-ttu-id="0e9a5-117">管理者の同意とアプリの割り当てエクスペリエンスに表示されるアクセス許可ヘルプテキスト。</span><span class="sxs-lookup"><span data-stu-id="0e9a5-117">Permission help text that appears in the admin consent and app assignment experiences.</span></span>|
|<span data-ttu-id="0e9a5-118">admincon/表示 displayname</span><span class="sxs-lookup"><span data-stu-id="0e9a5-118">adminConsentDisplayName</span></span>|<span data-ttu-id="0e9a5-119">String</span><span class="sxs-lookup"><span data-stu-id="0e9a5-119">String</span></span>|<span data-ttu-id="0e9a5-120">管理者の同意とアプリの割り当てエクスペリエンスに表示されるアクセス許可の表示名。</span><span class="sxs-lookup"><span data-stu-id="0e9a5-120">Display name for the permission that appears in the admin consent and app assignment experiences.</span></span>|
|<span data-ttu-id="0e9a5-121">id</span><span class="sxs-lookup"><span data-stu-id="0e9a5-121">id</span></span>|<span data-ttu-id="0e9a5-122">Guid</span><span class="sxs-lookup"><span data-stu-id="0e9a5-122">Guid</span></span>|<span data-ttu-id="0e9a5-123">oauth2Permissions コレクション内の一意のスコープアクセス許可識別子。</span><span class="sxs-lookup"><span data-stu-id="0e9a5-123">Unique scope permission identifier inside the oauth2Permissions collection.</span></span>|
|<span data-ttu-id="0e9a5-124">isEnabled</span><span class="sxs-lookup"><span data-stu-id="0e9a5-124">isEnabled</span></span>|<span data-ttu-id="0e9a5-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="0e9a5-125">Boolean</span></span>|<span data-ttu-id="0e9a5-126">アクセス許可を作成または更新する場合は、このプロパティを**true**に設定する必要があります (これは既定値です)。</span><span class="sxs-lookup"><span data-stu-id="0e9a5-126">When creating or updating a permission, this property must be set to **true** (which is the default).</span></span> <span data-ttu-id="0e9a5-127">権限を削除するには、最初にこのプロパティを**false**に設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="0e9a5-127">To delete a permission, this property must first be set to **false**.</span></span>  <span data-ttu-id="0e9a5-128">その時点で、以降の呼び出しでは、アクセス許可が削除されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0e9a5-128">At that point, in a subsequent call, the permission may be removed.</span></span>|
|<span data-ttu-id="0e9a5-129">type</span><span class="sxs-lookup"><span data-stu-id="0e9a5-129">type</span></span>|<span data-ttu-id="0e9a5-130">String</span><span class="sxs-lookup"><span data-stu-id="0e9a5-130">String</span></span>|<span data-ttu-id="0e9a5-131">この範囲のアクセス許可をエンドユーザーが同意することができるかどうか、または会社の管理者が同意する必要があるテナント全体のアクセス許可であるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="0e9a5-131">Specifies whether this scope permission can be consented to by an end user, or whether it is a tenant-wide permission that must be consented to by a Company Administrator.</span></span>  <span data-ttu-id="0e9a5-132">可能な値は、"User" または "Admin" です。</span><span class="sxs-lookup"><span data-stu-id="0e9a5-132">Possible values are "User" or "Admin".</span></span>|
|<span data-ttu-id="0e9a5-133">usercondescription の説明</span><span class="sxs-lookup"><span data-stu-id="0e9a5-133">userConsentDescription</span></span>|<span data-ttu-id="0e9a5-134">String</span><span class="sxs-lookup"><span data-stu-id="0e9a5-134">String</span></span>|<span data-ttu-id="0e9a5-135">エンドユーザーの同意画面に表示されるアクセス許可ヘルプテキスト。</span><span class="sxs-lookup"><span data-stu-id="0e9a5-135">Permission help text that appears in the end user consent experience.</span></span>|
|<span data-ttu-id="0e9a5-136">usercon使い方 displayname</span><span class="sxs-lookup"><span data-stu-id="0e9a5-136">userConsentDisplayName</span></span>|<span data-ttu-id="0e9a5-137">String</span><span class="sxs-lookup"><span data-stu-id="0e9a5-137">String</span></span>|<span data-ttu-id="0e9a5-138">エンドユーザーの同意画面に表示されるアクセス許可の表示名。</span><span class="sxs-lookup"><span data-stu-id="0e9a5-138">Display name for the permission that appears in the end user consent experience.</span></span>|
|<span data-ttu-id="0e9a5-139">value</span><span class="sxs-lookup"><span data-stu-id="0e9a5-139">value</span></span>|<span data-ttu-id="0e9a5-140">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="0e9a5-140">String</span></span>|<span data-ttu-id="0e9a5-141">OAuth 2.0 アクセストークンで想定されるリソースアプリケーションのスコープ要求の値。</span><span class="sxs-lookup"><span data-stu-id="0e9a5-141">The value of the scope claim that the resource application should expect in the OAuth 2.0 access token.</span></span>|

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
