---
title: NamedItem:Range
description: 名前に関連付けられている範囲オブジェクトを返します。名前付き項目の型が範囲でない場合、例外をスローします。
localization_priority: Normal
ms.openlocfilehash: 93b00c813c84d7013f23d6dbe30cd86640b4e880
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851178"
---
# <a name="nameditem-range"></a><span data-ttu-id="74e79-104">NamedItem:Range</span><span class="sxs-lookup"><span data-stu-id="74e79-104">NamedItem: Range</span></span>

<span data-ttu-id="74e79-p102">名前に関連付けられている範囲オブジェクトを返します。名前付き項目の型が範囲でない場合、例外をスローします。</span><span class="sxs-lookup"><span data-stu-id="74e79-p102">Returns the range object that is associated with the name. Throws an exception if the named item's type is not a range.</span></span>
## <a name="permissions"></a><span data-ttu-id="74e79-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="74e79-107">Permissions</span></span>
<span data-ttu-id="74e79-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="74e79-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74e79-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="74e79-110">Permission type</span></span>      | <span data-ttu-id="74e79-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="74e79-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="74e79-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="74e79-112">Delegated (work or school account)</span></span> | <span data-ttu-id="74e79-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="74e79-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="74e79-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="74e79-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74e79-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="74e79-115">Not supported.</span></span>    |
|<span data-ttu-id="74e79-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="74e79-116">Application</span></span> | <span data-ttu-id="74e79-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="74e79-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="74e79-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="74e79-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range

```
## <a name="request-headers"></a><span data-ttu-id="74e79-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="74e79-119">Request headers</span></span>
| <span data-ttu-id="74e79-120">名前</span><span class="sxs-lookup"><span data-stu-id="74e79-120">Name</span></span>       | <span data-ttu-id="74e79-121">説明</span><span class="sxs-lookup"><span data-stu-id="74e79-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="74e79-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="74e79-122">Authorization</span></span>  | <span data-ttu-id="74e79-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="74e79-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="74e79-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="74e79-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="74e79-p105">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="74e79-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="74e79-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="74e79-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="74e79-129">応答</span><span class="sxs-lookup"><span data-stu-id="74e79-129">Response</span></span>

<span data-ttu-id="74e79-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="74e79-130">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74e79-131">例</span><span class="sxs-lookup"><span data-stu-id="74e79-131">Example</span></span>
<span data-ttu-id="74e79-132">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="74e79-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="74e79-133">要求</span><span class="sxs-lookup"><span data-stu-id="74e79-133">Request</span></span>
<span data-ttu-id="74e79-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="74e79-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "idempotent": true,
  "name": "nameditem_range"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range
```

##### <a name="response"></a><span data-ttu-id="74e79-135">応答</span><span class="sxs-lookup"><span data-stu-id="74e79-135">Response</span></span>
<span data-ttu-id="74e79-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="74e79-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "NamedItem: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
