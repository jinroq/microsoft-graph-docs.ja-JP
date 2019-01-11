---
title: Update chartgridlines
description: chartgridlines オブジェクトのプロパティを更新します。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 6bba20f1bcf8a4cdccf56e7d390b5cf7c319fe97
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826062"
---
# <a name="update-chartgridlines"></a><span data-ttu-id="18150-103">Update chartgridlines</span><span class="sxs-lookup"><span data-stu-id="18150-103">Update chartgridlines</span></span>

<span data-ttu-id="18150-104">chartgridlines オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="18150-104">Update the properties of chartgridlines object.</span></span>
## <a name="permissions"></a><span data-ttu-id="18150-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="18150-105">Permissions</span></span>
<span data-ttu-id="18150-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="18150-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18150-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="18150-108">Permission type</span></span>      | <span data-ttu-id="18150-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="18150-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18150-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="18150-110">Delegated (work or school account)</span></span> | <span data-ttu-id="18150-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="18150-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="18150-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="18150-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18150-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="18150-113">Not supported.</span></span>    |
|<span data-ttu-id="18150-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="18150-114">Application</span></span> | <span data-ttu-id="18150-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="18150-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="18150-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="18150-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/minorGridlines
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/majorGridlines
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/majorGridlines
```
## <a name="request-headers"></a><span data-ttu-id="18150-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="18150-117">Request headers</span></span>
| <span data-ttu-id="18150-118">名前</span><span class="sxs-lookup"><span data-stu-id="18150-118">Name</span></span>       | <span data-ttu-id="18150-119">説明</span><span class="sxs-lookup"><span data-stu-id="18150-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="18150-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="18150-120">Authorization</span></span>  | <span data-ttu-id="18150-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="18150-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="18150-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="18150-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="18150-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="18150-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="18150-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="18150-126">Request body</span></span>
<span data-ttu-id="18150-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="18150-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="18150-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="18150-130">Property</span></span>     | <span data-ttu-id="18150-131">種類</span><span class="sxs-lookup"><span data-stu-id="18150-131">Type</span></span>   |<span data-ttu-id="18150-132">説明</span><span class="sxs-lookup"><span data-stu-id="18150-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="18150-133">visible</span><span class="sxs-lookup"><span data-stu-id="18150-133">visible</span></span>|<span data-ttu-id="18150-134">ブール値</span><span class="sxs-lookup"><span data-stu-id="18150-134">boolean</span></span>|<span data-ttu-id="18150-135">軸の目盛線を表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="18150-135">Boolean value representing if the axis gridlines are visible or not.</span></span>|

## <a name="response"></a><span data-ttu-id="18150-136">応答</span><span class="sxs-lookup"><span data-stu-id="18150-136">Response</span></span>

<span data-ttu-id="18150-137">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[WorkbookChartGridlines](../resources/chartgridlines.md)オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="18150-137">If successful, this method returns a `200 OK` response code and updated [WorkbookChartGridlines](../resources/chartgridlines.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="18150-138">例</span><span class="sxs-lookup"><span data-stu-id="18150-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="18150-139">要求</span><span class="sxs-lookup"><span data-stu-id="18150-139">Request</span></span>
<span data-ttu-id="18150-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="18150-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartgridlines"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/minorGridlines
Content-type: application/json
Content-length: 21

{
  "visible": true
}
```
##### <a name="response"></a><span data-ttu-id="18150-141">応答</span><span class="sxs-lookup"><span data-stu-id="18150-141">Response</span></span>
<span data-ttu-id="18150-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="18150-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartGridlines"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 21

{
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartgridlines",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
