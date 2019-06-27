---
title: 契約を取得する
description: アグリーメントオブジェクトのプロパティと関係を取得します。
localization_priority: Normal
ms.openlocfilehash: b500aa5a18fff6e2554dddea76dd02201e4467e8
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258640"
---
# <a name="get-agreement"></a><span data-ttu-id="d3022-103">契約を取得する</span><span class="sxs-lookup"><span data-stu-id="d3022-103">Get agreement</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3022-104">[アグリーメント](../resources/agreement.md)オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="d3022-104">Retrieve the properties and relationships of an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d3022-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d3022-105">Permissions</span></span>
<span data-ttu-id="d3022-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d3022-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3022-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d3022-108">Permission type</span></span>                        | <span data-ttu-id="d3022-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d3022-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="d3022-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d3022-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="d3022-111">Agreement.Read.All</span><span class="sxs-lookup"><span data-stu-id="d3022-111">Agreement.Read.All</span></span> |
|<span data-ttu-id="d3022-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d3022-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3022-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d3022-113">Not supported.</span></span> |
|<span data-ttu-id="d3022-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d3022-114">Application</span></span>                            | <span data-ttu-id="d3022-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d3022-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d3022-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d3022-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /agreements/<id>
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="d3022-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d3022-117">Request headers</span></span>
| <span data-ttu-id="d3022-118">名前</span><span class="sxs-lookup"><span data-stu-id="d3022-118">Name</span></span>         | <span data-ttu-id="d3022-119">型</span><span class="sxs-lookup"><span data-stu-id="d3022-119">Type</span></span>        | <span data-ttu-id="d3022-120">説明</span><span class="sxs-lookup"><span data-stu-id="d3022-120">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="d3022-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d3022-121">Authorization</span></span> | <span data-ttu-id="d3022-122">string</span><span class="sxs-lookup"><span data-stu-id="d3022-122">string</span></span> | <span data-ttu-id="d3022-p102">ベアラー \{トークン\}。必須。</span><span class="sxs-lookup"><span data-stu-id="d3022-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d3022-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="d3022-125">Request body</span></span>
<span data-ttu-id="d3022-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d3022-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d3022-127">応答</span><span class="sxs-lookup"><span data-stu-id="d3022-127">Response</span></span>
<span data-ttu-id="d3022-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[アグリーメント](../resources/agreement.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d3022-128">If successful, this method returns a `200 OK` response code and [agreement](../resources/agreement.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d3022-129">例</span><span class="sxs-lookup"><span data-stu-id="d3022-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d3022-130">要求</span><span class="sxs-lookup"><span data-stu-id="d3022-130">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_agreement"
}-->
```http
GET https://graph.microsoft.com/beta/agreements/<id>?$expand=files
```
##### <a name="response"></a><span data-ttu-id="d3022-131">応答</span><span class="sxs-lookup"><span data-stu-id="d3022-131">Response</span></span>
><span data-ttu-id="d3022-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="d3022-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreement"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "displayName": "MSGraph Sample",
  "isViewingBeforeAcceptanceRequired": true,
  "id": "id-value",
  "files": [
    {
      "id": "id-value",
      "language": "en",
      "fileName": "TOU.pdf",
      "isDefault": true
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="d3022-134">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="d3022-134">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d3022-135">C#</span><span class="sxs-lookup"><span data-stu-id="d3022-135">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_agreement-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d3022-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="d3022-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_agreement-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d3022-137">目的-C</span><span class="sxs-lookup"><span data-stu-id="d3022-137">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_agreement-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/agreement-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/agreement-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/agreement-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
