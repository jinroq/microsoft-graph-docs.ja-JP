---
title: appRoleAssignment を作成する
description: この API を使用して、新しい appRoleAssignment を作成します。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 5e78229f1e23afc185def38e4dc2b615e2714dbc
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36363915"
---
# <a name="create-approleassignment"></a><span data-ttu-id="38b50-103">appRoleAssignment を作成する</span><span class="sxs-lookup"><span data-stu-id="38b50-103">Create appRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38b50-104">この API を使用して、新しい appRoleAssignment を作成します。</span><span class="sxs-lookup"><span data-stu-id="38b50-104">Use this API to create a new appRoleAssignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="38b50-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="38b50-105">Permissions</span></span>
<span data-ttu-id="38b50-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="38b50-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38b50-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="38b50-108">Permission type</span></span>      | <span data-ttu-id="38b50-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="38b50-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="38b50-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="38b50-110">Delegated (work or school account)</span></span> | <span data-ttu-id="38b50-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="38b50-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="38b50-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="38b50-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="38b50-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="38b50-113">Not supported.</span></span>    |
|<span data-ttu-id="38b50-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="38b50-114">Application</span></span> | <span data-ttu-id="38b50-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="38b50-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="38b50-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="38b50-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/appRoleAssignments

```
## <a name="request-headers"></a><span data-ttu-id="38b50-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="38b50-117">Request headers</span></span>
| <span data-ttu-id="38b50-118">名前</span><span class="sxs-lookup"><span data-stu-id="38b50-118">Name</span></span>       | <span data-ttu-id="38b50-119">型</span><span class="sxs-lookup"><span data-stu-id="38b50-119">Type</span></span> | <span data-ttu-id="38b50-120">説明</span><span class="sxs-lookup"><span data-stu-id="38b50-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="38b50-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="38b50-121">Authorization</span></span>  | <span data-ttu-id="38b50-122">string</span><span class="sxs-lookup"><span data-stu-id="38b50-122">string</span></span>  | <span data-ttu-id="38b50-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="38b50-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="38b50-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="38b50-125">Request body</span></span>
<span data-ttu-id="38b50-126">要求本文で、 [Approleassignment](../resources/approleassignment.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="38b50-126">In the request body, supply a JSON representation of [appRoleAssignment](../resources/approleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="38b50-127">応答</span><span class="sxs-lookup"><span data-stu-id="38b50-127">Response</span></span>

<span data-ttu-id="38b50-128">成功した場合、この`201 Created`メソッドは応答コードと、応答本文で[approleassignment](../resources/approleassignment.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="38b50-128">If successful, this method returns `201 Created` response code and [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38b50-129">例</span><span class="sxs-lookup"><span data-stu-id="38b50-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="38b50-130">要求</span><span class="sxs-lookup"><span data-stu-id="38b50-130">Request</span></span>
<span data-ttu-id="38b50-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="38b50-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="38b50-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="38b50-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_approleassignment_from_serviceprincipal"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/appRoleAssignments
Content-type: application/json
Content-length: 233

{
  "creationTimestamp": "2016-10-19T10:37:00Z",
  "principalDisplayName": "principalDisplayName-value",
  "principalId": "principalId-value",
  "principalType": "principalType-value",
  "resourceDisplayName": "resourceDisplayName-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="38b50-133">C#</span><span class="sxs-lookup"><span data-stu-id="38b50-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-approleassignment-from-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="38b50-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="38b50-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-approleassignment-from-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="38b50-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="38b50-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-approleassignment-from-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="38b50-136">Java</span><span class="sxs-lookup"><span data-stu-id="38b50-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-approleassignment-from-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="38b50-137">要求本文で、 [Approleassignment](../resources/approleassignment.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="38b50-137">In the request body, supply a JSON representation of [appRoleAssignment](../resources/approleassignment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="38b50-138">応答</span><span class="sxs-lookup"><span data-stu-id="38b50-138">Response</span></span>
<span data-ttu-id="38b50-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="38b50-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 253

{
  "creationTimestamp": "2016-10-19T10:37:00Z",
  "id": "id-value",
  "principalDisplayName": "principalDisplayName-value",
  "principalId": "principalId-value",
  "principalType": "principalType-value",
  "resourceDisplayName": "resourceDisplayName-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create appRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
