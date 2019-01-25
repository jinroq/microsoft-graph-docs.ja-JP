---
title: oAuth2PermissionGrant リソースの種類
description: (サービス主体で表されます)、アプリケーションに与えられている OAuth 2.0 のスコープ (委任されたアクセス許可) をユーザーまたは管理者の承認プロセスの一環として表します。
localization_priority: Normal
ms.openlocfilehash: ea6486aedca4c3fcf73e59a5652ccf517fb01ddc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516925"
---
# <a name="oauth2permissiongrant-resource-type"></a><span data-ttu-id="d3d88-103">oAuth2PermissionGrant リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d3d88-103">oAuth2PermissionGrant resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3d88-104">(サービス主体で表されます)、アプリケーションに与えられている OAuth 2.0 のスコープ (委任されたアクセス許可) をユーザーまたは管理者の承認プロセスの一環として表します。</span><span class="sxs-lookup"><span data-stu-id="d3d88-104">Represents the OAuth 2.0 scopes (delegated permissions) that have been granted to an application (represented by a service principal) as part of the user or admin consent process.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d3d88-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d3d88-105">JSON representation</span></span>

<span data-ttu-id="d3d88-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="d3d88-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="d3d88-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d3d88-107">Properties</span></span>
| <span data-ttu-id="d3d88-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d3d88-108">Property</span></span>     | <span data-ttu-id="d3d88-109">型</span><span class="sxs-lookup"><span data-stu-id="d3d88-109">Type</span></span>   |<span data-ttu-id="d3d88-110">説明</span><span class="sxs-lookup"><span data-stu-id="d3d88-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d3d88-111">clientId</span><span class="sxs-lookup"><span data-stu-id="d3d88-111">clientId</span></span>|<span data-ttu-id="d3d88-112">String</span><span class="sxs-lookup"><span data-stu-id="d3d88-112">String</span></span>| <span data-ttu-id="d3d88-113">サービス ・ プリンシパルの id 付与 (resourceId プロパティによって表される) リソースにアクセスするときにユーザーを偽装するのに同意するものです。</span><span class="sxs-lookup"><span data-stu-id="d3d88-113">The id of the service principal granted consent to impersonate the user when accessing the resource (represented by the resourceId property).</span></span> |
|<span data-ttu-id="d3d88-114">consentType</span><span class="sxs-lookup"><span data-stu-id="d3d88-114">consentType</span></span>|<span data-ttu-id="d3d88-115">String</span><span class="sxs-lookup"><span data-stu-id="d3d88-115">String</span></span>| <span data-ttu-id="d3d88-116">同意が管理者 (組織) のため、個人に提供されるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d3d88-116">Indicates if consent was provided by the administrator (on behalf of the organization) or by an individual.</span></span> <span data-ttu-id="d3d88-117">可能な値は、"AllPrincipals" または "Principal" です。</span><span class="sxs-lookup"><span data-stu-id="d3d88-117">The possible values are *AllPrincipals* or *Principal*.</span></span> |
|<span data-ttu-id="d3d88-118">ExpiryTime</span><span class="sxs-lookup"><span data-stu-id="d3d88-118">expiryTime</span></span>|<span data-ttu-id="d3d88-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3d88-119">DateTimeOffset</span></span>| <span data-ttu-id="d3d88-120">現在、有効期限の時刻の値は無視されます。</span><span class="sxs-lookup"><span data-stu-id="d3d88-120">Currently, the expiry time value is ignored.</span></span> |
|<span data-ttu-id="d3d88-121">id</span><span class="sxs-lookup"><span data-stu-id="d3d88-121">id</span></span>|<span data-ttu-id="d3d88-122">String</span><span class="sxs-lookup"><span data-stu-id="d3d88-122">String</span></span>| <span data-ttu-id="d3d88-123">一意識別子</span><span class="sxs-lookup"><span data-stu-id="d3d88-123">Unique identifier.</span></span> <span data-ttu-id="d3d88-124">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d3d88-124">Read-only.</span></span>|
|<span data-ttu-id="d3d88-125">principalId</span><span class="sxs-lookup"><span data-stu-id="d3d88-125">principalId</span></span>|<span data-ttu-id="d3d88-126">String</span><span class="sxs-lookup"><span data-stu-id="d3d88-126">String</span></span>| <span data-ttu-id="d3d88-127">ConsentType が*AllPrincipals*である場合は、この値が null の場合と同意は、組織内のすべてのユーザーに適用されます。</span><span class="sxs-lookup"><span data-stu-id="d3d88-127">If consentType is *AllPrincipals* this value is null, and the consent applies to all users in the organization.</span></span> <span data-ttu-id="d3d88-128">ConsentType が*主体*の場合は、このプロパティは同意を付与し、そのユーザーに対してのみ適用されるユーザーの id を指定します。</span><span class="sxs-lookup"><span data-stu-id="d3d88-128">If consentType is *Principal*, then this property specifies the id of the user that granted consent and applies only for that user.</span></span> |
|<span data-ttu-id="d3d88-129">resourceId</span><span class="sxs-lookup"><span data-stu-id="d3d88-129">resourceId</span></span>|<span data-ttu-id="d3d88-130">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="d3d88-130">String</span></span>| <span data-ttu-id="d3d88-131">アクセスが許可されているリソース ・ サービス ・ プリンシパルの id を指定します。</span><span class="sxs-lookup"><span data-stu-id="d3d88-131">Specifies the id of the resource service principal to which access has been granted.</span></span> |
|<span data-ttu-id="d3d88-132">scope</span><span class="sxs-lookup"><span data-stu-id="d3d88-132">scope</span></span>|<span data-ttu-id="d3d88-133">String</span><span class="sxs-lookup"><span data-stu-id="d3d88-133">String</span></span>| <span data-ttu-id="d3d88-134">OAuth 2.0 のアクセス トークンには、リソース アプリケーションが期待する[スコープ](/graph/permissions-reference)の要求の値を指定します。</span><span class="sxs-lookup"><span data-stu-id="d3d88-134">Specifies the value of the [scope](/graph/permissions-reference) claim that the resource application should expect in the OAuth 2.0 access token.</span></span> <span data-ttu-id="d3d88-135">たとえば、 *User.Read*</span><span class="sxs-lookup"><span data-stu-id="d3d88-135">For example, *User.Read*</span></span> |
|<span data-ttu-id="d3d88-136">startTime</span><span class="sxs-lookup"><span data-stu-id="d3d88-136">startTime</span></span>|<span data-ttu-id="d3d88-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3d88-137">DateTimeOffset</span></span>| <span data-ttu-id="d3d88-138">現時点では、開始時刻の値は無視されます。</span><span class="sxs-lookup"><span data-stu-id="d3d88-138">Currently, the start time value is ignored.</span></span> |

