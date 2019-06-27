---
title: DataPolicyOperation を取得する
description: DataPolicyOperation オブジェクトのプロパティを取得します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 01cf28480b8b0d8f54bba08fb74e46a633000b2f
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35276378"
---
# <a name="get-datapolicyoperation"></a><span data-ttu-id="79e18-103">DataPolicyOperation を取得する</span><span class="sxs-lookup"><span data-stu-id="79e18-103">Get dataPolicyOperation</span></span>

<span data-ttu-id="79e18-104">**DataPolicyOperation**オブジェクトのプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="79e18-104">Retrieve the properties of a **dataPolicyOperation** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="79e18-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="79e18-105">Permissions</span></span>
<span data-ttu-id="79e18-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="79e18-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79e18-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="79e18-108">Permission type</span></span>      | <span data-ttu-id="79e18-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="79e18-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="79e18-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="79e18-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="79e18-111">すべてのユーザーをエクスポートします。</span><span class="sxs-lookup"><span data-stu-id="79e18-111">User.Export.All, User.Read.All</span></span>  |
|<span data-ttu-id="79e18-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="79e18-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="79e18-113">該当なし</span><span class="sxs-lookup"><span data-stu-id="79e18-113">Not applicable</span></span>  |
|<span data-ttu-id="79e18-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="79e18-114">Application</span></span> | <span data-ttu-id="79e18-115">すべてのユーザーをエクスポートします。</span><span class="sxs-lookup"><span data-stu-id="79e18-115">User.Export.All, User.Read.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="79e18-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="79e18-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /dataPolicyOperations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="79e18-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="79e18-117">Request headers</span></span>
| <span data-ttu-id="79e18-118">名前</span><span class="sxs-lookup"><span data-stu-id="79e18-118">Name</span></span>      |<span data-ttu-id="79e18-119">説明</span><span class="sxs-lookup"><span data-stu-id="79e18-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="79e18-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="79e18-120">Authorization</span></span>  | <span data-ttu-id="79e18-121">ベアラー {トークン}</span><span class="sxs-lookup"><span data-stu-id="79e18-121">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="79e18-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="79e18-122">Request body</span></span>
<span data-ttu-id="79e18-123">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="79e18-123">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="79e18-124">応答</span><span class="sxs-lookup"><span data-stu-id="79e18-124">Response</span></span>
<span data-ttu-id="79e18-125">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[dataPolicyOperation](../resources/datapolicyoperation.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="79e18-125">If successful, this method returns a `200 OK` response code and a [dataPolicyOperation](../resources/datapolicyoperation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="79e18-126">例</span><span class="sxs-lookup"><span data-stu-id="79e18-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="79e18-127">要求</span><span class="sxs-lookup"><span data-stu-id="79e18-127">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_datapolicyoperation"
}-->
```http
GET https://graph.microsoft.com/v1.0/dataPolicyOperations/{id}
```
##### <a name="response"></a><span data-ttu-id="79e18-128">応答</span><span class="sxs-lookup"><span data-stu-id="79e18-128">Response</span></span>
><span data-ttu-id="79e18-p102">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="79e18-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.dataPolicyOperation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 212

{
  "completedDateTime": "datetime-value",
  "id": "id-value",
  "status": "status-value",
  "storageLocation": "storageLocation-value",
  "userId": "userId-value",
  "submittedDateTime": "datetime-value", 
  "progress": "double-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="79e18-131">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="79e18-131">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="79e18-132">C#</span><span class="sxs-lookup"><span data-stu-id="79e18-132">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_datapolicyoperation-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="79e18-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="79e18-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_datapolicyoperation-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="79e18-134">目的-C</span><span class="sxs-lookup"><span data-stu-id="79e18-134">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_datapolicyoperation-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get dataPolicyOperation",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/datapolicyoperation-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/datapolicyoperation-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/datapolicyoperation-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
