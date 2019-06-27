---
title: WorkbookChartAxisTitle の更新
description: Workbookchartaxistitle オブジェクトのプロパティを更新します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 0d081bccd045fd387d076d1089ba3aee9aeb5eef
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35261832"
---
# <a name="update-workbookchartaxistitle"></a><span data-ttu-id="215cb-103">WorkbookChartAxisTitle の更新</span><span class="sxs-lookup"><span data-stu-id="215cb-103">Update workbookChartAxisTitle</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="215cb-104">WorkbookChartAxisTitle オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="215cb-104">Update the properties of workbookChartAxisTitle object.</span></span>
## <a name="permissions"></a><span data-ttu-id="215cb-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="215cb-105">Permissions</span></span>
<span data-ttu-id="215cb-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="215cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="215cb-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="215cb-108">Permission type</span></span>      | <span data-ttu-id="215cb-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="215cb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="215cb-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="215cb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="215cb-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="215cb-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="215cb-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="215cb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="215cb-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="215cb-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="215cb-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="215cb-114">Application</span></span> | <span data-ttu-id="215cb-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="215cb-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="215cb-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="215cb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/title
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/seriesaxis/title
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/title
```
## <a name="optional-request-headers"></a><span data-ttu-id="215cb-117">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="215cb-117">Optional request headers</span></span>
| <span data-ttu-id="215cb-118">名前</span><span class="sxs-lookup"><span data-stu-id="215cb-118">Name</span></span>       | <span data-ttu-id="215cb-119">説明</span><span class="sxs-lookup"><span data-stu-id="215cb-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="215cb-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="215cb-120">Authorization</span></span>  | <span data-ttu-id="215cb-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="215cb-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="215cb-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="215cb-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="215cb-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="215cb-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="215cb-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="215cb-126">Request body</span></span>
<span data-ttu-id="215cb-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="215cb-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="215cb-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="215cb-130">Property</span></span>     | <span data-ttu-id="215cb-131">型</span><span class="sxs-lookup"><span data-stu-id="215cb-131">Type</span></span>   |<span data-ttu-id="215cb-132">説明</span><span class="sxs-lookup"><span data-stu-id="215cb-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="215cb-133">text</span><span class="sxs-lookup"><span data-stu-id="215cb-133">text</span></span>|<span data-ttu-id="215cb-134">string</span><span class="sxs-lookup"><span data-stu-id="215cb-134">string</span></span>|<span data-ttu-id="215cb-135">軸タイトルを表します。</span><span class="sxs-lookup"><span data-stu-id="215cb-135">Represents the axis title.</span></span>|
|<span data-ttu-id="215cb-136">visible</span><span class="sxs-lookup"><span data-stu-id="215cb-136">visible</span></span>|<span data-ttu-id="215cb-137">ブール値</span><span class="sxs-lookup"><span data-stu-id="215cb-137">boolean</span></span>|<span data-ttu-id="215cb-138">軸のタイトルの表示/非表示を指定するブール型の値です。</span><span class="sxs-lookup"><span data-stu-id="215cb-138">A boolean that specifies the visibility of an axis title.</span></span>|

## <a name="response"></a><span data-ttu-id="215cb-139">応答</span><span class="sxs-lookup"><span data-stu-id="215cb-139">Response</span></span>

<span data-ttu-id="215cb-140">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で、更新された[workbookChartAxisTitle](../resources/workbookchartaxistitle.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="215cb-140">If successful, this method returns a `200 OK` response code and updated [workbookChartAxisTitle](../resources/workbookchartaxistitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="215cb-141">例</span><span class="sxs-lookup"><span data-stu-id="215cb-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="215cb-142">要求</span><span class="sxs-lookup"><span data-stu-id="215cb-142">Request</span></span>
<span data-ttu-id="215cb-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="215cb-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartaxistitle"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/title
Content-type: application/json
Content-length: 45

{
  "text": "text-value",
  "visible": true
}
```
##### <a name="response"></a><span data-ttu-id="215cb-144">応答</span><span class="sxs-lookup"><span data-stu-id="215cb-144">Response</span></span>
<span data-ttu-id="215cb-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="215cb-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="215cb-148">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="215cb-148">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="215cb-149">C#</span><span class="sxs-lookup"><span data-stu-id="215cb-149">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_chartaxistitle-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="215cb-150">Javascript</span><span class="sxs-lookup"><span data-stu-id="215cb-150">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_chartaxistitle-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="215cb-151">目的-C</span><span class="sxs-lookup"><span data-stu-id="215cb-151">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_chartaxistitle-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update chartaxistitle",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chartaxistitle-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/chartaxistitle-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/chartaxistitle-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
