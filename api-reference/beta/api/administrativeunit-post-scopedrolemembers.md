---
title: ScopedRoleMember を追加する
description: '新しい scopedRoleMembership を追加します。 注: スコープ付きの役割メンバーシップでは、現在、*ユーザーアカウント管理*者と*ヘルプデスク管理者*ロールのみがサポートされています。'
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 218080112c4b14e514896447ea0a4b360db08aab
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36318940"
---
# <a name="add-a-scopedrolemember"></a><span data-ttu-id="232d6-104">ScopedRoleMember を追加する</span><span class="sxs-lookup"><span data-stu-id="232d6-104">Add a scopedRoleMember</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="232d6-105">新しい[scopedRoleMembership](../resources/scopedrolemembership.md)を追加します。</span><span class="sxs-lookup"><span data-stu-id="232d6-105">Add a new [scopedRoleMembership](../resources/scopedrolemembership.md).</span></span> <span data-ttu-id="232d6-106">注: スコープ付きの役割メンバーシップでは、現在、*ユーザーアカウント管理*者と*ヘルプデスク管理者*ロールのみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="232d6-106">NOTE: Only the *User account administrator* and *Helpdesk administrator* roles are currently supported for scoped-role memberships.</span></span>

## <a name="permissions"></a><span data-ttu-id="232d6-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="232d6-107">Permissions</span></span>
<span data-ttu-id="232d6-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="232d6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="232d6-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="232d6-110">Permission type</span></span>      | <span data-ttu-id="232d6-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="232d6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="232d6-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="232d6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="232d6-113">RoleManagement、Directory.accessasuser.all、およびすべてのディレクトリ</span><span class="sxs-lookup"><span data-stu-id="232d6-113">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="232d6-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="232d6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="232d6-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="232d6-115">Not supported.</span></span>    |
|<span data-ttu-id="232d6-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="232d6-116">Application</span></span> | <span data-ttu-id="232d6-117">RoleManagement</span><span class="sxs-lookup"><span data-stu-id="232d6-117">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="232d6-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="232d6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits/{id}/scopedRoleMembers
```
## <a name="request-headers"></a><span data-ttu-id="232d6-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="232d6-119">Request headers</span></span>
| <span data-ttu-id="232d6-120">名前</span><span class="sxs-lookup"><span data-stu-id="232d6-120">Name</span></span>      |<span data-ttu-id="232d6-121">説明</span><span class="sxs-lookup"><span data-stu-id="232d6-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="232d6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="232d6-122">Authorization</span></span>  | <span data-ttu-id="232d6-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="232d6-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="232d6-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="232d6-125">Request body</span></span>
<span data-ttu-id="232d6-126">要求本文で、 [scopedRoleMembership](../resources/scopedrolemembership.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="232d6-126">In the request body, supply a JSON representation of [scopedRoleMembership](../resources/scopedrolemembership.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="232d6-127">応答</span><span class="sxs-lookup"><span data-stu-id="232d6-127">Response</span></span>

<span data-ttu-id="232d6-128">成功した場合、この`201 Created`メソッドは応答コードと、応答本文で[scopedRoleMembership](../resources/scopedrolemembership.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="232d6-128">If successful, this method returns `201 Created` response code and [scopedRoleMembership](../resources/scopedrolemembership.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="232d6-129">例</span><span class="sxs-lookup"><span data-stu-id="232d6-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="232d6-130">要求</span><span class="sxs-lookup"><span data-stu-id="232d6-130">Request</span></span>
<span data-ttu-id="232d6-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="232d6-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="232d6-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="232d6-132">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="232d6-133">C#</span><span class="sxs-lookup"><span data-stu-id="232d6-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-scopedrolemembership-from-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="232d6-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="232d6-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-scopedrolemembership-from-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="232d6-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="232d6-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-scopedrolemembership-from-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="232d6-136">Java</span><span class="sxs-lookup"><span data-stu-id="232d6-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-scopedrolemembership-from-administrativeunit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="232d6-137">要求本文で、 [scopedRoleMembership](../resources/scopedrolemembership.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="232d6-137">In the request body, supply a JSON representation of [scopedRoleMembership](../resources/scopedrolemembership.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="232d6-138">応答</span><span class="sxs-lookup"><span data-stu-id="232d6-138">Response</span></span>
<span data-ttu-id="232d6-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="232d6-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
