---
title: ChartAxis を更新する
description: chartaxis オブジェクトのプロパティを更新します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 8016fc4496c520f7116f0db352a35df4ac356d8c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36361752"
---
# <a name="update-chartaxis"></a><span data-ttu-id="99bff-103">ChartAxis を更新する</span><span class="sxs-lookup"><span data-stu-id="99bff-103">Update chartaxis</span></span>

<span data-ttu-id="99bff-104">chartaxis オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="99bff-104">Update the properties of chartaxis object.</span></span>
## <a name="permissions"></a><span data-ttu-id="99bff-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="99bff-105">Permissions</span></span>
<span data-ttu-id="99bff-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="99bff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99bff-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="99bff-108">Permission type</span></span>      | <span data-ttu-id="99bff-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="99bff-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="99bff-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="99bff-110">Delegated (work or school account)</span></span> | <span data-ttu-id="99bff-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="99bff-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="99bff-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="99bff-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99bff-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="99bff-113">Not supported.</span></span>    |
|<span data-ttu-id="99bff-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="99bff-114">Application</span></span> | <span data-ttu-id="99bff-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="99bff-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="99bff-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="99bff-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis
```
## <a name="optional-request-headers"></a><span data-ttu-id="99bff-117">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="99bff-117">Optional request headers</span></span>
| <span data-ttu-id="99bff-118">名前</span><span class="sxs-lookup"><span data-stu-id="99bff-118">Name</span></span>       | <span data-ttu-id="99bff-119">説明</span><span class="sxs-lookup"><span data-stu-id="99bff-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="99bff-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="99bff-120">Authorization</span></span>  | <span data-ttu-id="99bff-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="99bff-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="99bff-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="99bff-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="99bff-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="99bff-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="99bff-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="99bff-126">Request body</span></span>
<span data-ttu-id="99bff-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="99bff-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="99bff-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="99bff-130">Property</span></span>     | <span data-ttu-id="99bff-131">型</span><span class="sxs-lookup"><span data-stu-id="99bff-131">Type</span></span>   |<span data-ttu-id="99bff-132">説明</span><span class="sxs-lookup"><span data-stu-id="99bff-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="99bff-133">majorUnit</span><span class="sxs-lookup"><span data-stu-id="99bff-133">majorUnit</span></span>|<span data-ttu-id="99bff-134">Json</span><span class="sxs-lookup"><span data-stu-id="99bff-134">Json</span></span>|<span data-ttu-id="99bff-p105">2 つの大きい目盛の間隔を表します。数値の値または空の文字列を設定できます。戻り値は常に数値です。</span><span class="sxs-lookup"><span data-stu-id="99bff-p105">Represents the interval between two major tick marks. Can be set to a numeric value or an empty string.  The returned value is always a number.</span></span>|
|<span data-ttu-id="99bff-138">maximum</span><span class="sxs-lookup"><span data-stu-id="99bff-138">maximum</span></span>|<span data-ttu-id="99bff-139">Json</span><span class="sxs-lookup"><span data-stu-id="99bff-139">Json</span></span>|<span data-ttu-id="99bff-p106">数値軸の最大値を表します。数値の値または空の文字列を設定できます (軸の値が自動の場合)。戻り値は常に数値です。</span><span class="sxs-lookup"><span data-stu-id="99bff-p106">Represents the maximum value on the value axis.  Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="99bff-143">minimum</span><span class="sxs-lookup"><span data-stu-id="99bff-143">minimum</span></span>|<span data-ttu-id="99bff-144">Json</span><span class="sxs-lookup"><span data-stu-id="99bff-144">Json</span></span>|<span data-ttu-id="99bff-p107">数値軸の最小値を表します。数値の値または空の文字列を設定できます (軸の値が自動の場合)。戻り値は常に数値です。</span><span class="sxs-lookup"><span data-stu-id="99bff-p107">Represents the minimum value on the value axis. Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="99bff-148">minorUnit</span><span class="sxs-lookup"><span data-stu-id="99bff-148">minorUnit</span></span>|<span data-ttu-id="99bff-149">Json</span><span class="sxs-lookup"><span data-stu-id="99bff-149">Json</span></span>|<span data-ttu-id="99bff-p108">2 つの小さい目盛の間隔を表します。"数値の値または空の文字列を設定できます (軸の値が自動の場合)。戻り値は常に数値です。</span><span class="sxs-lookup"><span data-stu-id="99bff-p108">Represents the interval between two minor tick marks. "Can be set to a numeric value or an empty string (for automatic axis values). The returned value is always a number.</span></span>|

## <a name="response"></a><span data-ttu-id="99bff-153">応答</span><span class="sxs-lookup"><span data-stu-id="99bff-153">Response</span></span>

<span data-ttu-id="99bff-154">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で、更新された[WorkbookChartAxis](../resources/chartaxis.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="99bff-154">If successful, this method returns a `200 OK` response code and updated [WorkbookChartAxis](../resources/chartaxis.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="99bff-155">例</span><span class="sxs-lookup"><span data-stu-id="99bff-155">Example</span></span>
##### <a name="request"></a><span data-ttu-id="99bff-156">要求</span><span class="sxs-lookup"><span data-stu-id="99bff-156">Request</span></span>
<span data-ttu-id="99bff-157">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="99bff-157">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="99bff-158">プロトコル</span><span class="sxs-lookup"><span data-stu-id="99bff-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_chartaxis"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis
Content-type: application/json
Content-length: 64

{
  "majorUnit": {
  },
  "maximum": {
  },
  "minimum": {
  }
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="99bff-159">C#</span><span class="sxs-lookup"><span data-stu-id="99bff-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-chartaxis-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="99bff-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="99bff-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-chartaxis-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="99bff-161">目的-C</span><span class="sxs-lookup"><span data-stu-id="99bff-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-chartaxis-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="99bff-162">Java</span><span class="sxs-lookup"><span data-stu-id="99bff-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-chartaxis-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="99bff-163">応答</span><span class="sxs-lookup"><span data-stu-id="99bff-163">Response</span></span>
<span data-ttu-id="99bff-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="99bff-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartAxis"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 64

{
  "majorUnit": {
  },
  "maximum": {
  },
  "minimum": {
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartaxis",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
