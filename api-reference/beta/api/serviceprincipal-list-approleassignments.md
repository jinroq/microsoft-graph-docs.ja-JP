---
title: 'servicePrincipal: appRoleAssignments のリスト'
description: Approleassignment オブジェクトのリストを取得します。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: eb8e0d88612e24522d907cb5daabc5d76a1eb3b2
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36410332"
---
# <a name="serviceprincipal-list-approleassignments"></a><span data-ttu-id="fdfd8-103">servicePrincipal: appRoleAssignments のリスト</span><span class="sxs-lookup"><span data-stu-id="fdfd8-103">servicePrincipal: List appRoleAssignments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fdfd8-104">Approleassignment オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="fdfd8-104">Retrieve a list of approleassignment objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="fdfd8-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="fdfd8-105">Permissions</span></span>
<span data-ttu-id="fdfd8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fdfd8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fdfd8-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fdfd8-108">Permission type</span></span>      | <span data-ttu-id="fdfd8-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="fdfd8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fdfd8-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fdfd8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fdfd8-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fdfd8-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fdfd8-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fdfd8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fdfd8-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fdfd8-113">Not supported.</span></span>    |
|<span data-ttu-id="fdfd8-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fdfd8-114">Application</span></span> | <span data-ttu-id="fdfd8-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdfd8-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fdfd8-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fdfd8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/appRoleAssignments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fdfd8-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="fdfd8-117">Optional query parameters</span></span>
<span data-ttu-id="fdfd8-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="fdfd8-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fdfd8-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fdfd8-119">Request headers</span></span>
| <span data-ttu-id="fdfd8-120">名前</span><span class="sxs-lookup"><span data-stu-id="fdfd8-120">Name</span></span>       | <span data-ttu-id="fdfd8-121">型</span><span class="sxs-lookup"><span data-stu-id="fdfd8-121">Type</span></span> | <span data-ttu-id="fdfd8-122">説明</span><span class="sxs-lookup"><span data-stu-id="fdfd8-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="fdfd8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fdfd8-123">Authorization</span></span>  | <span data-ttu-id="fdfd8-124">string</span><span class="sxs-lookup"><span data-stu-id="fdfd8-124">string</span></span>  | <span data-ttu-id="fdfd8-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="fdfd8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fdfd8-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="fdfd8-127">Request body</span></span>
<span data-ttu-id="fdfd8-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="fdfd8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fdfd8-129">応答</span><span class="sxs-lookup"><span data-stu-id="fdfd8-129">Response</span></span>

<span data-ttu-id="fdfd8-130">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[approleassignment](../resources/approleassignment.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="fdfd8-130">If successful, this method returns a `200 OK` response code and collection of [appRoleAssignment](../resources/approleassignment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fdfd8-131">例</span><span class="sxs-lookup"><span data-stu-id="fdfd8-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fdfd8-132">要求</span><span class="sxs-lookup"><span data-stu-id="fdfd8-132">Request</span></span>
<span data-ttu-id="fdfd8-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fdfd8-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="fdfd8-134">プロトコル</span><span class="sxs-lookup"><span data-stu-id="fdfd8-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_approleassignments"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/appRoleAssignments
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fdfd8-135">C#</span><span class="sxs-lookup"><span data-stu-id="fdfd8-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-approleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fdfd8-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fdfd8-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-approleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fdfd8-137">目的-C</span><span class="sxs-lookup"><span data-stu-id="fdfd8-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-approleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="fdfd8-138">応答</span><span class="sxs-lookup"><span data-stu-id="fdfd8-138">Response</span></span>
<span data-ttu-id="fdfd8-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="fdfd8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 306

{
  "value": [
    {
      "creationTimestamp": "2016-10-19T10:37:00Z",
      "id": "id-value",
      "principalDisplayName": "principalDisplayName-value",
      "principalId": "principalId-value",
      "principalType": "principalType-value",
      "resourceDisplayName": "resourceDisplayName-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List appRoleAssignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
