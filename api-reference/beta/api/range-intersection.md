---
title: 範囲:Intersection
description: 指定した範囲の長方形の交差を表す範囲オブジェクトを取得します。
author: lumine2008
ms.openlocfilehash: 0ba9767c3c7d30ee5746b5a6723fd8103c1b8533
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344556"
---
# <a name="range-intersection"></a><span data-ttu-id="7d153-103">範囲:Intersection</span><span class="sxs-lookup"><span data-stu-id="7d153-103">Range: Intersection</span></span>

> <span data-ttu-id="7d153-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7d153-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7d153-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7d153-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7d153-106">指定した範囲の長方形の交差を表す範囲オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="7d153-106">Gets the range object that represents the rectangular intersection of the given ranges.</span></span>
## <a name="permissions"></a><span data-ttu-id="7d153-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7d153-107">Permissions</span></span>
<span data-ttu-id="7d153-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7d153-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d153-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7d153-110">Permission type</span></span>      | <span data-ttu-id="7d153-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7d153-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7d153-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7d153-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7d153-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7d153-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7d153-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7d153-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d153-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7d153-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7d153-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7d153-116">Application</span></span> | <span data-ttu-id="7d153-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7d153-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7d153-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7d153-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/Intersection
GET /workbook/worksheets/{id|name}/range(address='<address>')/Intersection
GET /workbook/tables/{id|name}/columns/{id|name}/range/Intersection

```
## <a name="request-headers"></a><span data-ttu-id="7d153-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7d153-119">Request headers</span></span>
| <span data-ttu-id="7d153-120">名前</span><span class="sxs-lookup"><span data-stu-id="7d153-120">Name</span></span>       | <span data-ttu-id="7d153-121">説明</span><span class="sxs-lookup"><span data-stu-id="7d153-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7d153-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7d153-122">Authorization</span></span>  | <span data-ttu-id="7d153-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7d153-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7d153-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7d153-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="7d153-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="7d153-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d153-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="7d153-128">Request body</span></span>
<span data-ttu-id="7d153-129">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="7d153-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7d153-130">パラメーター</span><span class="sxs-lookup"><span data-stu-id="7d153-130">Parameter</span></span>    | <span data-ttu-id="7d153-131">種類</span><span class="sxs-lookup"><span data-stu-id="7d153-131">Type</span></span>   |<span data-ttu-id="7d153-132">説明</span><span class="sxs-lookup"><span data-stu-id="7d153-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7d153-133">anotherRange</span><span class="sxs-lookup"><span data-stu-id="7d153-133">anotherRange</span></span>|<span data-ttu-id="7d153-134">string</span><span class="sxs-lookup"><span data-stu-id="7d153-134">string</span></span>|<span data-ttu-id="7d153-135">範囲の交差を判断するために使用される、Range オブジェクトまたは Range アドレス。</span><span class="sxs-lookup"><span data-stu-id="7d153-135">The range object or range address that will be used to determine the intersection of ranges.</span></span>|

## <a name="response"></a><span data-ttu-id="7d153-136">応答</span><span class="sxs-lookup"><span data-stu-id="7d153-136">Response</span></span>

<span data-ttu-id="7d153-137">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7d153-137">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d153-138">例</span><span class="sxs-lookup"><span data-stu-id="7d153-138">Example</span></span>
<span data-ttu-id="7d153-139">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="7d153-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7d153-140">要求</span><span class="sxs-lookup"><span data-stu-id="7d153-140">Request</span></span>
<span data-ttu-id="7d153-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7d153-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_intersection"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/Intersection
Content-type: application/json
Content-length: 42

{
  "anotherRange": "anotherRange-value"
}
```

##### <a name="response"></a><span data-ttu-id="7d153-142">応答</span><span class="sxs-lookup"><span data-stu-id="7d153-142">Response</span></span>
<span data-ttu-id="7d153-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7d153-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
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