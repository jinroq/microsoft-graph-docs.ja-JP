---
title: WorkbookApplication を取得する
description: WorkbookApplication オブジェクトのプロパティとリレーションシップを取得します。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: a7b175ae9c9446f3e2938a75aab88eaadc642d9c
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35269441"
---
# <a name="get-workbookapplication"></a><span data-ttu-id="8655a-103">WorkbookApplication を取得する</span><span class="sxs-lookup"><span data-stu-id="8655a-103">Get workbookApplication</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8655a-104">WorkbookApplication オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="8655a-104">Retrieve the properties and relationships of workbookApplication object.</span></span>
## <a name="permissions"></a><span data-ttu-id="8655a-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8655a-105">Permissions</span></span>
<span data-ttu-id="8655a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8655a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8655a-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8655a-108">Permission type</span></span>      | <span data-ttu-id="8655a-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8655a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8655a-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8655a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8655a-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8655a-111">Not supported.</span></span>    |
|<span data-ttu-id="8655a-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8655a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8655a-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8655a-113">Not supported.</span></span>    |
|<span data-ttu-id="8655a-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8655a-114">Application</span></span> | <span data-ttu-id="8655a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8655a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8655a-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8655a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/application
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8655a-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="8655a-117">Optional query parameters</span></span>
<span data-ttu-id="8655a-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="8655a-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8655a-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8655a-119">Request headers</span></span>
| <span data-ttu-id="8655a-120">名前</span><span class="sxs-lookup"><span data-stu-id="8655a-120">Name</span></span>      |<span data-ttu-id="8655a-121">説明</span><span class="sxs-lookup"><span data-stu-id="8655a-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8655a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8655a-122">Authorization</span></span>  | <span data-ttu-id="8655a-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8655a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8655a-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="8655a-125">Request body</span></span>
<span data-ttu-id="8655a-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="8655a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8655a-127">応答</span><span class="sxs-lookup"><span data-stu-id="8655a-127">Response</span></span>

<span data-ttu-id="8655a-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[workbookApplication](../resources/workbookapplication.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8655a-128">If successful, this method returns a `200 OK` response code and [workbookApplication](../resources/workbookapplication.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8655a-129">例</span><span class="sxs-lookup"><span data-stu-id="8655a-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8655a-130">要求</span><span class="sxs-lookup"><span data-stu-id="8655a-130">Request</span></span>
<span data-ttu-id="8655a-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8655a-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_workbookApplication"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/application
```
##### <a name="response"></a><span data-ttu-id="8655a-132">応答</span><span class="sxs-lookup"><span data-stu-id="8655a-132">Response</span></span>
<span data-ttu-id="8655a-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8655a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookApplication"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 48

{
  "calculationMode": "calculationMode-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="8655a-136">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="8655a-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8655a-137">C#</span><span class="sxs-lookup"><span data-stu-id="8655a-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_workbookApplication-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8655a-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="8655a-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_workbookApplication-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="8655a-139">目的-C</span><span class="sxs-lookup"><span data-stu-id="8655a-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_workbookApplication-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get workbookApplication",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/workbookapplication-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/workbookapplication-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/workbookapplication-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
