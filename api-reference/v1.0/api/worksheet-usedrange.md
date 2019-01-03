---
title: ワークシート:UsedRange
description: 使用範囲とは、値または書式設定が割り当たっているすべてのセルを包含する最小の範囲です。ワークシートが空白の場合、この関数は左上のセルを返します。
ms.openlocfilehash: 6da0ad6ab5fe71491d30eac1e95255d39ba37a18
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020668"
---
# <a name="worksheet-usedrange"></a><span data-ttu-id="ad4db-104">ワークシート:UsedRange</span><span class="sxs-lookup"><span data-stu-id="ad4db-104">Worksheet: UsedRange</span></span>

<span data-ttu-id="ad4db-p102">使用範囲とは、値または書式設定が割り当たっているすべてのセルを包含する最小の範囲です。ワークシートが空白の場合、この関数は左上のセルを返します。</span><span class="sxs-lookup"><span data-stu-id="ad4db-p102">The used range is the smallest range that encompasses any cells that have a value or formatting assigned to them. If the worksheet is blank, this function will return the top left cell.</span></span>
## <a name="permissions"></a><span data-ttu-id="ad4db-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ad4db-107">Permissions</span></span>
<span data-ttu-id="ad4db-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ad4db-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad4db-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ad4db-110">Permission type</span></span>      | <span data-ttu-id="ad4db-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ad4db-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ad4db-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ad4db-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ad4db-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ad4db-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ad4db-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ad4db-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad4db-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ad4db-115">Not supported.</span></span>    |
|<span data-ttu-id="ad4db-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ad4db-116">Application</span></span> | <span data-ttu-id="ad4db-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ad4db-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ad4db-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ad4db-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/usedRange

```

## <a name="function-parameters"></a><span data-ttu-id="ad4db-119">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="ad4db-119">Function parameters</span></span>
<span data-ttu-id="ad4db-120">要求 URL で省略可能なパラメーターを提供することがあります。</span><span class="sxs-lookup"><span data-stu-id="ad4db-120">In the request URL you may provide optional parameters.</span></span>

| <span data-ttu-id="ad4db-121">パラメーター</span><span class="sxs-lookup"><span data-stu-id="ad4db-121">Parameter</span></span>    | <span data-ttu-id="ad4db-122">型</span><span class="sxs-lookup"><span data-stu-id="ad4db-122">Type</span></span>   |<span data-ttu-id="ad4db-123">説明</span><span class="sxs-lookup"><span data-stu-id="ad4db-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ad4db-124">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="ad4db-124">valuesOnly</span></span>|<span data-ttu-id="ad4db-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad4db-125">Boolean</span></span>|<span data-ttu-id="ad4db-p104">省略可能。値の入っているセルのみを使用セルと見なします (書式設定は無視されます)。</span><span class="sxs-lookup"><span data-stu-id="ad4db-p104">Optional. Considers only cells with values as used cells (ignores formatting).</span></span>|

## <a name="request-headers"></a><span data-ttu-id="ad4db-128">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ad4db-128">Request headers</span></span>
| <span data-ttu-id="ad4db-129">名前</span><span class="sxs-lookup"><span data-stu-id="ad4db-129">Name</span></span>       | <span data-ttu-id="ad4db-130">説明</span><span class="sxs-lookup"><span data-stu-id="ad4db-130">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ad4db-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad4db-131">Authorization</span></span>  | <span data-ttu-id="ad4db-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ad4db-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ad4db-134">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ad4db-134">Workbook-Session-Id</span></span>  | <span data-ttu-id="ad4db-p106">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="ad4db-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad4db-137">要求本文</span><span class="sxs-lookup"><span data-stu-id="ad4db-137">Request body</span></span>
<span data-ttu-id="ad4db-138">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ad4db-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ad4db-139">応答</span><span class="sxs-lookup"><span data-stu-id="ad4db-139">Response</span></span>

<span data-ttu-id="ad4db-140">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ad4db-140">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad4db-141">例</span><span class="sxs-lookup"><span data-stu-id="ad4db-141">Example</span></span>
<span data-ttu-id="ad4db-142">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="ad4db-142">Here is an example that shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="ad4db-143">要求</span><span class="sxs-lookup"><span data-stu-id="ad4db-143">Request</span></span>
<span data-ttu-id="ad4db-144">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ad4db-144">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "worksheet_usedrange"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/usedRange
```

##### <a name="response"></a><span data-ttu-id="ad4db-145">応答</span><span class="sxs-lookup"><span data-stu-id="ad4db-145">Response</span></span>
<span data-ttu-id="ad4db-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ad4db-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "addressLocal": "addressLocal-value"
}
```

<span data-ttu-id="ad4db-149">オプションの代わりに、この関数を呼び出すことができます`valuesOnly`パラメーター。</span><span class="sxs-lookup"><span data-stu-id="ad4db-149">Alternatively, this function can be called with the optional `valuesOnly` parameter.</span></span>

##### <a name="request"></a><span data-ttu-id="ad4db-150">要求</span><span class="sxs-lookup"><span data-stu-id="ad4db-150">Request</span></span>
<span data-ttu-id="ad4db-151">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ad4db-151">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "worksheet_usedrange_valuesonly"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/usedRange(valuesOnly=true)
```

##### <a name="response"></a><span data-ttu-id="ad4db-152">応答</span><span class="sxs-lookup"><span data-stu-id="ad4db-152">Response</span></span>
<span data-ttu-id="ad4db-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ad4db-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "addressLocal": "addressLocal-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Worksheet: UsedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->