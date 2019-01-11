---
title: oAuth2PermissionGrant リソースの種類
description: (サービス主体で表されます)、アプリケーションに与えられている OAuth 2.0 のスコープ (委任されたアクセス許可) をユーザーまたは管理者の承認プロセスの一環として表します。
localization_priority: Normal
ms.openlocfilehash: 835e4a2c1a8d19c9c21e706adbf2f10a6a505bb3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884449"
---
# <a name="oauth2permissiongrant-resource-type"></a><span data-ttu-id="a9569-103">oAuth2PermissionGrant リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a9569-103">oAuth2PermissionGrant resource type</span></span>

> <span data-ttu-id="a9569-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a9569-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a9569-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a9569-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a9569-106">(サービス主体で表されます)、アプリケーションに与えられている OAuth 2.0 のスコープ (委任されたアクセス許可) をユーザーまたは管理者の承認プロセスの一環として表します。</span><span class="sxs-lookup"><span data-stu-id="a9569-106">Represents the OAuth 2.0 scopes (delegated permissions) that have been granted to an application (represented by a service principal) as part of the user or admin consent process.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a9569-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a9569-107">JSON representation</span></span>

<span data-ttu-id="a9569-108">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="a9569-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.oAuth2Permissiongrant"
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
## <a name="properties"></a><span data-ttu-id="a9569-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a9569-109">Properties</span></span>
| <span data-ttu-id="a9569-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a9569-110">Property</span></span>     | <span data-ttu-id="a9569-111">種類</span><span class="sxs-lookup"><span data-stu-id="a9569-111">Type</span></span>   |<span data-ttu-id="a9569-112">説明</span><span class="sxs-lookup"><span data-stu-id="a9569-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a9569-113">clientId</span><span class="sxs-lookup"><span data-stu-id="a9569-113">clientId</span></span>|<span data-ttu-id="a9569-114">String</span><span class="sxs-lookup"><span data-stu-id="a9569-114">String</span></span>| <span data-ttu-id="a9569-115">サービス ・ プリンシパルの id 付与 (resourceId プロパティによって表される) リソースにアクセスするときにユーザーを偽装するのに同意するものです。</span><span class="sxs-lookup"><span data-stu-id="a9569-115">The id of the service principal granted consent to impersonate the user when accessing the resource (represented by the resourceId property).</span></span> |
|<span data-ttu-id="a9569-116">consentType</span><span class="sxs-lookup"><span data-stu-id="a9569-116">consentType</span></span>|<span data-ttu-id="a9569-117">String</span><span class="sxs-lookup"><span data-stu-id="a9569-117">String</span></span>| <span data-ttu-id="a9569-118">同意が管理者 (組織) のため、個人に提供されるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="a9569-118">Indicates if consent was provided by the administrator (on behalf of the organization) or by an individual.</span></span> <span data-ttu-id="a9569-119">使用可能な値は、 *AllPrincipals*または*プリンシパル*です。</span><span class="sxs-lookup"><span data-stu-id="a9569-119">The possible values are *AllPrincipals* or *Principal*.</span></span> |
|<span data-ttu-id="a9569-120">expiryTime</span><span class="sxs-lookup"><span data-stu-id="a9569-120">expiryTime</span></span>|<span data-ttu-id="a9569-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9569-121">DateTimeOffset</span></span>| <span data-ttu-id="a9569-122">現在、有効期限の時刻の値は無視されます。</span><span class="sxs-lookup"><span data-stu-id="a9569-122">Currently, the expiry time value is ignored.</span></span> |
|<span data-ttu-id="a9569-123">id</span><span class="sxs-lookup"><span data-stu-id="a9569-123">id</span></span>|<span data-ttu-id="a9569-124">String</span><span class="sxs-lookup"><span data-stu-id="a9569-124">String</span></span>| <span data-ttu-id="a9569-125">一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="a9569-125">Unique identifier.</span></span> <span data-ttu-id="a9569-126">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a9569-126">Read-only.</span></span>|
|<span data-ttu-id="a9569-127">principalId</span><span class="sxs-lookup"><span data-stu-id="a9569-127">principalId</span></span>|<span data-ttu-id="a9569-128">String</span><span class="sxs-lookup"><span data-stu-id="a9569-128">String</span></span>| <span data-ttu-id="a9569-129">ConsentType が*AllPrincipals*である場合は、この値が null の場合と同意は、組織内のすべてのユーザーに適用されます。</span><span class="sxs-lookup"><span data-stu-id="a9569-129">If consentType is *AllPrincipals* this value is null, and the consent applies to all users in the organization.</span></span> <span data-ttu-id="a9569-130">ConsentType が*主体*の場合は、このプロパティは同意を付与し、そのユーザーに対してのみ適用されるユーザーの id を指定します。</span><span class="sxs-lookup"><span data-stu-id="a9569-130">If consentType is *Principal*, then this property specifies the id of the user that granted consent and applies only for that user.</span></span> |
|<span data-ttu-id="a9569-131">resourceId</span><span class="sxs-lookup"><span data-stu-id="a9569-131">resourceId</span></span>|<span data-ttu-id="a9569-132">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="a9569-132">String</span></span>| <span data-ttu-id="a9569-133">アクセスが許可されているリソース ・ サービス ・ プリンシパルの id を指定します。</span><span class="sxs-lookup"><span data-stu-id="a9569-133">Specifies the id of the resource service principal to which access has been granted.</span></span> |
|<span data-ttu-id="a9569-134">scope</span><span class="sxs-lookup"><span data-stu-id="a9569-134">scope</span></span>|<span data-ttu-id="a9569-135">String</span><span class="sxs-lookup"><span data-stu-id="a9569-135">String</span></span>| <span data-ttu-id="a9569-136">OAuth 2.0 のアクセス トークンには、リソース アプリケーションが期待する[スコープ](/graph/permissions-reference)の要求の値を指定します。</span><span class="sxs-lookup"><span data-stu-id="a9569-136">Specifies the value of the [scope](/graph/permissions-reference) claim that the resource application should expect in the OAuth 2.0 access token.</span></span> <span data-ttu-id="a9569-137">たとえば、 *User.Read*</span><span class="sxs-lookup"><span data-stu-id="a9569-137">For example, *User.Read*</span></span> |
|<span data-ttu-id="a9569-138">startTime</span><span class="sxs-lookup"><span data-stu-id="a9569-138">startTime</span></span>|<span data-ttu-id="a9569-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9569-139">DateTimeOffset</span></span>| <span data-ttu-id="a9569-140">現時点では、開始時刻の値は無視されます。</span><span class="sxs-lookup"><span data-stu-id="a9569-140">Currently, the start time value is ignored.</span></span> |

