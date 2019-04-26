---
title: Get ChartSeries
description: chartseries オブジェクトのプロパティと関係を取得します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: e0635400b553a9d7050f49c8be9eb899b5560f62
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33327602"
---
# <a name="get-chartseries"></a><span data-ttu-id="36ee4-103">Get ChartSeries</span><span class="sxs-lookup"><span data-stu-id="36ee4-103">Get ChartSeries</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36ee4-104">chartseries オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="36ee4-104">Retrieve the properties and relationships of chartseries object.</span></span>
## <a name="permissions"></a><span data-ttu-id="36ee4-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="36ee4-105">Permissions</span></span>
<span data-ttu-id="36ee4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="36ee4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36ee4-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="36ee4-108">Permission type</span></span>      | <span data-ttu-id="36ee4-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="36ee4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="36ee4-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="36ee4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="36ee4-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="36ee4-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="36ee4-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="36ee4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36ee4-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="36ee4-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="36ee4-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="36ee4-114">Application</span></span> | <span data-ttu-id="36ee4-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="36ee4-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="36ee4-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="36ee4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts/{name}/series/{undefined}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="36ee4-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="36ee4-117">Optional query parameters</span></span>
<span data-ttu-id="36ee4-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="36ee4-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="36ee4-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="36ee4-119">Request headers</span></span>
| <span data-ttu-id="36ee4-120">名前</span><span class="sxs-lookup"><span data-stu-id="36ee4-120">Name</span></span>      |<span data-ttu-id="36ee4-121">説明</span><span class="sxs-lookup"><span data-stu-id="36ee4-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="36ee4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="36ee4-122">Authorization</span></span>  | <span data-ttu-id="36ee4-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="36ee4-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="36ee4-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="36ee4-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="36ee4-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="36ee4-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="36ee4-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="36ee4-128">Request body</span></span>
<span data-ttu-id="36ee4-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="36ee4-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="36ee4-130">応答</span><span class="sxs-lookup"><span data-stu-id="36ee4-130">Response</span></span>

<span data-ttu-id="36ee4-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[workbookChartSeries](../resources/workbookchartseries.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="36ee4-131">If successful, this method returns a `200 OK` response code and [workbookChartSeries](../resources/workbookchartseries.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="36ee4-132">例</span><span class="sxs-lookup"><span data-stu-id="36ee4-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="36ee4-133">要求</span><span class="sxs-lookup"><span data-stu-id="36ee4-133">Request</span></span>
<span data-ttu-id="36ee4-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="36ee4-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_chartseries"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{undefined}
```
##### <a name="response"></a><span data-ttu-id="36ee4-135">応答</span><span class="sxs-lookup"><span data-stu-id="36ee4-135">Response</span></span>
<span data-ttu-id="36ee4-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="36ee4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartSeries"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get ChartSeries",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
