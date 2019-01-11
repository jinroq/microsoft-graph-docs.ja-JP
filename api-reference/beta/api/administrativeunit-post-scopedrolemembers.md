---
title: ScopedRoleMember を追加します。
description: 新しい scopedRoleMembership を追加します。 注:*ユーザー アカウントの管理者*と*ヘルプ デスクの管理者*の役割のみ現在サポートされてスコープ ロールのメンバーシップ。
localization_priority: Normal
ms.openlocfilehash: e2ff1803ac0357fa8fef9e1cf68b2ff78f877895
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860019"
---
# <a name="add-a-scopedrolemember"></a><span data-ttu-id="307df-104">ScopedRoleMember を追加します。</span><span class="sxs-lookup"><span data-stu-id="307df-104">Add a scopedRoleMember</span></span>

> <span data-ttu-id="307df-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="307df-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="307df-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="307df-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="307df-107">新しい[scopedRoleMembership](../resources/scopedrolemembership.md)を追加します。</span><span class="sxs-lookup"><span data-stu-id="307df-107">Add a new [scopedRoleMembership](../resources/scopedrolemembership.md).</span></span> <span data-ttu-id="307df-108">注:*ユーザー アカウントの管理者*と*ヘルプ デスクの管理者*の役割のみ現在サポートされてスコープ ロールのメンバーシップ。</span><span class="sxs-lookup"><span data-stu-id="307df-108">NOTE: Only the *User account administrator* and *Helpdesk administrator* roles are currently supported for scoped-role memberships.</span></span>

## <a name="permissions"></a><span data-ttu-id="307df-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="307df-109">Permissions</span></span>
<span data-ttu-id="307df-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="307df-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="307df-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="307df-112">Permission type</span></span>      | <span data-ttu-id="307df-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="307df-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="307df-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="307df-114">Delegated (work or school account)</span></span> | <span data-ttu-id="307df-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="307df-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="307df-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="307df-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="307df-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="307df-117">Not supported.</span></span>    |
|<span data-ttu-id="307df-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="307df-118">Application</span></span> | <span data-ttu-id="307df-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="307df-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="307df-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="307df-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits/{id}/scopedRoleMembers
```
## <a name="request-headers"></a><span data-ttu-id="307df-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="307df-121">Request headers</span></span>
| <span data-ttu-id="307df-122">名前</span><span class="sxs-lookup"><span data-stu-id="307df-122">Name</span></span>      |<span data-ttu-id="307df-123">説明</span><span class="sxs-lookup"><span data-stu-id="307df-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="307df-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="307df-124">Authorization</span></span>  | <span data-ttu-id="307df-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="307df-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="307df-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="307df-127">Request body</span></span>
<span data-ttu-id="307df-128">要求の本文には、 [scopedRoleMembership](../resources/scopedrolemembership.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="307df-128">In the request body, supply a JSON representation of [scopedRoleMembership](../resources/scopedrolemembership.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="307df-129">応答</span><span class="sxs-lookup"><span data-stu-id="307df-129">Response</span></span>

<span data-ttu-id="307df-130">かどうかは成功すると、このメソッドを返します`201 Created`、応答の本体で応答コードと[scopedRoleMembership](../resources/scopedrolemembership.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="307df-130">If successful, this method returns `201 Created` response code and [scopedRoleMembership](../resources/scopedrolemembership.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="307df-131">例</span><span class="sxs-lookup"><span data-stu-id="307df-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="307df-132">要求</span><span class="sxs-lookup"><span data-stu-id="307df-132">Request</span></span>
<span data-ttu-id="307df-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="307df-133">Here is an example of the request.</span></span>
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
<span data-ttu-id="307df-134">要求の本文には、 [scopedRoleMembership](../resources/scopedrolemembership.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="307df-134">In the request body, supply a JSON representation of [scopedRoleMembership](../resources/scopedrolemembership.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="307df-135">応答</span><span class="sxs-lookup"><span data-stu-id="307df-135">Response</span></span>
<span data-ttu-id="307df-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="307df-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.scopedrolemembership"
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
<!-- {
  "type": "#page.annotation",
  "description": "Create scopedRoleMembership",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
