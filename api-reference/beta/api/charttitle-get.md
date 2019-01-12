---
title: Get ChartTitle
description: charttitle オブジェクトのプロパティと関係を取得します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: be6450fc27df46549fbecc5c2a23c8e854d9407e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946379"
---
# <a name="get-charttitle"></a><span data-ttu-id="34526-103">Get ChartTitle</span><span class="sxs-lookup"><span data-stu-id="34526-103">Get ChartTitle</span></span>

> <span data-ttu-id="34526-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="34526-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="34526-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="34526-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="34526-106">charttitle オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="34526-106">Retrieve the properties and relationships of charttitle object.</span></span>
## <a name="permissions"></a><span data-ttu-id="34526-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="34526-107">Permissions</span></span>
<span data-ttu-id="34526-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="34526-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34526-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="34526-110">Permission type</span></span>      | <span data-ttu-id="34526-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="34526-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="34526-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="34526-112">Delegated (work or school account)</span></span> | <span data-ttu-id="34526-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="34526-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="34526-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="34526-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="34526-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="34526-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="34526-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="34526-116">Application</span></span> | <span data-ttu-id="34526-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="34526-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="34526-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="34526-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts(<name>)/title
```
## <a name="optional-query-parameters"></a><span data-ttu-id="34526-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="34526-119">Optional query parameters</span></span>
<span data-ttu-id="34526-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="34526-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="34526-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="34526-121">Request headers</span></span>
| <span data-ttu-id="34526-122">名前</span><span class="sxs-lookup"><span data-stu-id="34526-122">Name</span></span>      |<span data-ttu-id="34526-123">説明</span><span class="sxs-lookup"><span data-stu-id="34526-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="34526-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="34526-124">Authorization</span></span>  | <span data-ttu-id="34526-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="34526-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="34526-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="34526-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="34526-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="34526-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="34526-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="34526-130">Request body</span></span>
<span data-ttu-id="34526-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="34526-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="34526-132">応答</span><span class="sxs-lookup"><span data-stu-id="34526-132">Response</span></span>

<span data-ttu-id="34526-133">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [ChartTitle](../resources/charttitle.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="34526-133">If successful, this method returns a `200 OK` response code and [ChartTitle](../resources/charttitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="34526-134">例</span><span class="sxs-lookup"><span data-stu-id="34526-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="34526-135">要求</span><span class="sxs-lookup"><span data-stu-id="34526-135">Request</span></span>
<span data-ttu-id="34526-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="34526-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_charttitle"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/title
```
##### <a name="response"></a><span data-ttu-id="34526-137">応答</span><span class="sxs-lookup"><span data-stu-id="34526-137">Response</span></span>
<span data-ttu-id="34526-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="34526-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartTitle"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 64

{
  "overlay": true,
  "text": "text-value",
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get ChartTitle",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
