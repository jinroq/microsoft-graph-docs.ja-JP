---
title: oAuth2PermissionGrant リソースの種類
description: ユーザーまたは管理者の同意プロセスの一部としてアプリケーション (サービスプリンシパルによって表される) に付与された OAuth 2.0 スコープ (デリゲートされたアクセス許可) を表します。
localization_priority: Normal
ms.openlocfilehash: ea6486aedca4c3fcf73e59a5652ccf517fb01ddc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581546"
---
# <a name="oauth2permissiongrant-resource-type"></a><span data-ttu-id="a6ba2-103">oAuth2PermissionGrant リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a6ba2-103">oAuth2PermissionGrant resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a6ba2-104">ユーザーまたは管理者の同意プロセスの一部としてアプリケーション (サービスプリンシパルによって表される) に付与された OAuth 2.0 スコープ (デリゲートされたアクセス許可) を表します。</span><span class="sxs-lookup"><span data-stu-id="a6ba2-104">Represents the OAuth 2.0 scopes (delegated permissions) that have been granted to an application (represented by a service principal) as part of the user or admin consent process.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a6ba2-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a6ba2-105">JSON representation</span></span>

<span data-ttu-id="a6ba2-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="a6ba2-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="a6ba2-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a6ba2-107">Properties</span></span>
| <span data-ttu-id="a6ba2-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a6ba2-108">Property</span></span>     | <span data-ttu-id="a6ba2-109">型</span><span class="sxs-lookup"><span data-stu-id="a6ba2-109">Type</span></span>   |<span data-ttu-id="a6ba2-110">説明</span><span class="sxs-lookup"><span data-stu-id="a6ba2-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a6ba2-111">clientId</span><span class="sxs-lookup"><span data-stu-id="a6ba2-111">clientId</span></span>|<span data-ttu-id="a6ba2-112">String</span><span class="sxs-lookup"><span data-stu-id="a6ba2-112">String</span></span>| <span data-ttu-id="a6ba2-113">リソースにアクセスするときにユーザーを偽装する同意を付与するサービスプリンシパルの id (resourceId プロパティで表されます)。</span><span class="sxs-lookup"><span data-stu-id="a6ba2-113">The id of the service principal granted consent to impersonate the user when accessing the resource (represented by the resourceId property).</span></span> |
|<span data-ttu-id="a6ba2-114">consentType</span><span class="sxs-lookup"><span data-stu-id="a6ba2-114">consentType</span></span>|<span data-ttu-id="a6ba2-115">String</span><span class="sxs-lookup"><span data-stu-id="a6ba2-115">String</span></span>| <span data-ttu-id="a6ba2-116">同意が管理者によって (組織の代わりに) 提供されたか、個人によって提供されたかを示します。</span><span class="sxs-lookup"><span data-stu-id="a6ba2-116">Indicates if consent was provided by the administrator (on behalf of the organization) or by an individual.</span></span> <span data-ttu-id="a6ba2-117">使用可能な値は*allprincipals*または*Principal*です。</span><span class="sxs-lookup"><span data-stu-id="a6ba2-117">The possible values are *AllPrincipals* or *Principal*.</span></span> |
|<span data-ttu-id="a6ba2-118">expiryTime</span><span class="sxs-lookup"><span data-stu-id="a6ba2-118">expiryTime</span></span>|<span data-ttu-id="a6ba2-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6ba2-119">DateTimeOffset</span></span>| <span data-ttu-id="a6ba2-120">現時点では、有効期限の値は無視されます。</span><span class="sxs-lookup"><span data-stu-id="a6ba2-120">Currently, the expiry time value is ignored.</span></span> |
|<span data-ttu-id="a6ba2-121">id</span><span class="sxs-lookup"><span data-stu-id="a6ba2-121">id</span></span>|<span data-ttu-id="a6ba2-122">String</span><span class="sxs-lookup"><span data-stu-id="a6ba2-122">String</span></span>| <span data-ttu-id="a6ba2-123">一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="a6ba2-123">Unique identifier.</span></span> <span data-ttu-id="a6ba2-124">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="a6ba2-124">Read-only.</span></span>|
|<span data-ttu-id="a6ba2-125">principalId</span><span class="sxs-lookup"><span data-stu-id="a6ba2-125">principalId</span></span>|<span data-ttu-id="a6ba2-126">String</span><span class="sxs-lookup"><span data-stu-id="a6ba2-126">String</span></span>| <span data-ttu-id="a6ba2-127">consettings type が*allprincipals*の場合、この値は null になり、組織内のすべてのユーザーに同意が適用されます。</span><span class="sxs-lookup"><span data-stu-id="a6ba2-127">If consentType is *AllPrincipals* this value is null, and the consent applies to all users in the organization.</span></span> <span data-ttu-id="a6ba2-128">conな種類が*Principal*の場合、このプロパティは同意を付与されたユーザーの id を指定し、そのユーザーに対してのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="a6ba2-128">If consentType is *Principal*, then this property specifies the id of the user that granted consent and applies only for that user.</span></span> |
|<span data-ttu-id="a6ba2-129">resourceId</span><span class="sxs-lookup"><span data-stu-id="a6ba2-129">resourceId</span></span>|<span data-ttu-id="a6ba2-130">String</span><span class="sxs-lookup"><span data-stu-id="a6ba2-130">String</span></span>| <span data-ttu-id="a6ba2-131">アクセスが許可されているリソースサービスプリンシパルの id を指定します。</span><span class="sxs-lookup"><span data-stu-id="a6ba2-131">Specifies the id of the resource service principal to which access has been granted.</span></span> |
|<span data-ttu-id="a6ba2-132">scope</span><span class="sxs-lookup"><span data-stu-id="a6ba2-132">scope</span></span>|<span data-ttu-id="a6ba2-133">文字列</span><span class="sxs-lookup"><span data-stu-id="a6ba2-133">String</span></span>| <span data-ttu-id="a6ba2-134">OAuth 2.0 アクセストークンでリソースアプリケーションが想定する[スコープ](/graph/permissions-reference)要求の値を指定します。</span><span class="sxs-lookup"><span data-stu-id="a6ba2-134">Specifies the value of the [scope](/graph/permissions-reference) claim that the resource application should expect in the OAuth 2.0 access token.</span></span> <span data-ttu-id="a6ba2-135">たとえば、「ユーザー」と表示*します。*</span><span class="sxs-lookup"><span data-stu-id="a6ba2-135">For example, *User.Read*</span></span> |
|<span data-ttu-id="a6ba2-136">startTime</span><span class="sxs-lookup"><span data-stu-id="a6ba2-136">startTime</span></span>|<span data-ttu-id="a6ba2-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6ba2-137">DateTimeOffset</span></span>| <span data-ttu-id="a6ba2-138">現時点では、開始時刻の値は無視されます。</span><span class="sxs-lookup"><span data-stu-id="a6ba2-138">Currently, the start time value is ignored.</span></span> |

