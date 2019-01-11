---
title: Update chartaxistitle
description: chartaxistitle オブジェクトのプロパティを更新します。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 692cf189c3eb4824c5b4dd9b56048434f4b3cfa1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836674"
---
# <a name="update-chartaxistitle"></a><span data-ttu-id="f1d43-103">Update chartaxistitle</span><span class="sxs-lookup"><span data-stu-id="f1d43-103">Update chartaxistitle</span></span>

<span data-ttu-id="f1d43-104">chartaxistitle オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f1d43-104">Update the properties of chartaxistitle object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f1d43-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f1d43-105">Permissions</span></span>
<span data-ttu-id="f1d43-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f1d43-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1d43-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f1d43-108">Permission type</span></span>      | <span data-ttu-id="f1d43-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f1d43-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f1d43-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f1d43-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f1d43-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f1d43-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f1d43-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f1d43-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1d43-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f1d43-113">Not supported.</span></span>    |
|<span data-ttu-id="f1d43-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f1d43-114">Application</span></span> | <span data-ttu-id="f1d43-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f1d43-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f1d43-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f1d43-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/title
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/title
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/title
```
## <a name="optional-request-headers"></a><span data-ttu-id="f1d43-117">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f1d43-117">Optional request headers</span></span>
| <span data-ttu-id="f1d43-118">名前</span><span class="sxs-lookup"><span data-stu-id="f1d43-118">Name</span></span>       | <span data-ttu-id="f1d43-119">説明</span><span class="sxs-lookup"><span data-stu-id="f1d43-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="f1d43-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1d43-120">Authorization</span></span>  | <span data-ttu-id="f1d43-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f1d43-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f1d43-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f1d43-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="f1d43-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="f1d43-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1d43-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="f1d43-126">Request body</span></span>
<span data-ttu-id="f1d43-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="f1d43-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f1d43-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f1d43-130">Property</span></span>     | <span data-ttu-id="f1d43-131">種類</span><span class="sxs-lookup"><span data-stu-id="f1d43-131">Type</span></span>   |<span data-ttu-id="f1d43-132">説明</span><span class="sxs-lookup"><span data-stu-id="f1d43-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f1d43-133">text</span><span class="sxs-lookup"><span data-stu-id="f1d43-133">text</span></span>|<span data-ttu-id="f1d43-134">文字列</span><span class="sxs-lookup"><span data-stu-id="f1d43-134">string</span></span>|<span data-ttu-id="f1d43-135">軸タイトルを表します。</span><span class="sxs-lookup"><span data-stu-id="f1d43-135">Represents the axis title.</span></span>|
|<span data-ttu-id="f1d43-136">visible</span><span class="sxs-lookup"><span data-stu-id="f1d43-136">visible</span></span>|<span data-ttu-id="f1d43-137">ブール値</span><span class="sxs-lookup"><span data-stu-id="f1d43-137">boolean</span></span>|<span data-ttu-id="f1d43-138">軸のタイトルの表示/非表示を指定するブール型の値です。</span><span class="sxs-lookup"><span data-stu-id="f1d43-138">A boolean that specifies the visibility of an axis title.</span></span>|

## <a name="response"></a><span data-ttu-id="f1d43-139">応答</span><span class="sxs-lookup"><span data-stu-id="f1d43-139">Response</span></span>

<span data-ttu-id="f1d43-140">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[WorkbookChartAxisTitle](../resources/chartaxistitle.md)オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="f1d43-140">If successful, this method returns a `200 OK` response code and updated [WorkbookChartAxisTitle](../resources/chartaxistitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f1d43-141">例</span><span class="sxs-lookup"><span data-stu-id="f1d43-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f1d43-142">要求</span><span class="sxs-lookup"><span data-stu-id="f1d43-142">Request</span></span>
<span data-ttu-id="f1d43-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f1d43-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartaxistitle"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/title
Content-type: application/json
Content-length: 45

{
  "text": "text-value",
  "visible": true
}
```
##### <a name="response"></a><span data-ttu-id="f1d43-144">応答</span><span class="sxs-lookup"><span data-stu-id="f1d43-144">Response</span></span>
<span data-ttu-id="f1d43-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f1d43-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartAxisTitle"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "text": "text-value",
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartaxistitle",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
