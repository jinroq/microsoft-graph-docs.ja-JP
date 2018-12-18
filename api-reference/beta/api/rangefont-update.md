---
title: ｒangefont を更新する
description: rangefont オブジェクトのプロパティを更新します。
author: lumine2008
ms.openlocfilehash: 29cda6e2902f20c040ecc307755eed8fc58d25a8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350051"
---
# <a name="update-rangefont"></a><span data-ttu-id="2170a-103">ｒangefont を更新する</span><span class="sxs-lookup"><span data-stu-id="2170a-103">Update rangefont</span></span>

> <span data-ttu-id="2170a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2170a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2170a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2170a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2170a-106">rangefont オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="2170a-106">Update the properties of rangefont object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2170a-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2170a-107">Permissions</span></span>
<span data-ttu-id="2170a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2170a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2170a-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2170a-110">Permission type</span></span>      | <span data-ttu-id="2170a-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2170a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2170a-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2170a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2170a-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2170a-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2170a-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2170a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2170a-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2170a-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2170a-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2170a-116">Application</span></span> | <span data-ttu-id="2170a-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2170a-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2170a-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2170a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)/range/format/font
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format/font
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/font
```
## <a name="optional-request-headers"></a><span data-ttu-id="2170a-119">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2170a-119">Optional request headers</span></span>
| <span data-ttu-id="2170a-120">名前</span><span class="sxs-lookup"><span data-stu-id="2170a-120">Name</span></span>       | <span data-ttu-id="2170a-121">説明</span><span class="sxs-lookup"><span data-stu-id="2170a-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="2170a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2170a-122">Authorization</span></span>  | <span data-ttu-id="2170a-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2170a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2170a-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="2170a-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="2170a-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="2170a-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2170a-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="2170a-128">Request body</span></span>
<span data-ttu-id="2170a-p105">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="2170a-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="2170a-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2170a-132">Property</span></span>     | <span data-ttu-id="2170a-133">種類</span><span class="sxs-lookup"><span data-stu-id="2170a-133">Type</span></span>   |<span data-ttu-id="2170a-134">説明</span><span class="sxs-lookup"><span data-stu-id="2170a-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2170a-135">bold</span><span class="sxs-lookup"><span data-stu-id="2170a-135">bold</span></span>|<span data-ttu-id="2170a-136">ブール値</span><span class="sxs-lookup"><span data-stu-id="2170a-136">boolean</span></span>|<span data-ttu-id="2170a-137">フォントの太字の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="2170a-137">Represents the bold status of font.</span></span>|
|<span data-ttu-id="2170a-138">color</span><span class="sxs-lookup"><span data-stu-id="2170a-138">color</span></span>|<span data-ttu-id="2170a-139">文字列</span><span class="sxs-lookup"><span data-stu-id="2170a-139">string</span></span>|<span data-ttu-id="2170a-p106">テキストの色の HTML カラー コード表記。たとえば、#FF0000 は赤を表します。</span><span class="sxs-lookup"><span data-stu-id="2170a-p106">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="2170a-143">italic</span><span class="sxs-lookup"><span data-stu-id="2170a-143">italic</span></span>|<span data-ttu-id="2170a-144">ブール値</span><span class="sxs-lookup"><span data-stu-id="2170a-144">boolean</span></span>|<span data-ttu-id="2170a-145">フォントの斜体の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="2170a-145">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="2170a-146">name</span><span class="sxs-lookup"><span data-stu-id="2170a-146">name</span></span>|<span data-ttu-id="2170a-147">文字列</span><span class="sxs-lookup"><span data-stu-id="2170a-147">string</span></span>|<span data-ttu-id="2170a-148">フォント名 (例: "Calibri")</span><span class="sxs-lookup"><span data-stu-id="2170a-148">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="2170a-149">size</span><span class="sxs-lookup"><span data-stu-id="2170a-149">size</span></span>|<span data-ttu-id="2170a-150">double</span><span class="sxs-lookup"><span data-stu-id="2170a-150">double</span></span>|<span data-ttu-id="2170a-151">フォント サイズ</span><span class="sxs-lookup"><span data-stu-id="2170a-151">Font size.</span></span>|
|<span data-ttu-id="2170a-152">underline</span><span class="sxs-lookup"><span data-stu-id="2170a-152">underline</span></span>|<span data-ttu-id="2170a-153">文字列</span><span class="sxs-lookup"><span data-stu-id="2170a-153">string</span></span>|<span data-ttu-id="2170a-p107">フォントに適用する下線の種類。可能な値は、`None`、`Single`、`Double`、`SingleAccountant`、`DoubleAccountant` です。</span><span class="sxs-lookup"><span data-stu-id="2170a-p107">Type of underline applied to the font. Possible values are: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span></span>|

## <a name="response"></a><span data-ttu-id="2170a-156">応答</span><span class="sxs-lookup"><span data-stu-id="2170a-156">Response</span></span>

<span data-ttu-id="2170a-157">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された [RangeFont](../resources/rangefont.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2170a-157">If successful, this method returns a `200 OK` response code and updated [RangeFont](../resources/rangefont.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2170a-158">例</span><span class="sxs-lookup"><span data-stu-id="2170a-158">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2170a-159">要求</span><span class="sxs-lookup"><span data-stu-id="2170a-159">Request</span></span>
<span data-ttu-id="2170a-160">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2170a-160">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_rangefont"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/format/font
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
##### <a name="response"></a><span data-ttu-id="2170a-161">応答</span><span class="sxs-lookup"><span data-stu-id="2170a-161">Response</span></span>
<span data-ttu-id="2170a-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2170a-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFont"
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
  "description": "Update rangefont",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->