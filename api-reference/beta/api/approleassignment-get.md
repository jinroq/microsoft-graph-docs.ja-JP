---
title: appRoleAssignment を取得する
description: approleassignment オブジェクトのプロパティとリレーションシップを取得します。
localization_priority: Priority
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 1b9eded012eba7ed9cd2e0354698dc982f219ceb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35945376"
---
# <a name="get-approleassignment"></a><span data-ttu-id="dffe0-103">appRoleAssignment を取得する</span><span class="sxs-lookup"><span data-stu-id="dffe0-103">Get appRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dffe0-104">approleassignment オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="dffe0-104">Retrieve the properties and relationships of approleassignment object.</span></span>
## <a name="permissions"></a><span data-ttu-id="dffe0-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="dffe0-105">Permissions</span></span>
<span data-ttu-id="dffe0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dffe0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dffe0-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="dffe0-108">Permission type</span></span>      | <span data-ttu-id="dffe0-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="dffe0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dffe0-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="dffe0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="dffe0-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="dffe0-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="dffe0-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="dffe0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dffe0-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dffe0-113">Not supported.</span></span>    |
|<span data-ttu-id="dffe0-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="dffe0-114">Application</span></span> | <span data-ttu-id="dffe0-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dffe0-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dffe0-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="dffe0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/appRoleAssignments/{id}
GET /servicePrincipals/{id}/appRoleAssignedTo
GET /groups/{id}/appRoleAssignments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="dffe0-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="dffe0-117">Optional query parameters</span></span>
<span data-ttu-id="dffe0-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="dffe0-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dffe0-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dffe0-119">Request headers</span></span>
| <span data-ttu-id="dffe0-120">名前</span><span class="sxs-lookup"><span data-stu-id="dffe0-120">Name</span></span>       | <span data-ttu-id="dffe0-121">種類</span><span class="sxs-lookup"><span data-stu-id="dffe0-121">Type</span></span> | <span data-ttu-id="dffe0-122">説明</span><span class="sxs-lookup"><span data-stu-id="dffe0-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="dffe0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dffe0-123">Authorization</span></span>  | <span data-ttu-id="dffe0-124">string</span><span class="sxs-lookup"><span data-stu-id="dffe0-124">string</span></span>  | <span data-ttu-id="dffe0-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="dffe0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dffe0-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="dffe0-127">Request body</span></span>
<span data-ttu-id="dffe0-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="dffe0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dffe0-129">応答</span><span class="sxs-lookup"><span data-stu-id="dffe0-129">Response</span></span>

<span data-ttu-id="dffe0-130">成功した場合、このメソッドは `200 OK` 応答コードと応答本文で [roleAssignment](../resources/approleassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="dffe0-130">If successful, this method returns a `200 OK` response code and [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="dffe0-131">例</span><span class="sxs-lookup"><span data-stu-id="dffe0-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dffe0-132">要求</span><span class="sxs-lookup"><span data-stu-id="dffe0-132">Request</span></span>
<span data-ttu-id="dffe0-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="dffe0-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="dffe0-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="dffe0-134">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_approleassignment"
}-->
```http
GET https://graph.microsoft.com/beta/appRoleAssignments/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dffe0-135">C#</span><span class="sxs-lookup"><span data-stu-id="dffe0-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-approleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dffe0-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="dffe0-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-approleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dffe0-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dffe0-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-approleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="dffe0-138">Java</span><span class="sxs-lookup"><span data-stu-id="dffe0-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-approleassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="dffe0-139">応答</span><span class="sxs-lookup"><span data-stu-id="dffe0-139">Response</span></span>
<span data-ttu-id="dffe0-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="dffe0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Get appRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
