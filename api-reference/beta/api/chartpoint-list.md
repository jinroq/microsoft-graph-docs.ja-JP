---
title: List ChartPointsCollection
description: chartpoint オブジェクトのリストを取得します。
author: lumine2008
ms.openlocfilehash: 1541e93505da09cbadb4434e4d24133f59a13de9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328218"
---
# <a name="list-chartpointscollection"></a><span data-ttu-id="46a69-103">List ChartPointsCollection</span><span class="sxs-lookup"><span data-stu-id="46a69-103">List ChartPointsCollection</span></span>

> <span data-ttu-id="46a69-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="46a69-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="46a69-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="46a69-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="46a69-106">chartpoint オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="46a69-106">Retrieve a list of chartpoint objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="46a69-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="46a69-107">Permissions</span></span>
<span data-ttu-id="46a69-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="46a69-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46a69-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="46a69-110">Permission type</span></span>      | <span data-ttu-id="46a69-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="46a69-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="46a69-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="46a69-112">Delegated (work or school account)</span></span> | <span data-ttu-id="46a69-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="46a69-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="46a69-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="46a69-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46a69-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="46a69-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="46a69-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="46a69-116">Application</span></span> | <span data-ttu-id="46a69-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="46a69-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="46a69-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="46a69-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts(<name>)/series(<undefined>)/points
```
## <a name="optional-query-parameters"></a><span data-ttu-id="46a69-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="46a69-119">Optional query parameters</span></span>
<span data-ttu-id="46a69-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="46a69-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="46a69-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="46a69-121">Request headers</span></span>
| <span data-ttu-id="46a69-122">名前</span><span class="sxs-lookup"><span data-stu-id="46a69-122">Name</span></span>      |<span data-ttu-id="46a69-123">説明</span><span class="sxs-lookup"><span data-stu-id="46a69-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="46a69-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="46a69-124">Authorization</span></span>  | <span data-ttu-id="46a69-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="46a69-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="46a69-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="46a69-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="46a69-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="46a69-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="46a69-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="46a69-130">Request body</span></span>
<span data-ttu-id="46a69-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="46a69-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="46a69-132">応答</span><span class="sxs-lookup"><span data-stu-id="46a69-132">Response</span></span>

<span data-ttu-id="46a69-133">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [ChartPoint](../resources/chartpoint.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="46a69-133">If successful, this method returns a `200 OK` response code and collection of [ChartPoint](../resources/chartpoint.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="46a69-134">例</span><span class="sxs-lookup"><span data-stu-id="46a69-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="46a69-135">要求</span><span class="sxs-lookup"><span data-stu-id="46a69-135">Request</span></span>
<span data-ttu-id="46a69-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="46a69-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_chartpointscollection"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/series(<undefined>)/points
```
##### <a name="response"></a><span data-ttu-id="46a69-137">応答</span><span class="sxs-lookup"><span data-stu-id="46a69-137">Response</span></span>
<span data-ttu-id="46a69-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="46a69-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartPoint",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 57

{
  "value": [
    {
      "value": {
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List ChartPointsCollection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->