---
title: NamedItem:Range
description: 名前に関連付けられている範囲オブジェクトを返します。名前付き項目の型が範囲でない場合、例外をスローします。
localization_priority: Normal
ms.openlocfilehash: d6ada5c4a5dce8c5a2ddb1510e69aba38f373134
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35276665"
---
# <a name="nameditem-range"></a><span data-ttu-id="aacd7-104">NamedItem:Range</span><span class="sxs-lookup"><span data-stu-id="aacd7-104">NamedItem: Range</span></span>

<span data-ttu-id="aacd7-p102">名前に関連付けられている範囲オブジェクトを返します。名前付き項目の型が範囲でない場合、例外をスローします。</span><span class="sxs-lookup"><span data-stu-id="aacd7-p102">Returns the range object that is associated with the name. Throws an exception if the named item's type is not a range.</span></span>
## <a name="permissions"></a><span data-ttu-id="aacd7-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="aacd7-107">Permissions</span></span>
<span data-ttu-id="aacd7-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="aacd7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aacd7-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="aacd7-110">Permission type</span></span>      | <span data-ttu-id="aacd7-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="aacd7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aacd7-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="aacd7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="aacd7-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aacd7-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="aacd7-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="aacd7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aacd7-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aacd7-115">Not supported.</span></span>    |
|<span data-ttu-id="aacd7-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="aacd7-116">Application</span></span> | <span data-ttu-id="aacd7-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aacd7-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="aacd7-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="aacd7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range

```
## <a name="request-headers"></a><span data-ttu-id="aacd7-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="aacd7-119">Request headers</span></span>
| <span data-ttu-id="aacd7-120">名前</span><span class="sxs-lookup"><span data-stu-id="aacd7-120">Name</span></span>       | <span data-ttu-id="aacd7-121">説明</span><span class="sxs-lookup"><span data-stu-id="aacd7-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="aacd7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="aacd7-122">Authorization</span></span>  | <span data-ttu-id="aacd7-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="aacd7-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="aacd7-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="aacd7-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="aacd7-p105">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="aacd7-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="aacd7-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="aacd7-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="aacd7-129">応答</span><span class="sxs-lookup"><span data-stu-id="aacd7-129">Response</span></span>

<span data-ttu-id="aacd7-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="aacd7-130">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aacd7-131">例</span><span class="sxs-lookup"><span data-stu-id="aacd7-131">Example</span></span>
<span data-ttu-id="aacd7-132">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="aacd7-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="aacd7-133">要求</span><span class="sxs-lookup"><span data-stu-id="aacd7-133">Request</span></span>
<span data-ttu-id="aacd7-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="aacd7-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "idempotent": true,
  "name": "nameditem_range"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range
```

##### <a name="response"></a><span data-ttu-id="aacd7-135">応答</span><span class="sxs-lookup"><span data-stu-id="aacd7-135">Response</span></span>
<span data-ttu-id="aacd7-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="aacd7-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="aacd7-139">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="aacd7-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="aacd7-140">C#</span><span class="sxs-lookup"><span data-stu-id="aacd7-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/nameditem_range-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="aacd7-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="aacd7-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/nameditem_range-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="aacd7-142">目的-C</span><span class="sxs-lookup"><span data-stu-id="aacd7-142">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/nameditem_range-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "NamedItem: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/nameditem-range.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/nameditem-range.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/nameditem-range.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