## <a name="relationships"></a><span data-ttu-id="d3d88-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d3d88-139">Relationships</span></span>
<span data-ttu-id="d3d88-140">なし</span><span class="sxs-lookup"><span data-stu-id="d3d88-140">None</span></span>


## <a name="methods"></a><span data-ttu-id="d3d88-141">メソッド</span><span class="sxs-lookup"><span data-stu-id="d3d88-141">Methods</span></span>

| <span data-ttu-id="d3d88-142">メソッド</span><span class="sxs-lookup"><span data-stu-id="d3d88-142">Method</span></span>           | <span data-ttu-id="d3d88-143">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d3d88-143">Return Type</span></span>    |<span data-ttu-id="d3d88-144">説明</span><span class="sxs-lookup"><span data-stu-id="d3d88-144">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d3d88-145">OAuth2PermissionGrant を取得します。</span><span class="sxs-lookup"><span data-stu-id="d3d88-145">Get oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-get.md) | [<span data-ttu-id="d3d88-146">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="d3d88-146">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) |<span data-ttu-id="d3d88-147">OAuth2PermissionGrant オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d3d88-147">Read properties and relationships of oAuth2PermissionGrant object.</span></span>|
|[<span data-ttu-id="d3d88-148">リスト oAuth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="d3d88-148">List oAuth2PermissionGrants</span></span>](../api/oauth2permissiongrant-list.md) | <span data-ttu-id="d3d88-149">[oAuth2PermissionGrant](oauth2permissiongrant.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="d3d88-149">[oAuth2PermissionGrant](oauth2permissiongrant.md) collection</span></span> | <span data-ttu-id="d3d88-150">Oauth2PermissionGrant オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="d3d88-150">Retrieve a list of oauth2PermissionGrant objects.</span></span> |
|[<span data-ttu-id="d3d88-151">OAuth2PermissionGrant を更新します。</span><span class="sxs-lookup"><span data-stu-id="d3d88-151">Update oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-update.md) | [<span data-ttu-id="d3d88-152">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="d3d88-152">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) |<span data-ttu-id="d3d88-153">OAuth2PermissionGrant オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="d3d88-153">Update oAuth2PermissionGrant object.</span></span> |
|[<span data-ttu-id="d3d88-154">OAuth2PermissionGrant を削除します。</span><span class="sxs-lookup"><span data-stu-id="d3d88-154">Delete oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-delete.md) | <span data-ttu-id="d3d88-155">なし</span><span class="sxs-lookup"><span data-stu-id="d3d88-155">None</span></span> |<span data-ttu-id="d3d88-156">OAuth2PermissionGrant オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="d3d88-156">Delete oAuth2PermissionGrant object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oAuth2PermissionGrant resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/oauth2permissiongrant.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