## <a name="relationships"></a><span data-ttu-id="a6ba2-139">関係</span><span class="sxs-lookup"><span data-stu-id="a6ba2-139">Relationships</span></span>
<span data-ttu-id="a6ba2-140">なし</span><span class="sxs-lookup"><span data-stu-id="a6ba2-140">None</span></span>


## <a name="methods"></a><span data-ttu-id="a6ba2-141">メソッド</span><span class="sxs-lookup"><span data-stu-id="a6ba2-141">Methods</span></span>

| <span data-ttu-id="a6ba2-142">メソッド</span><span class="sxs-lookup"><span data-stu-id="a6ba2-142">Method</span></span>           | <span data-ttu-id="a6ba2-143">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a6ba2-143">Return Type</span></span>    |<span data-ttu-id="a6ba2-144">説明</span><span class="sxs-lookup"><span data-stu-id="a6ba2-144">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a6ba2-145">oAuth2PermissionGrant を取得する</span><span class="sxs-lookup"><span data-stu-id="a6ba2-145">Get oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-get.md) | [<span data-ttu-id="a6ba2-146">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="a6ba2-146">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) |<span data-ttu-id="a6ba2-147">oAuth2PermissionGrant オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="a6ba2-147">Read properties and relationships of oAuth2PermissionGrant object.</span></span>|
|[<span data-ttu-id="a6ba2-148">リスト oAuth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="a6ba2-148">List oAuth2PermissionGrants</span></span>](../api/oauth2permissiongrant-list.md) | <span data-ttu-id="a6ba2-149">[oAuth2PermissionGrant](oauth2permissiongrant.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a6ba2-149">[oAuth2PermissionGrant](oauth2permissiongrant.md) collection</span></span> | <span data-ttu-id="a6ba2-150">oauth2PermissionGrant オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="a6ba2-150">Retrieve a list of oauth2PermissionGrant objects.</span></span> |
|[<span data-ttu-id="a6ba2-151">oAuth2PermissionGrant の更新</span><span class="sxs-lookup"><span data-stu-id="a6ba2-151">Update oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-update.md) | [<span data-ttu-id="a6ba2-152">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="a6ba2-152">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) |<span data-ttu-id="a6ba2-153">oAuth2PermissionGrant オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="a6ba2-153">Update oAuth2PermissionGrant object.</span></span> |
|[<span data-ttu-id="a6ba2-154">oAuth2PermissionGrant の削除</span><span class="sxs-lookup"><span data-stu-id="a6ba2-154">Delete oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-delete.md) | <span data-ttu-id="a6ba2-155">なし</span><span class="sxs-lookup"><span data-stu-id="a6ba2-155">None</span></span> |<span data-ttu-id="a6ba2-156">oAuth2PermissionGrant オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="a6ba2-156">Delete oAuth2PermissionGrant object.</span></span> |

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
