---
title: Update chartfont
description: chartfont オブジェクトのプロパティを更新します。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: b9a3a6e3fd29c551ef9b26e8c5d4ac939b0e5dea
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858073"
---
# <a name="update-chartfont"></a><span data-ttu-id="00ef5-103">Update chartfont</span><span class="sxs-lookup"><span data-stu-id="00ef5-103">Update chartfont</span></span>

<span data-ttu-id="00ef5-104">chartfont オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="00ef5-104">Update the properties of chartfont object.</span></span>
## <a name="permissions"></a><span data-ttu-id="00ef5-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="00ef5-105">Permissions</span></span>
<span data-ttu-id="00ef5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="00ef5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00ef5-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="00ef5-108">Permission type</span></span>      | <span data-ttu-id="00ef5-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="00ef5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="00ef5-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="00ef5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="00ef5-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="00ef5-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="00ef5-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="00ef5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00ef5-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="00ef5-113">Not supported.</span></span>    |
|<span data-ttu-id="00ef5-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="00ef5-114">Application</span></span> | <span data-ttu-id="00ef5-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="00ef5-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="00ef5-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="00ef5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/format/font
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/format/font
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/format/font
```
## <a name="optional-request-headers"></a><span data-ttu-id="00ef5-117">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="00ef5-117">Optional request headers</span></span>
| <span data-ttu-id="00ef5-118">名前</span><span class="sxs-lookup"><span data-stu-id="00ef5-118">Name</span></span>       | <span data-ttu-id="00ef5-119">説明</span><span class="sxs-lookup"><span data-stu-id="00ef5-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="00ef5-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="00ef5-120">Authorization</span></span>  | <span data-ttu-id="00ef5-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="00ef5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="00ef5-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="00ef5-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="00ef5-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="00ef5-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="00ef5-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="00ef5-126">Request body</span></span>
<span data-ttu-id="00ef5-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="00ef5-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="00ef5-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="00ef5-130">Property</span></span>     | <span data-ttu-id="00ef5-131">種類</span><span class="sxs-lookup"><span data-stu-id="00ef5-131">Type</span></span>   |<span data-ttu-id="00ef5-132">説明</span><span class="sxs-lookup"><span data-stu-id="00ef5-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="00ef5-133">bold</span><span class="sxs-lookup"><span data-stu-id="00ef5-133">bold</span></span>|<span data-ttu-id="00ef5-134">ブール値</span><span class="sxs-lookup"><span data-stu-id="00ef5-134">boolean</span></span>|<span data-ttu-id="00ef5-135">フォントの太字の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="00ef5-135">Represents the bold status of font.</span></span>|
|<span data-ttu-id="00ef5-136">color</span><span class="sxs-lookup"><span data-stu-id="00ef5-136">color</span></span>|<span data-ttu-id="00ef5-137">文字列</span><span class="sxs-lookup"><span data-stu-id="00ef5-137">string</span></span>|<span data-ttu-id="00ef5-p105">テキストの色の HTML カラー コード表記。たとえば、#FF0000 は赤を表します。</span><span class="sxs-lookup"><span data-stu-id="00ef5-p105">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="00ef5-141">italic</span><span class="sxs-lookup"><span data-stu-id="00ef5-141">italic</span></span>|<span data-ttu-id="00ef5-142">ブール値</span><span class="sxs-lookup"><span data-stu-id="00ef5-142">boolean</span></span>|<span data-ttu-id="00ef5-143">フォントの斜体の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="00ef5-143">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="00ef5-144">name</span><span class="sxs-lookup"><span data-stu-id="00ef5-144">name</span></span>|<span data-ttu-id="00ef5-145">文字列</span><span class="sxs-lookup"><span data-stu-id="00ef5-145">string</span></span>|<span data-ttu-id="00ef5-146">フォント名 (例: "Calibri")</span><span class="sxs-lookup"><span data-stu-id="00ef5-146">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="00ef5-147">size</span><span class="sxs-lookup"><span data-stu-id="00ef5-147">size</span></span>|<span data-ttu-id="00ef5-148">double</span><span class="sxs-lookup"><span data-stu-id="00ef5-148">double</span></span>|<span data-ttu-id="00ef5-149">フォント サイズ (例: 11)</span><span class="sxs-lookup"><span data-stu-id="00ef5-149">Size of the font (e.g. 11)</span></span>|
|<span data-ttu-id="00ef5-150">underline</span><span class="sxs-lookup"><span data-stu-id="00ef5-150">underline</span></span>|<span data-ttu-id="00ef5-151">文字列</span><span class="sxs-lookup"><span data-stu-id="00ef5-151">string</span></span>|<span data-ttu-id="00ef5-152">フォントに適用する下線の種類です。</span><span class="sxs-lookup"><span data-stu-id="00ef5-152">Type of underline applied to the font.</span></span> <span data-ttu-id="00ef5-153">可能な値: `None`、 `Single`。</span><span class="sxs-lookup"><span data-stu-id="00ef5-153">The possible values are: `None`, `Single`.</span></span>|

## <a name="response"></a><span data-ttu-id="00ef5-154">応答</span><span class="sxs-lookup"><span data-stu-id="00ef5-154">Response</span></span>

<span data-ttu-id="00ef5-155">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[WorkbookChartFont](../resources/chartfont.md)オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="00ef5-155">If successful, this method returns a `200 OK` response code and updated [WorkbookChartFont](../resources/chartfont.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="00ef5-156">例</span><span class="sxs-lookup"><span data-stu-id="00ef5-156">Example</span></span>
##### <a name="request"></a><span data-ttu-id="00ef5-157">要求</span><span class="sxs-lookup"><span data-stu-id="00ef5-157">Request</span></span>
<span data-ttu-id="00ef5-158">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="00ef5-158">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="00ef5-159">応答</span><span class="sxs-lookup"><span data-stu-id="00ef5-159">Response</span></span>
<span data-ttu-id="00ef5-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="00ef5-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
