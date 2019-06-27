---
title: agreementAcceptances を一覧表示する
description: ユーザーの agreementAcceptance オブジェクトのリストを取得します。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8ca6788bec02713131aaa6006e4327b85e85eff0
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35270302"
---
# <a name="list-agreementacceptances"></a><span data-ttu-id="ae992-103">agreementAcceptances を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="ae992-103">List agreementAcceptances</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae992-104">ユーザーの[agreementAcceptance](../resources/agreementacceptance.md)オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="ae992-104">Retrieve a list of a user's [agreementAcceptance](../resources/agreementacceptance.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="ae992-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ae992-105">Permissions</span></span>
<span data-ttu-id="ae992-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ae992-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae992-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ae992-108">Permission type</span></span>                        | <span data-ttu-id="ae992-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ae992-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae992-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ae992-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="ae992-111">AgreementAcceptance.Read</span><span class="sxs-lookup"><span data-stu-id="ae992-111">AgreementAcceptance.Read</span></span> |
|<span data-ttu-id="ae992-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ae992-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae992-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ae992-113">Not supported.</span></span> |
|<span data-ttu-id="ae992-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ae992-114">Application</span></span>                            | <span data-ttu-id="ae992-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ae992-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae992-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ae992-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/agreementAcceptances
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="ae992-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ae992-117">Request headers</span></span>
| <span data-ttu-id="ae992-118">名前</span><span class="sxs-lookup"><span data-stu-id="ae992-118">Name</span></span>      |<span data-ttu-id="ae992-119">説明</span><span class="sxs-lookup"><span data-stu-id="ae992-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ae992-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae992-120">Authorization</span></span> | <span data-ttu-id="ae992-121">ベアラー {トークン}</span><span class="sxs-lookup"><span data-stu-id="ae992-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="ae992-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="ae992-122">Request body</span></span>
<span data-ttu-id="ae992-123">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ae992-123">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="ae992-124">応答</span><span class="sxs-lookup"><span data-stu-id="ae992-124">Response</span></span>
<span data-ttu-id="ae992-125">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[agreementAcceptance](../resources/agreementacceptance.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="ae992-125">If successful, this method returns a `200 OK` response code and a collection of [agreementAcceptance](../resources/agreementacceptance.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ae992-126">例</span><span class="sxs-lookup"><span data-stu-id="ae992-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ae992-127">要求</span><span class="sxs-lookup"><span data-stu-id="ae992-127">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_agreementacceptances"
}-->
```http
GET https://graph.microsoft.com/beta/me/agreementAcceptances
```
##### <a name="response"></a><span data-ttu-id="ae992-128">応答</span><span class="sxs-lookup"><span data-stu-id="ae992-128">Response</span></span>
><span data-ttu-id="ae992-p102">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="ae992-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="ae992-131">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="ae992-131">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ae992-132">C#</span><span class="sxs-lookup"><span data-stu-id="ae992-132">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_agreementacceptances-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ae992-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="ae992-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_agreementacceptances-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="ae992-134">目的-C</span><span class="sxs-lookup"><span data-stu-id="ae992-134">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_agreementacceptances-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/user-list-agreementacceptances.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/user-list-agreementacceptances.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-list-agreementacceptances.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
