---
title: agreementAcceptances を一覧表示する
description: ユーザーの agreementAcceptance オブジェクトのリストを取得します。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d64915ee5e61521176a705ac5877ee449a01d60e
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36409002"
---
# <a name="list-agreementacceptances"></a><span data-ttu-id="1d8cc-103">agreementAcceptances を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="1d8cc-103">List agreementAcceptances</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1d8cc-104">ユーザーの[agreementAcceptance](../resources/agreementacceptance.md)オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="1d8cc-104">Retrieve a list of a user's [agreementAcceptance](../resources/agreementacceptance.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="1d8cc-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1d8cc-105">Permissions</span></span>
<span data-ttu-id="1d8cc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1d8cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d8cc-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1d8cc-108">Permission type</span></span>                        | <span data-ttu-id="1d8cc-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1d8cc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="1d8cc-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1d8cc-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="1d8cc-111">AgreementAcceptance.Read</span><span class="sxs-lookup"><span data-stu-id="1d8cc-111">AgreementAcceptance.Read</span></span> |
|<span data-ttu-id="1d8cc-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1d8cc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d8cc-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1d8cc-113">Not supported.</span></span> |
|<span data-ttu-id="1d8cc-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1d8cc-114">Application</span></span>                            | <span data-ttu-id="1d8cc-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1d8cc-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1d8cc-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1d8cc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/agreementAcceptances
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="1d8cc-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1d8cc-117">Request headers</span></span>
| <span data-ttu-id="1d8cc-118">名前</span><span class="sxs-lookup"><span data-stu-id="1d8cc-118">Name</span></span>      |<span data-ttu-id="1d8cc-119">説明</span><span class="sxs-lookup"><span data-stu-id="1d8cc-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1d8cc-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d8cc-120">Authorization</span></span> | <span data-ttu-id="1d8cc-121">ベアラー {トークン}</span><span class="sxs-lookup"><span data-stu-id="1d8cc-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="1d8cc-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="1d8cc-122">Request body</span></span>
<span data-ttu-id="1d8cc-123">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1d8cc-123">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="1d8cc-124">応答</span><span class="sxs-lookup"><span data-stu-id="1d8cc-124">Response</span></span>
<span data-ttu-id="1d8cc-125">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[agreementAcceptance](../resources/agreementacceptance.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="1d8cc-125">If successful, this method returns a `200 OK` response code and a collection of [agreementAcceptance](../resources/agreementacceptance.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1d8cc-126">例</span><span class="sxs-lookup"><span data-stu-id="1d8cc-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1d8cc-127">要求</span><span class="sxs-lookup"><span data-stu-id="1d8cc-127">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1d8cc-128">プロトコル</span><span class="sxs-lookup"><span data-stu-id="1d8cc-128">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_agreementacceptances"
}-->
```http
GET https://graph.microsoft.com/beta/me/agreementAcceptances
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1d8cc-129">C#</span><span class="sxs-lookup"><span data-stu-id="1d8cc-129">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-agreementacceptances-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1d8cc-130">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1d8cc-130">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-agreementacceptances-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1d8cc-131">目的-C</span><span class="sxs-lookup"><span data-stu-id="1d8cc-131">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-agreementacceptances-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1d8cc-132">応答</span><span class="sxs-lookup"><span data-stu-id="1d8cc-132">Response</span></span>
><span data-ttu-id="1d8cc-p102">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="1d8cc-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreementAcceptance",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 303

{
  "value": [
    {
      "agreementId": "agreementId-value",
      "userId": "userId-value",
      "agreementFileId": "agreementFileId-value",
      "recordedDateTime": "datetime-value",
      "userDisplayName": "userDisplayName-value",
      "userPrincipalName": "userPrincipalName-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List agreementAcceptances",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
