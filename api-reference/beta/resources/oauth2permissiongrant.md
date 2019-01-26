---
title: oAuth2PermissionGrant リソースの種類
description: (サービス主体で表されます)、アプリケーションに与えられている OAuth 2.0 のスコープ (委任されたアクセス許可) をユーザーまたは管理者の承認プロセスの一環として表します。
localization_priority: Normal
ms.openlocfilehash: 5d3d900395843f39645f61d1b984e3ed4f79d476
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576970"
---
# <a name="oauth2permissiongrant-resource-type"></a><span data-ttu-id="2943c-103">oAuth2PermissionGrant リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2943c-103">oAuth2PermissionGrant resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2943c-104">(サービス主体で表されます)、アプリケーションに与えられている OAuth 2.0 のスコープ (委任されたアクセス許可) をユーザーまたは管理者の承認プロセスの一環として表します。</span><span class="sxs-lookup"><span data-stu-id="2943c-104">Represents the OAuth 2.0 scopes (delegated permissions) that have been granted to an application (represented by a service principal) as part of the user or admin consent process.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2943c-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2943c-105">JSON representation</span></span>

<span data-ttu-id="2943c-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="2943c-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="2943c-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2943c-107">Properties</span></span>
| <span data-ttu-id="2943c-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2943c-108">Property</span></span>     | <span data-ttu-id="2943c-109">型</span><span class="sxs-lookup"><span data-stu-id="2943c-109">Type</span></span>   |<span data-ttu-id="2943c-110">説明</span><span class="sxs-lookup"><span data-stu-id="2943c-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2943c-111">clientId</span><span class="sxs-lookup"><span data-stu-id="2943c-111">clientId</span></span>|<span data-ttu-id="2943c-112">String</span><span class="sxs-lookup"><span data-stu-id="2943c-112">String</span></span>| <span data-ttu-id="2943c-113">サービス ・ プリンシパルの id 付与 (resourceId プロパティによって表される) リソースにアクセスするときにユーザーを偽装するのに同意するものです。</span><span class="sxs-lookup"><span data-stu-id="2943c-113">The id of the service principal granted consent to impersonate the user when accessing the resource (represented by the resourceId property).</span></span> |
|<span data-ttu-id="2943c-114">consentType</span><span class="sxs-lookup"><span data-stu-id="2943c-114">consentType</span></span>|<span data-ttu-id="2943c-115">String</span><span class="sxs-lookup"><span data-stu-id="2943c-115">String</span></span>| <span data-ttu-id="2943c-116">同意が管理者 (組織) のため、個人に提供されるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2943c-116">Indicates if consent was provided by the administrator (on behalf of the organization) or by an individual.</span></span> <span data-ttu-id="2943c-117">使用可能な値は、 *AllPrincipals*または*プリンシパル*です。</span><span class="sxs-lookup"><span data-stu-id="2943c-117">The possible values are *AllPrincipals* or *Principal*.</span></span> |
|<span data-ttu-id="2943c-118">expiryTime</span><span class="sxs-lookup"><span data-stu-id="2943c-118">expiryTime</span></span>|<span data-ttu-id="2943c-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2943c-119">DateTimeOffset</span></span>| <span data-ttu-id="2943c-120">現在、有効期限の時刻の値は無視されます。</span><span class="sxs-lookup"><span data-stu-id="2943c-120">Currently, the expiry time value is ignored.</span></span> |
|<span data-ttu-id="2943c-121">id</span><span class="sxs-lookup"><span data-stu-id="2943c-121">id</span></span>|<span data-ttu-id="2943c-122">String</span><span class="sxs-lookup"><span data-stu-id="2943c-122">String</span></span>| <span data-ttu-id="2943c-123">一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="2943c-123">Unique identifier.</span></span> <span data-ttu-id="2943c-124">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="2943c-124">Read-only.</span></span>|
|<span data-ttu-id="2943c-125">principalId</span><span class="sxs-lookup"><span data-stu-id="2943c-125">principalId</span></span>|<span data-ttu-id="2943c-126">String</span><span class="sxs-lookup"><span data-stu-id="2943c-126">String</span></span>| <span data-ttu-id="2943c-127">ConsentType が*AllPrincipals*である場合は、この値が null の場合と同意は、組織内のすべてのユーザーに適用されます。</span><span class="sxs-lookup"><span data-stu-id="2943c-127">If consentType is *AllPrincipals* this value is null, and the consent applies to all users in the organization.</span></span> <span data-ttu-id="2943c-128">ConsentType が*主体*の場合は、このプロパティは同意を付与し、そのユーザーに対してのみ適用されるユーザーの id を指定します。</span><span class="sxs-lookup"><span data-stu-id="2943c-128">If consentType is *Principal*, then this property specifies the id of the user that granted consent and applies only for that user.</span></span> |
|<span data-ttu-id="2943c-129">resourceId</span><span class="sxs-lookup"><span data-stu-id="2943c-129">resourceId</span></span>|<span data-ttu-id="2943c-130">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="2943c-130">String</span></span>| <span data-ttu-id="2943c-131">アクセスが許可されているリソース ・ サービス ・ プリンシパルの id を指定します。</span><span class="sxs-lookup"><span data-stu-id="2943c-131">Specifies the id of the resource service principal to which access has been granted.</span></span> |
|<span data-ttu-id="2943c-132">scope</span><span class="sxs-lookup"><span data-stu-id="2943c-132">scope</span></span>|<span data-ttu-id="2943c-133">String</span><span class="sxs-lookup"><span data-stu-id="2943c-133">String</span></span>| <span data-ttu-id="2943c-134">OAuth 2.0 のアクセス トークンには、リソース アプリケーションが期待する[スコープ](/graph/permissions-reference)の要求の値を指定します。</span><span class="sxs-lookup"><span data-stu-id="2943c-134">Specifies the value of the [scope](/graph/permissions-reference) claim that the resource application should expect in the OAuth 2.0 access token.</span></span> <span data-ttu-id="2943c-135">たとえば、 *User.Read*</span><span class="sxs-lookup"><span data-stu-id="2943c-135">For example, *User.Read*</span></span> |
|<span data-ttu-id="2943c-136">startTime</span><span class="sxs-lookup"><span data-stu-id="2943c-136">startTime</span></span>|<span data-ttu-id="2943c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2943c-137">DateTimeOffset</span></span>| <span data-ttu-id="2943c-138">現時点では、開始時刻の値は無視されます。</span><span class="sxs-lookup"><span data-stu-id="2943c-138">Currently, the start time value is ignored.</span></span> |

