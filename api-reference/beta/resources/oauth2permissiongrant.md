---
title: oAuth2PermissionGrant リソースの種類
description: ユーザーまたは管理者の同意プロセスの一部としてアプリケーション (サービスプリンシパルによって表される) に付与された OAuth 2.0 スコープ (デリゲートされたアクセス許可) を表します。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 25f012baca1a7dfa5aeb62b8885b00b151a657ed
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966616"
---
# <a name="oauth2permissiongrant-resource-type"></a><span data-ttu-id="83a0c-103">oAuth2PermissionGrant リソースの種類</span><span class="sxs-lookup"><span data-stu-id="83a0c-103">oAuth2PermissionGrant resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83a0c-104">ユーザーまたは管理者の同意プロセスの一部としてアプリケーション (サービスプリンシパルによって表される) に付与された OAuth 2.0 スコープ (デリゲートされたアクセス許可) を表します。</span><span class="sxs-lookup"><span data-stu-id="83a0c-104">Represents the OAuth 2.0 scopes (delegated permissions) that have been granted to an application (represented by a service principal) as part of the user or admin consent process.</span></span>

## <a name="json-representation"></a><span data-ttu-id="83a0c-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="83a0c-105">JSON representation</span></span>

<span data-ttu-id="83a0c-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="83a0c-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant"
}-->

```json
{
  "clientId": "string",
  "consentType": "string",
  "expiryTime": "String (timestamp)",
  "id": "string (identifier)",
  "principalId": "string",
  "resourceId": "string",
  "scope": "string",
  "startTime": "String (timestamp)"
}

```
## <a name="properties"></a><span data-ttu-id="83a0c-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="83a0c-107">Properties</span></span>
| <span data-ttu-id="83a0c-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="83a0c-108">Property</span></span>     | <span data-ttu-id="83a0c-109">型</span><span class="sxs-lookup"><span data-stu-id="83a0c-109">Type</span></span>   |<span data-ttu-id="83a0c-110">説明</span><span class="sxs-lookup"><span data-stu-id="83a0c-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="83a0c-111">clientId</span><span class="sxs-lookup"><span data-stu-id="83a0c-111">clientId</span></span>|<span data-ttu-id="83a0c-112">String</span><span class="sxs-lookup"><span data-stu-id="83a0c-112">String</span></span>| <span data-ttu-id="83a0c-113">リソースにアクセスするときにユーザーを偽装する同意を付与するサービスプリンシパルの id (resourceId プロパティで表されます)。</span><span class="sxs-lookup"><span data-stu-id="83a0c-113">The id of the service principal granted consent to impersonate the user when accessing the resource (represented by the resourceId property).</span></span> |
|<span data-ttu-id="83a0c-114">consentType</span><span class="sxs-lookup"><span data-stu-id="83a0c-114">consentType</span></span>|<span data-ttu-id="83a0c-115">String</span><span class="sxs-lookup"><span data-stu-id="83a0c-115">String</span></span>| <span data-ttu-id="83a0c-116">同意が管理者によって (組織の代わりに) 提供されたか、個人によって提供されたかを示します。</span><span class="sxs-lookup"><span data-stu-id="83a0c-116">Indicates if consent was provided by the administrator (on behalf of the organization) or by an individual.</span></span> <span data-ttu-id="83a0c-117">使用可能な値は*allprincipals*または*Principal*です。</span><span class="sxs-lookup"><span data-stu-id="83a0c-117">The possible values are *AllPrincipals* or *Principal*.</span></span> |
|<span data-ttu-id="83a0c-118">expiryTime</span><span class="sxs-lookup"><span data-stu-id="83a0c-118">expiryTime</span></span>|<span data-ttu-id="83a0c-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83a0c-119">DateTimeOffset</span></span>| <span data-ttu-id="83a0c-120">現時点では、有効期限の値は無視されます。</span><span class="sxs-lookup"><span data-stu-id="83a0c-120">Currently, the expiry time value is ignored.</span></span> |
|<span data-ttu-id="83a0c-121">id</span><span class="sxs-lookup"><span data-stu-id="83a0c-121">id</span></span>|<span data-ttu-id="83a0c-122">文字列</span><span class="sxs-lookup"><span data-stu-id="83a0c-122">String</span></span>| <span data-ttu-id="83a0c-123">一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="83a0c-123">Unique identifier.</span></span> <span data-ttu-id="83a0c-124">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="83a0c-124">Read-only.</span></span>|
|<span data-ttu-id="83a0c-125">principalId</span><span class="sxs-lookup"><span data-stu-id="83a0c-125">principalId</span></span>|<span data-ttu-id="83a0c-126">String</span><span class="sxs-lookup"><span data-stu-id="83a0c-126">String</span></span>| <span data-ttu-id="83a0c-127">Consettings Type が*Allprincipals*の場合、この値は null になり、組織内のすべてのユーザーに同意が適用されます。</span><span class="sxs-lookup"><span data-stu-id="83a0c-127">If consentType is *AllPrincipals* this value is null, and the consent applies to all users in the organization.</span></span> <span data-ttu-id="83a0c-128">Conな種類が*Principal*の場合、このプロパティは同意を付与されたユーザーの id を指定し、そのユーザーに対してのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="83a0c-128">If consentType is *Principal*, then this property specifies the id of the user that granted consent and applies only for that user.</span></span> |
|<span data-ttu-id="83a0c-129">resourceId</span><span class="sxs-lookup"><span data-stu-id="83a0c-129">resourceId</span></span>|<span data-ttu-id="83a0c-130">String</span><span class="sxs-lookup"><span data-stu-id="83a0c-130">String</span></span>| <span data-ttu-id="83a0c-131">アクセスが許可されているリソースサービスプリンシパルの id を指定します。</span><span class="sxs-lookup"><span data-stu-id="83a0c-131">Specifies the id of the resource service principal to which access has been granted.</span></span> |
|<span data-ttu-id="83a0c-132">scope</span><span class="sxs-lookup"><span data-stu-id="83a0c-132">scope</span></span>|<span data-ttu-id="83a0c-133">文字列</span><span class="sxs-lookup"><span data-stu-id="83a0c-133">String</span></span>| <span data-ttu-id="83a0c-134">OAuth 2.0 アクセストークンでリソースアプリケーションが想定する[スコープ](/graph/permissions-reference)要求の値を指定します。</span><span class="sxs-lookup"><span data-stu-id="83a0c-134">Specifies the value of the [scope](/graph/permissions-reference) claim that the resource application should expect in the OAuth 2.0 access token.</span></span> <span data-ttu-id="83a0c-135">たとえば、「ユーザー」と表示*します。*</span><span class="sxs-lookup"><span data-stu-id="83a0c-135">For example, *User.Read*</span></span> |
|<span data-ttu-id="83a0c-136">startTime</span><span class="sxs-lookup"><span data-stu-id="83a0c-136">startTime</span></span>|<span data-ttu-id="83a0c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83a0c-137">DateTimeOffset</span></span>| <span data-ttu-id="83a0c-138">現時点では、開始時刻の値は無視されます。</span><span class="sxs-lookup"><span data-stu-id="83a0c-138">Currently, the start time value is ignored.</span></span> |

