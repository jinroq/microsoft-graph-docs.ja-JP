---
title: 範囲:UsedRange
description: 指定した範囲オブジェクトのうち使用されている範囲を返します。
ms.openlocfilehash: 26938b010a42e58b8bdc01687211c434514277de
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022721"
---
# <a name="range-usedrange"></a><span data-ttu-id="c56eb-103">範囲:UsedRange</span><span class="sxs-lookup"><span data-stu-id="c56eb-103">Range: UsedRange</span></span>

<span data-ttu-id="c56eb-104">指定した範囲オブジェクトのうち使用されている範囲を返します。</span><span class="sxs-lookup"><span data-stu-id="c56eb-104">Returns the used range of the given range object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c56eb-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c56eb-105">Permissions</span></span>
<span data-ttu-id="c56eb-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c56eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c56eb-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c56eb-108">Permission type</span></span>      | <span data-ttu-id="c56eb-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c56eb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c56eb-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c56eb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c56eb-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c56eb-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c56eb-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c56eb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c56eb-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c56eb-113">Not supported.</span></span>    |
|<span data-ttu-id="c56eb-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c56eb-114">Application</span></span> | <span data-ttu-id="c56eb-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c56eb-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c56eb-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c56eb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/usedRange
GET /workbook/worksheets/{id|name}/range(address='<address>')/usedRange
GET /workbook/tables/{id|name}/columns/{id|name}/range/usedRange

```
## <a name="request-headers"></a><span data-ttu-id="c56eb-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c56eb-117">Request headers</span></span>
| <span data-ttu-id="c56eb-118">名前</span><span class="sxs-lookup"><span data-stu-id="c56eb-118">Name</span></span>       | <span data-ttu-id="c56eb-119">説明</span><span class="sxs-lookup"><span data-stu-id="c56eb-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c56eb-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="c56eb-120">Authorization</span></span>  | <span data-ttu-id="c56eb-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c56eb-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c56eb-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c56eb-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="c56eb-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="c56eb-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="path-parameters"></a><span data-ttu-id="c56eb-126">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="c56eb-126">Path parameters</span></span>
| <span data-ttu-id="c56eb-127">パラメーター</span><span class="sxs-lookup"><span data-stu-id="c56eb-127">Parameter</span></span>    | <span data-ttu-id="c56eb-128">型</span><span class="sxs-lookup"><span data-stu-id="c56eb-128">Type</span></span>   |<span data-ttu-id="c56eb-129">説明</span><span class="sxs-lookup"><span data-stu-id="c56eb-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c56eb-130">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="c56eb-130">valuesOnly</span></span>|<span data-ttu-id="c56eb-131">ブール値</span><span class="sxs-lookup"><span data-stu-id="c56eb-131">boolean</span></span>|<span data-ttu-id="c56eb-p104">省略可能。値の入っているセルのみを使用セルと見なします。</span><span class="sxs-lookup"><span data-stu-id="c56eb-p104">Optional. Considers only cells with values as used cells.</span></span>|

## <a name="response"></a><span data-ttu-id="c56eb-134">応答</span><span class="sxs-lookup"><span data-stu-id="c56eb-134">Response</span></span>

<span data-ttu-id="c56eb-135">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c56eb-135">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c56eb-136">例</span><span class="sxs-lookup"><span data-stu-id="c56eb-136">Example</span></span>
<span data-ttu-id="c56eb-137">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="c56eb-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c56eb-138">要求</span><span class="sxs-lookup"><span data-stu-id="c56eb-138">Request</span></span>
<span data-ttu-id="c56eb-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c56eb-139">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_usedrange"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/usedRange
```

##### <a name="response"></a><span data-ttu-id="c56eb-140">応答</span><span class="sxs-lookup"><span data-stu-id="c56eb-140">Response</span></span>
<span data-ttu-id="c56eb-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c56eb-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<span data-ttu-id="c56eb-144">オプションを指定する例を次のとおりです`valuesOnly`のパラメーターです。</span><span class="sxs-lookup"><span data-stu-id="c56eb-144">Here is an example specifying the optional `valuesOnly` parameter.</span></span>

##### <a name="request"></a><span data-ttu-id="c56eb-145">要求</span><span class="sxs-lookup"><span data-stu-id="c56eb-145">Request</span></span>
<span data-ttu-id="c56eb-146">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c56eb-146">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_usedrange_valuesonly"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/usedRange(valuesOnly=true)
```

##### <a name="response"></a><span data-ttu-id="c56eb-147">応答</span><span class="sxs-lookup"><span data-stu-id="c56eb-147">Response</span></span>

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
  "cellCount": 90,
  "columnCount": 90,
  "columnIndex": 90,
  "valueTypes": "valueTypes-value"
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: UsedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->