## <a name="relationships"></a><span data-ttu-id="2943c-139">関係</span><span class="sxs-lookup"><span data-stu-id="2943c-139">Relationships</span></span>
<span data-ttu-id="2943c-140">なし</span><span class="sxs-lookup"><span data-stu-id="2943c-140">None</span></span>


## <a name="methods"></a><span data-ttu-id="2943c-141">メソッド</span><span class="sxs-lookup"><span data-stu-id="2943c-141">Methods</span></span>

| <span data-ttu-id="2943c-142">メソッド</span><span class="sxs-lookup"><span data-stu-id="2943c-142">Method</span></span>           | <span data-ttu-id="2943c-143">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="2943c-143">Return Type</span></span>    |<span data-ttu-id="2943c-144">説明</span><span class="sxs-lookup"><span data-stu-id="2943c-144">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2943c-145">OAuth2PermissionGrant を取得します。</span><span class="sxs-lookup"><span data-stu-id="2943c-145">Get oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-get.md) | [<span data-ttu-id="2943c-146">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="2943c-146">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) |<span data-ttu-id="2943c-147">OAuth2PermissionGrant オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2943c-147">Read properties and relationships of oAuth2PermissionGrant object.</span></span>|
|[<span data-ttu-id="2943c-148">リスト oAuth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="2943c-148">List oAuth2PermissionGrants</span></span>](../api/oauth2permissiongrant-list.md) | <span data-ttu-id="2943c-149">[oAuth2PermissionGrant](oauth2permissiongrant.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="2943c-149">[oAuth2PermissionGrant](oauth2permissiongrant.md) collection</span></span> | <span data-ttu-id="2943c-150">Oauth2PermissionGrant オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="2943c-150">Retrieve a list of oauth2PermissionGrant objects.</span></span> |
|[<span data-ttu-id="2943c-151">OAuth2PermissionGrant を更新します。</span><span class="sxs-lookup"><span data-stu-id="2943c-151">Update oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-update.md) | [<span data-ttu-id="2943c-152">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="2943c-152">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) |<span data-ttu-id="2943c-153">OAuth2PermissionGrant オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="2943c-153">Update oAuth2PermissionGrant object.</span></span> |
|[<span data-ttu-id="2943c-154">OAuth2PermissionGrant を削除します。</span><span class="sxs-lookup"><span data-stu-id="2943c-154">Delete oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-delete.md) | <span data-ttu-id="2943c-155">なし</span><span class="sxs-lookup"><span data-stu-id="2943c-155">None</span></span> |<span data-ttu-id="2943c-156">OAuth2PermissionGrant オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="2943c-156">Delete oAuth2PermissionGrant object.</span></span> |

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
