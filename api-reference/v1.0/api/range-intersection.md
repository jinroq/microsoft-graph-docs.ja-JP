---
title: 範囲:Intersection
description: 指定した範囲の長方形の交差を表す範囲オブジェクトを取得します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 95e7af555c1ac857272994dc634ed0dc9f1b0fad
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951636"
---
# <a name="range-intersection"></a><span data-ttu-id="afc5a-103">範囲:Intersection</span><span class="sxs-lookup"><span data-stu-id="afc5a-103">Range: Intersection</span></span>

<span data-ttu-id="afc5a-104">指定した範囲の長方形の交差を表す範囲オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="afc5a-104">Gets the range object that represents the rectangular intersection of the given ranges.</span></span>
## <a name="permissions"></a><span data-ttu-id="afc5a-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="afc5a-105">Permissions</span></span>
<span data-ttu-id="afc5a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="afc5a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="afc5a-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="afc5a-108">Permission type</span></span>      | <span data-ttu-id="afc5a-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="afc5a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="afc5a-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="afc5a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="afc5a-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="afc5a-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="afc5a-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="afc5a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="afc5a-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="afc5a-113">Not supported.</span></span>    |
|<span data-ttu-id="afc5a-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="afc5a-114">Application</span></span> | <span data-ttu-id="afc5a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="afc5a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="afc5a-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="afc5a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/intersection
GET /workbook/worksheets/{id|name}/range(address='<address>')/intersection
GET /workbook/tables/{id|name}/columns/{id|name}/range/intersection

```
## <a name="request-headers"></a><span data-ttu-id="afc5a-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="afc5a-117">Request headers</span></span>
| <span data-ttu-id="afc5a-118">名前</span><span class="sxs-lookup"><span data-stu-id="afc5a-118">Name</span></span>       | <span data-ttu-id="afc5a-119">説明</span><span class="sxs-lookup"><span data-stu-id="afc5a-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="afc5a-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="afc5a-120">Authorization</span></span>  | <span data-ttu-id="afc5a-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="afc5a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="afc5a-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="afc5a-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="afc5a-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="afc5a-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="afc5a-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="afc5a-126">Request body</span></span>
<span data-ttu-id="afc5a-127">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="afc5a-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="afc5a-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="afc5a-128">Parameter</span></span>    | <span data-ttu-id="afc5a-129">Type</span><span class="sxs-lookup"><span data-stu-id="afc5a-129">Type</span></span>   |<span data-ttu-id="afc5a-130">説明</span><span class="sxs-lookup"><span data-stu-id="afc5a-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="afc5a-131">anotherRange</span><span class="sxs-lookup"><span data-stu-id="afc5a-131">anotherRange</span></span>|<span data-ttu-id="afc5a-132">文字列</span><span class="sxs-lookup"><span data-stu-id="afc5a-132">string</span></span>|<span data-ttu-id="afc5a-133">範囲の交差を判断するために使用される、Range オブジェクトまたは Range アドレス。</span><span class="sxs-lookup"><span data-stu-id="afc5a-133">The range object or range address that will be used to determine the intersection of ranges.</span></span>|

## <a name="response"></a><span data-ttu-id="afc5a-134">応答</span><span class="sxs-lookup"><span data-stu-id="afc5a-134">Response</span></span>

<span data-ttu-id="afc5a-135">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="afc5a-135">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="afc5a-136">例</span><span class="sxs-lookup"><span data-stu-id="afc5a-136">Example</span></span>
<span data-ttu-id="afc5a-137">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="afc5a-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="afc5a-138">要求</span><span class="sxs-lookup"><span data-stu-id="afc5a-138">Request</span></span>
<span data-ttu-id="afc5a-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="afc5a-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "isComposable": true,
  "name": "range_intersection"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/intersection
Content-type: application/json
Content-length: 42

{
  "anotherRange": "anotherRange-value"
}
```

##### <a name="response"></a><span data-ttu-id="afc5a-140">応答</span><span class="sxs-lookup"><span data-stu-id="afc5a-140">Response</span></span>
<span data-ttu-id="afc5a-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="afc5a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: Intersection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
