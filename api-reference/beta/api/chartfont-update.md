---
title: WorkbookChartFont の更新
description: WorkbookChartFont オブジェクトのプロパティを更新します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 4f42f2ef09743ba62e7462d696bd3259b9435289
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33635114"
---
# <a name="update-chartfont"></a><span data-ttu-id="54b02-103">Update chartfont</span><span class="sxs-lookup"><span data-stu-id="54b02-103">Update chartfont</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54b02-104">chartfont オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="54b02-104">Update the properties of chartfont object.</span></span>
## <a name="permissions"></a><span data-ttu-id="54b02-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="54b02-105">Permissions</span></span>
<span data-ttu-id="54b02-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="54b02-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54b02-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="54b02-108">Permission type</span></span>      | <span data-ttu-id="54b02-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="54b02-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="54b02-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="54b02-110">Delegated (work or school account)</span></span> | <span data-ttu-id="54b02-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="54b02-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="54b02-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="54b02-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="54b02-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="54b02-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="54b02-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="54b02-114">Application</span></span> | <span data-ttu-id="54b02-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="54b02-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="54b02-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="54b02-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/format/font
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/seriesaxis/format/font
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/format/font
```
## <a name="optional-request-headers"></a><span data-ttu-id="54b02-117">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="54b02-117">Optional request headers</span></span>
| <span data-ttu-id="54b02-118">名前</span><span class="sxs-lookup"><span data-stu-id="54b02-118">Name</span></span>       | <span data-ttu-id="54b02-119">説明</span><span class="sxs-lookup"><span data-stu-id="54b02-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="54b02-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="54b02-120">Authorization</span></span>  | <span data-ttu-id="54b02-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="54b02-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="54b02-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="54b02-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="54b02-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="54b02-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="54b02-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="54b02-126">Request body</span></span>
<span data-ttu-id="54b02-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="54b02-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="54b02-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="54b02-130">Property</span></span>     | <span data-ttu-id="54b02-131">型</span><span class="sxs-lookup"><span data-stu-id="54b02-131">Type</span></span>   |<span data-ttu-id="54b02-132">説明</span><span class="sxs-lookup"><span data-stu-id="54b02-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="54b02-133">bold</span><span class="sxs-lookup"><span data-stu-id="54b02-133">bold</span></span>|<span data-ttu-id="54b02-134">ブール値</span><span class="sxs-lookup"><span data-stu-id="54b02-134">boolean</span></span>|<span data-ttu-id="54b02-135">フォントの太字の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="54b02-135">Represents the bold status of font.</span></span>|
|<span data-ttu-id="54b02-136">color</span><span class="sxs-lookup"><span data-stu-id="54b02-136">color</span></span>|<span data-ttu-id="54b02-137">string</span><span class="sxs-lookup"><span data-stu-id="54b02-137">string</span></span>|<span data-ttu-id="54b02-p105">テキストの色の HTML カラー コード表記。たとえば、#FF0000 は赤を表します。</span><span class="sxs-lookup"><span data-stu-id="54b02-p105">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="54b02-141">italic</span><span class="sxs-lookup"><span data-stu-id="54b02-141">italic</span></span>|<span data-ttu-id="54b02-142">ブール値</span><span class="sxs-lookup"><span data-stu-id="54b02-142">boolean</span></span>|<span data-ttu-id="54b02-143">フォントの斜体の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="54b02-143">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="54b02-144">name</span><span class="sxs-lookup"><span data-stu-id="54b02-144">name</span></span>|<span data-ttu-id="54b02-145">string</span><span class="sxs-lookup"><span data-stu-id="54b02-145">string</span></span>|<span data-ttu-id="54b02-146">フォント名 (例: "Calibri")</span><span class="sxs-lookup"><span data-stu-id="54b02-146">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="54b02-147">size</span><span class="sxs-lookup"><span data-stu-id="54b02-147">size</span></span>|<span data-ttu-id="54b02-148">double</span><span class="sxs-lookup"><span data-stu-id="54b02-148">double</span></span>|<span data-ttu-id="54b02-149">フォント サイズ (例: 11)</span><span class="sxs-lookup"><span data-stu-id="54b02-149">Size of the font (e.g. 11)</span></span>|
|<span data-ttu-id="54b02-150">underline</span><span class="sxs-lookup"><span data-stu-id="54b02-150">underline</span></span>|<span data-ttu-id="54b02-151">文字列</span><span class="sxs-lookup"><span data-stu-id="54b02-151">string</span></span>|<span data-ttu-id="54b02-p106">フォントに適用する下線の種類。可能な値は、`None`、`Single` です。</span><span class="sxs-lookup"><span data-stu-id="54b02-p106">Type of underline applied to the font. Possible values are: `None`, `Single`.</span></span>|

## <a name="response"></a><span data-ttu-id="54b02-154">応答</span><span class="sxs-lookup"><span data-stu-id="54b02-154">Response</span></span>

<span data-ttu-id="54b02-155">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で、更新された[workbookChartFont](../resources/workbookchartfont.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="54b02-155">If successful, this method returns a `200 OK` response code and updated [workbookChartFont](../resources/workbookchartfont.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="54b02-156">例</span><span class="sxs-lookup"><span data-stu-id="54b02-156">Example</span></span>
##### <a name="request"></a><span data-ttu-id="54b02-157">要求</span><span class="sxs-lookup"><span data-stu-id="54b02-157">Request</span></span>
<span data-ttu-id="54b02-158">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="54b02-158">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartfont"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/format/font
Content-type: application/json
Content-length: 134

{
  "bold": true,
  "color": "color-value",
  "italic": true,
  "name": "name-value",
  "size": 99,
  "underline": "underline-value"
}
```
##### <a name="response"></a><span data-ttu-id="54b02-159">応答</span><span class="sxs-lookup"><span data-stu-id="54b02-159">Response</span></span>
<span data-ttu-id="54b02-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="54b02-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartFont"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 134

{
  "bold": true,
  "color": "color-value",
  "italic": true,
  "name": "name-value",
  "size": 99,
  "underline": "underline-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="54b02-163">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="54b02-163">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="54b02-164">Visual</span><span class="sxs-lookup"><span data-stu-id="54b02-164">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_chartfont-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="54b02-165">Java</span><span class="sxs-lookup"><span data-stu-id="54b02-165">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_chartfont-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update chartfont",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chartfont-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/chartfont-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