## <a name="relationships"></a><span data-ttu-id="a9569-141">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a9569-141">Relationships</span></span>
<span data-ttu-id="a9569-142">なし</span><span class="sxs-lookup"><span data-stu-id="a9569-142">None</span></span>


## <a name="methods"></a><span data-ttu-id="a9569-143">メソッド</span><span class="sxs-lookup"><span data-stu-id="a9569-143">Methods</span></span>

| <span data-ttu-id="a9569-144">メソッド</span><span class="sxs-lookup"><span data-stu-id="a9569-144">Method</span></span>           | <span data-ttu-id="a9569-145">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a9569-145">Return Type</span></span>    |<span data-ttu-id="a9569-146">説明</span><span class="sxs-lookup"><span data-stu-id="a9569-146">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a9569-147">OAuth2PermissionGrant を取得します。</span><span class="sxs-lookup"><span data-stu-id="a9569-147">Get oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-get.md) | [<span data-ttu-id="a9569-148">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="a9569-148">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) |<span data-ttu-id="a9569-149">OAuth2PermissionGrant オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a9569-149">Read properties and relationships of oAuth2PermissionGrant object.</span></span>|
|[<span data-ttu-id="a9569-150">リスト oAuth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="a9569-150">List oAuth2PermissionGrants</span></span>](../api/oauth2permissiongrant-list.md) | <span data-ttu-id="a9569-151">[oAuth2PermissionGrant](oauth2permissiongrant.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a9569-151">[oAuth2PermissionGrant](oauth2permissiongrant.md) collection</span></span> | <span data-ttu-id="a9569-152">Oauth2PermissionGrant オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="a9569-152">Retrieve a list of oauth2PermissionGrant objects.</span></span> |
|[<span data-ttu-id="a9569-153">OAuth2PermissionGrant を更新します。</span><span class="sxs-lookup"><span data-stu-id="a9569-153">Update oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-update.md) | [<span data-ttu-id="a9569-154">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="a9569-154">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) |<span data-ttu-id="a9569-155">OAuth2PermissionGrant オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="a9569-155">Update oAuth2PermissionGrant object.</span></span> |
|[<span data-ttu-id="a9569-156">OAuth2PermissionGrant を削除します。</span><span class="sxs-lookup"><span data-stu-id="a9569-156">Delete oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-delete.md) | <span data-ttu-id="a9569-157">なし</span><span class="sxs-lookup"><span data-stu-id="a9569-157">None</span></span> |<span data-ttu-id="a9569-158">OAuth2PermissionGrant オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="a9569-158">Delete oAuth2PermissionGrant object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "oAuth2PermissionGrant resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
