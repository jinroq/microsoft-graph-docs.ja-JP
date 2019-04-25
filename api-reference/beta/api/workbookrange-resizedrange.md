---
title: 'workbookRange: resizedRange'
description: 現在の範囲オブジェクトに似た (ただし、右下隅がいくつかの行と列で拡張 (または縮小) されている) 範囲オブジェクトを取得します。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 667393920d936b0227affe178cb38f6bb54d49ac
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32536097"
---
# <a name="workbookrange-resizedrange"></a><span data-ttu-id="c4a3c-103">workbookRange: resizedRange</span><span class="sxs-lookup"><span data-stu-id="c4a3c-103">workbookRange: resizedRange</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4a3c-104">現在の範囲オブジェクトに似た (ただし、右下隅がいくつかの行と列で拡張 (または縮小) されている) 範囲オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="c4a3c-104">Gets a range object similar to the current range object, but with its bottom-right corner expanded (or contracted) by some number of rows and columns.</span></span>

## <a name="permissions"></a><span data-ttu-id="c4a3c-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c4a3c-105">Permissions</span></span>
<span data-ttu-id="c4a3c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c4a3c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4a3c-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c4a3c-108">Permission type</span></span>      | <span data-ttu-id="c4a3c-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c4a3c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c4a3c-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c4a3c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c4a3c-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c4a3c-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c4a3c-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c4a3c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4a3c-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c4a3c-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c4a3c-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c4a3c-114">Application</span></span> | <span data-ttu-id="c4a3c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c4a3c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c4a3c-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c4a3c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/resizedRange(deltaRows={n}, deltaColumns={n})

```

## <a name="function-parameters"></a><span data-ttu-id="c4a3c-117">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="c4a3c-117">Function parameters</span></span>

| <span data-ttu-id="c4a3c-118">パラメーター</span><span class="sxs-lookup"><span data-stu-id="c4a3c-118">Parameter</span></span>    | <span data-ttu-id="c4a3c-119">型</span><span class="sxs-lookup"><span data-stu-id="c4a3c-119">Type</span></span>   |<span data-ttu-id="c4a3c-120">説明</span><span class="sxs-lookup"><span data-stu-id="c4a3c-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c4a3c-121">deltaRows</span><span class="sxs-lookup"><span data-stu-id="c4a3c-121">deltarows</span></span>|<span data-ttu-id="c4a3c-122">Int32</span><span class="sxs-lookup"><span data-stu-id="c4a3c-122">Int32</span></span>|<span data-ttu-id="c4a3c-p102">現在の範囲を基準にして、右下隅を拡張する行の数です。範囲を拡張するには正の数値、または範囲を縮小するには負の数値を使用します</span><span class="sxs-lookup"><span data-stu-id="c4a3c-p102">The number of rows by which to expand the bottom-right corner, relative to the current range. Use a positive number to expand the range, or a negative number to decrease it</span></span>|
|<span data-ttu-id="c4a3c-125">deltaColumns</span><span class="sxs-lookup"><span data-stu-id="c4a3c-125">deltaColumns</span></span>|<span data-ttu-id="c4a3c-126">Int32</span><span class="sxs-lookup"><span data-stu-id="c4a3c-126">Int32</span></span>|<span data-ttu-id="c4a3c-p103">現在の範囲を基準にして、右下隅を拡張する列の数です。範囲を拡張するには正の数値、または範囲を縮小するには負の数値を使用します。</span><span class="sxs-lookup"><span data-stu-id="c4a3c-p103">The number of columnsby which to expand the bottom-right corner, relative to the current range. Use a positive number to expand the range, or a negative number to decrease it.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="c4a3c-129">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c4a3c-129">Request headers</span></span>
| <span data-ttu-id="c4a3c-130">名前</span><span class="sxs-lookup"><span data-stu-id="c4a3c-130">Name</span></span>       | <span data-ttu-id="c4a3c-131">説明</span><span class="sxs-lookup"><span data-stu-id="c4a3c-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c4a3c-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="c4a3c-132">Authorization</span></span>  | <span data-ttu-id="c4a3c-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c4a3c-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c4a3c-135">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c4a3c-135">Workbook-Session-Id</span></span>  | <span data-ttu-id="c4a3c-p105">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="c4a3c-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4a3c-138">要求本文</span><span class="sxs-lookup"><span data-stu-id="c4a3c-138">Request body</span></span>
<span data-ttu-id="c4a3c-139">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c4a3c-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c4a3c-140">応答</span><span class="sxs-lookup"><span data-stu-id="c4a3c-140">Response</span></span>

<span data-ttu-id="c4a3c-141">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [workbookRange](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c4a3c-141">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4a3c-142">例</span><span class="sxs-lookup"><span data-stu-id="c4a3c-142">Example</span></span>
<span data-ttu-id="c4a3c-143">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="c4a3c-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c4a3c-144">要求</span><span class="sxs-lookup"><span data-stu-id="c4a3c-144">Request</span></span>
<span data-ttu-id="c4a3c-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c4a3c-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_resizedrange"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range/resizedRange(deltarows={n}, deltaColumns={n})
```

##### <a name="response"></a><span data-ttu-id="c4a3c-146">応答</span><span class="sxs-lookup"><span data-stu-id="c4a3c-146">Response</span></span>
<span data-ttu-id="c4a3c-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c4a3c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 157

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnHidden": true,
  "columnIndex": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "workbookRange: resizedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/workbookrange-resizedrange.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