## <a name="relationships"></a><span data-ttu-id="83a0c-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="83a0c-139">Relationships</span></span>
<span data-ttu-id="83a0c-140">なし</span><span class="sxs-lookup"><span data-stu-id="83a0c-140">None</span></span>


## <a name="methods"></a><span data-ttu-id="83a0c-141">メソッド</span><span class="sxs-lookup"><span data-stu-id="83a0c-141">Methods</span></span>

| <span data-ttu-id="83a0c-142">メソッド</span><span class="sxs-lookup"><span data-stu-id="83a0c-142">Method</span></span>           | <span data-ttu-id="83a0c-143">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="83a0c-143">Return Type</span></span>    |<span data-ttu-id="83a0c-144">説明</span><span class="sxs-lookup"><span data-stu-id="83a0c-144">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="83a0c-145">OAuth2PermissionGrant を取得する</span><span class="sxs-lookup"><span data-stu-id="83a0c-145">Get oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-get.md) | [<span data-ttu-id="83a0c-146">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="83a0c-146">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) |<span data-ttu-id="83a0c-147">OAuth2PermissionGrant オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="83a0c-147">Read properties and relationships of oAuth2PermissionGrant object.</span></span>|
|[<span data-ttu-id="83a0c-148">リスト oAuth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="83a0c-148">List oAuth2PermissionGrants</span></span>](../api/oauth2permissiongrant-list.md) | <span data-ttu-id="83a0c-149">[oAuth2PermissionGrant](oauth2permissiongrant.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="83a0c-149">[oAuth2PermissionGrant](oauth2permissiongrant.md) collection</span></span> | <span data-ttu-id="83a0c-150">Oauth2PermissionGrant オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="83a0c-150">Retrieve a list of oauth2PermissionGrant objects.</span></span> |
|[<span data-ttu-id="83a0c-151">OAuth2PermissionGrant の更新</span><span class="sxs-lookup"><span data-stu-id="83a0c-151">Update oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-update.md) | [<span data-ttu-id="83a0c-152">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="83a0c-152">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) |<span data-ttu-id="83a0c-153">OAuth2PermissionGrant オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="83a0c-153">Update oAuth2PermissionGrant object.</span></span> |
|[<span data-ttu-id="83a0c-154">OAuth2PermissionGrant の削除</span><span class="sxs-lookup"><span data-stu-id="83a0c-154">Delete oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-delete.md) | <span data-ttu-id="83a0c-155">None</span><span class="sxs-lookup"><span data-stu-id="83a0c-155">None</span></span> |<span data-ttu-id="83a0c-156">OAuth2PermissionGrant オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="83a0c-156">Delete oAuth2PermissionGrant object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oAuth2PermissionGrant resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
