---
title: ScopedRoleMember を追加します。
description: 新しい scopedRoleMembership を追加します。 注:*ユーザー アカウントの管理者*と*ヘルプ デスクの管理者*の役割のみ現在サポートされてスコープ ロールのメンバーシップ。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e93dc3bc245b323e3c40fdd5678f4bfba495eafd
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571829"
---
# <a name="add-a-scopedrolemember"></a><span data-ttu-id="86c45-104">ScopedRoleMember を追加します。</span><span class="sxs-lookup"><span data-stu-id="86c45-104">Add a scopedRoleMember</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86c45-105">新しい[scopedRoleMembership](../resources/scopedrolemembership.md)を追加します。</span><span class="sxs-lookup"><span data-stu-id="86c45-105">Add a new [scopedRoleMembership](../resources/scopedrolemembership.md).</span></span> <span data-ttu-id="86c45-106">注:*ユーザー アカウントの管理者*と*ヘルプ デスクの管理者*の役割のみ現在サポートされてスコープ ロールのメンバーシップ。</span><span class="sxs-lookup"><span data-stu-id="86c45-106">NOTE: Only the *User account administrator* and *Helpdesk administrator* roles are currently supported for scoped-role memberships.</span></span>

## <a name="permissions"></a><span data-ttu-id="86c45-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="86c45-107">Permissions</span></span>
<span data-ttu-id="86c45-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="86c45-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="86c45-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="86c45-110">Permission type</span></span>      | <span data-ttu-id="86c45-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="86c45-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="86c45-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="86c45-112">Delegated (work or school account)</span></span> | <span data-ttu-id="86c45-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="86c45-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="86c45-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="86c45-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86c45-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="86c45-115">Not supported.</span></span>    |
|<span data-ttu-id="86c45-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="86c45-116">Application</span></span> | <span data-ttu-id="86c45-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="86c45-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="86c45-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="86c45-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits/{id}/scopedRoleMembers
```
## <a name="request-headers"></a><span data-ttu-id="86c45-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="86c45-119">Request headers</span></span>
| <span data-ttu-id="86c45-120">名前</span><span class="sxs-lookup"><span data-stu-id="86c45-120">Name</span></span>      |<span data-ttu-id="86c45-121">説明</span><span class="sxs-lookup"><span data-stu-id="86c45-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="86c45-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="86c45-122">Authorization</span></span>  | <span data-ttu-id="86c45-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="86c45-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="86c45-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="86c45-125">Request body</span></span>
<span data-ttu-id="86c45-126">要求の本文には、 [scopedRoleMembership](../resources/scopedrolemembership.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="86c45-126">In the request body, supply a JSON representation of [scopedRoleMembership](../resources/scopedrolemembership.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="86c45-127">応答</span><span class="sxs-lookup"><span data-stu-id="86c45-127">Response</span></span>

<span data-ttu-id="86c45-128">かどうかは成功すると、このメソッドを返します`201 Created`、応答の本体で応答コードと[scopedRoleMembership](../resources/scopedrolemembership.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="86c45-128">If successful, this method returns `201 Created` response code and [scopedRoleMembership](../resources/scopedrolemembership.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86c45-129">例</span><span class="sxs-lookup"><span data-stu-id="86c45-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="86c45-130">要求</span><span class="sxs-lookup"><span data-stu-id="86c45-130">Request</span></span>
<span data-ttu-id="86c45-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="86c45-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_scopedrolemembership_from_administrativeunit"
}-->
```http
POST https://graph.microsoft.com/beta/administrativeUnits/{id}/scopedRoleMembers
Content-type: application/json
Content-length: 272

{
  "roleId": "roleId-value",
  "roleMemberInfo": {
    "id": "id-value"
  }
}
```
<span data-ttu-id="86c45-132">要求の本文には、 [scopedRoleMembership](../resources/scopedrolemembership.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="86c45-132">In the request body, supply a JSON representation of [scopedRoleMembership](../resources/scopedrolemembership.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="86c45-133">応答</span><span class="sxs-lookup"><span data-stu-id="86c45-133">Response</span></span>
<span data-ttu-id="86c45-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="86c45-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.scopedRoleMembership"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 294

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#scopedRoleMemberships/$entity",
  "administrativeUnitId": "administrativeUnitId-value",
  "roleId": "roleId-value",
  "roleMemberInfo": {
    "id": "id-value",
    "displayName": "displayName-value",
    "userPrincipalName": "userPrincipalName-value"
  },
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create scopedRoleMembership",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/administrativeunit-post-scopedrolemembers.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
