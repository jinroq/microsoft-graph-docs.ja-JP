---
title: Update chartfont
description: chartfont オブジェクトのプロパティを更新します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 27b636394a28dca50b547ae0b16f92c52122c91b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36003547"
---
# <a name="update-chartfont"></a><span data-ttu-id="be9d9-103">Update chartfont</span><span class="sxs-lookup"><span data-stu-id="be9d9-103">Update chartfont</span></span>

<span data-ttu-id="be9d9-104">chartfont オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="be9d9-104">Update the properties of chartfont object.</span></span>
## <a name="permissions"></a><span data-ttu-id="be9d9-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="be9d9-105">Permissions</span></span>
<span data-ttu-id="be9d9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="be9d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be9d9-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="be9d9-108">Permission type</span></span>      | <span data-ttu-id="be9d9-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="be9d9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="be9d9-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="be9d9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="be9d9-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be9d9-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="be9d9-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="be9d9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be9d9-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="be9d9-113">Not supported.</span></span>    |
|<span data-ttu-id="be9d9-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="be9d9-114">Application</span></span> | <span data-ttu-id="be9d9-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="be9d9-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="be9d9-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="be9d9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/format/font
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/format/font
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/format/font
```
## <a name="optional-request-headers"></a><span data-ttu-id="be9d9-117">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="be9d9-117">Optional request headers</span></span>
| <span data-ttu-id="be9d9-118">名前</span><span class="sxs-lookup"><span data-stu-id="be9d9-118">Name</span></span>       | <span data-ttu-id="be9d9-119">説明</span><span class="sxs-lookup"><span data-stu-id="be9d9-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="be9d9-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="be9d9-120">Authorization</span></span>  | <span data-ttu-id="be9d9-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="be9d9-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="be9d9-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="be9d9-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="be9d9-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="be9d9-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="be9d9-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="be9d9-126">Request body</span></span>
<span data-ttu-id="be9d9-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="be9d9-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="be9d9-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="be9d9-130">Property</span></span>     | <span data-ttu-id="be9d9-131">型</span><span class="sxs-lookup"><span data-stu-id="be9d9-131">Type</span></span>   |<span data-ttu-id="be9d9-132">説明</span><span class="sxs-lookup"><span data-stu-id="be9d9-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="be9d9-133">bold</span><span class="sxs-lookup"><span data-stu-id="be9d9-133">bold</span></span>|<span data-ttu-id="be9d9-134">ブール値</span><span class="sxs-lookup"><span data-stu-id="be9d9-134">boolean</span></span>|<span data-ttu-id="be9d9-135">フォントの太字の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="be9d9-135">Represents the bold status of font.</span></span>|
|<span data-ttu-id="be9d9-136">color</span><span class="sxs-lookup"><span data-stu-id="be9d9-136">color</span></span>|<span data-ttu-id="be9d9-137">string</span><span class="sxs-lookup"><span data-stu-id="be9d9-137">string</span></span>|<span data-ttu-id="be9d9-p105">テキストの色の HTML カラー コード表記。たとえば、#FF0000 は赤を表します。</span><span class="sxs-lookup"><span data-stu-id="be9d9-p105">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="be9d9-141">italic</span><span class="sxs-lookup"><span data-stu-id="be9d9-141">italic</span></span>|<span data-ttu-id="be9d9-142">ブール値</span><span class="sxs-lookup"><span data-stu-id="be9d9-142">boolean</span></span>|<span data-ttu-id="be9d9-143">フォントの斜体の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="be9d9-143">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="be9d9-144">name</span><span class="sxs-lookup"><span data-stu-id="be9d9-144">name</span></span>|<span data-ttu-id="be9d9-145">string</span><span class="sxs-lookup"><span data-stu-id="be9d9-145">string</span></span>|<span data-ttu-id="be9d9-146">フォント名 (例: "Calibri")</span><span class="sxs-lookup"><span data-stu-id="be9d9-146">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="be9d9-147">size</span><span class="sxs-lookup"><span data-stu-id="be9d9-147">size</span></span>|<span data-ttu-id="be9d9-148">double</span><span class="sxs-lookup"><span data-stu-id="be9d9-148">double</span></span>|<span data-ttu-id="be9d9-149">フォント サイズ (例: 11)</span><span class="sxs-lookup"><span data-stu-id="be9d9-149">Size of the font (e.g. 11)</span></span>|
|<span data-ttu-id="be9d9-150">underline</span><span class="sxs-lookup"><span data-stu-id="be9d9-150">underline</span></span>|<span data-ttu-id="be9d9-151">文字列</span><span class="sxs-lookup"><span data-stu-id="be9d9-151">string</span></span>|<span data-ttu-id="be9d9-152">フォントに適用する下線の種類。</span><span class="sxs-lookup"><span data-stu-id="be9d9-152">Type of underline applied to the font.</span></span> <span data-ttu-id="be9d9-153">使用可能な値は`None`、 `Single`、です。</span><span class="sxs-lookup"><span data-stu-id="be9d9-153">The possible values are: `None`, `Single`.</span></span>|

## <a name="response"></a><span data-ttu-id="be9d9-154">応答</span><span class="sxs-lookup"><span data-stu-id="be9d9-154">Response</span></span>

<span data-ttu-id="be9d9-155">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で、更新された[WorkbookChartFont](../resources/chartfont.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="be9d9-155">If successful, this method returns a `200 OK` response code and updated [WorkbookChartFont](../resources/chartfont.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="be9d9-156">例</span><span class="sxs-lookup"><span data-stu-id="be9d9-156">Example</span></span>
##### <a name="request"></a><span data-ttu-id="be9d9-157">要求</span><span class="sxs-lookup"><span data-stu-id="be9d9-157">Request</span></span>
<span data-ttu-id="be9d9-158">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="be9d9-158">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="be9d9-159">プロトコル</span><span class="sxs-lookup"><span data-stu-id="be9d9-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_chartfont"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/format/font
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="be9d9-160">C#</span><span class="sxs-lookup"><span data-stu-id="be9d9-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-chartfont-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="be9d9-161">Javascript</span><span class="sxs-lookup"><span data-stu-id="be9d9-161">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-chartfont-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="be9d9-162">目的-C</span><span class="sxs-lookup"><span data-stu-id="be9d9-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-chartfont-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="be9d9-163">Java</span><span class="sxs-lookup"><span data-stu-id="be9d9-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-chartfont-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="be9d9-164">応答</span><span class="sxs-lookup"><span data-stu-id="be9d9-164">Response</span></span>
<span data-ttu-id="be9d9-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="be9d9-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartfont",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
