---
title: Update chartaxistitle
description: chartaxistitle オブジェクトのプロパティを更新します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: a38e768904539c011a44ebc8b242a86f22ce43fb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32580078"
---
# <a name="update-chartaxistitle"></a><span data-ttu-id="bb4bf-103">Update chartaxistitle</span><span class="sxs-lookup"><span data-stu-id="bb4bf-103">Update chartaxistitle</span></span>

<span data-ttu-id="bb4bf-104">chartaxistitle オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="bb4bf-104">Update the properties of chartaxistitle object.</span></span>
## <a name="permissions"></a><span data-ttu-id="bb4bf-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="bb4bf-105">Permissions</span></span>
<span data-ttu-id="bb4bf-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bb4bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb4bf-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bb4bf-108">Permission type</span></span>      | <span data-ttu-id="bb4bf-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="bb4bf-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bb4bf-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bb4bf-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bb4bf-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bb4bf-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bb4bf-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bb4bf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb4bf-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bb4bf-113">Not supported.</span></span>    |
|<span data-ttu-id="bb4bf-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bb4bf-114">Application</span></span> | <span data-ttu-id="bb4bf-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bb4bf-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bb4bf-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bb4bf-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/title
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/title
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/title
```
## <a name="optional-request-headers"></a><span data-ttu-id="bb4bf-117">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bb4bf-117">Optional request headers</span></span>
| <span data-ttu-id="bb4bf-118">名前</span><span class="sxs-lookup"><span data-stu-id="bb4bf-118">Name</span></span>       | <span data-ttu-id="bb4bf-119">説明</span><span class="sxs-lookup"><span data-stu-id="bb4bf-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="bb4bf-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb4bf-120">Authorization</span></span>  | <span data-ttu-id="bb4bf-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="bb4bf-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bb4bf-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="bb4bf-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="bb4bf-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="bb4bf-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb4bf-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="bb4bf-126">Request body</span></span>
<span data-ttu-id="bb4bf-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="bb4bf-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="bb4bf-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bb4bf-130">Property</span></span>     | <span data-ttu-id="bb4bf-131">型</span><span class="sxs-lookup"><span data-stu-id="bb4bf-131">Type</span></span>   |<span data-ttu-id="bb4bf-132">説明</span><span class="sxs-lookup"><span data-stu-id="bb4bf-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bb4bf-133">text</span><span class="sxs-lookup"><span data-stu-id="bb4bf-133">text</span></span>|<span data-ttu-id="bb4bf-134">string</span><span class="sxs-lookup"><span data-stu-id="bb4bf-134">string</span></span>|<span data-ttu-id="bb4bf-135">軸タイトルを表します。</span><span class="sxs-lookup"><span data-stu-id="bb4bf-135">Represents the axis title.</span></span>|
|<span data-ttu-id="bb4bf-136">visible</span><span class="sxs-lookup"><span data-stu-id="bb4bf-136">visible</span></span>|<span data-ttu-id="bb4bf-137">ブール値</span><span class="sxs-lookup"><span data-stu-id="bb4bf-137">boolean</span></span>|<span data-ttu-id="bb4bf-138">軸のタイトルの表示/非表示を指定するブール型の値です。</span><span class="sxs-lookup"><span data-stu-id="bb4bf-138">A boolean that specifies the visibility of an axis title.</span></span>|

## <a name="response"></a><span data-ttu-id="bb4bf-139">応答</span><span class="sxs-lookup"><span data-stu-id="bb4bf-139">Response</span></span>

<span data-ttu-id="bb4bf-140">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で、更新された[WorkbookChartAxisTitle](../resources/chartaxistitle.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="bb4bf-140">If successful, this method returns a `200 OK` response code and updated [WorkbookChartAxisTitle](../resources/chartaxistitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bb4bf-141">例</span><span class="sxs-lookup"><span data-stu-id="bb4bf-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bb4bf-142">要求</span><span class="sxs-lookup"><span data-stu-id="bb4bf-142">Request</span></span>
<span data-ttu-id="bb4bf-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bb4bf-143">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="bb4bf-144">応答</span><span class="sxs-lookup"><span data-stu-id="bb4bf-144">Response</span></span>
<span data-ttu-id="bb4bf-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bb4bf-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
