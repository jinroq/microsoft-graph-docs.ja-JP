---
title: ワークシート:UsedRange
description: 使用範囲とは、値または書式設定が割り当たっているすべてのセルを包含する最小の範囲です。ワークシートが空白の場合、この関数は左上のセルを返します。
ms.openlocfilehash: 424d8226a8f109242956b139670ed674ae50b43d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067934"
---
# <a name="worksheet-usedrange"></a><span data-ttu-id="e79a2-104">ワークシート:UsedRange</span><span class="sxs-lookup"><span data-stu-id="e79a2-104">Worksheet: UsedRange</span></span>

<span data-ttu-id="e79a2-p102">使用範囲とは、値または書式設定が割り当たっているすべてのセルを包含する最小の範囲です。ワークシートが空白の場合、この関数は左上のセルを返します。</span><span class="sxs-lookup"><span data-stu-id="e79a2-p102">The used range is the smallest range that encompasses any cells that have a value or formatting assigned to them. If the worksheet is blank, this function will return the top left cell.</span></span>
## <a name="permissions"></a><span data-ttu-id="e79a2-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e79a2-107">Permissions</span></span>
<span data-ttu-id="e79a2-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e79a2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e79a2-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e79a2-110">Permission type</span></span>      | <span data-ttu-id="e79a2-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e79a2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e79a2-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e79a2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e79a2-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e79a2-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e79a2-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e79a2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e79a2-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e79a2-115">Not supported.</span></span>    |
|<span data-ttu-id="e79a2-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e79a2-116">Application</span></span> | <span data-ttu-id="e79a2-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e79a2-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e79a2-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e79a2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/UsedRange

```

## <a name="function-parameters"></a><span data-ttu-id="e79a2-119">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="e79a2-119">Function parameters</span></span>
<span data-ttu-id="e79a2-120">要求の URL では、オプションのクエリ パラメーターを提供します。</span><span class="sxs-lookup"><span data-stu-id="e79a2-120">In the request URL, provide an optional query parameter.</span></span>

| <span data-ttu-id="e79a2-121">パラメーター</span><span class="sxs-lookup"><span data-stu-id="e79a2-121">Parameter</span></span>    | <span data-ttu-id="e79a2-122">型</span><span class="sxs-lookup"><span data-stu-id="e79a2-122">Type</span></span>   |<span data-ttu-id="e79a2-123">説明</span><span class="sxs-lookup"><span data-stu-id="e79a2-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e79a2-124">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="e79a2-124">valuesOnly</span></span>|<span data-ttu-id="e79a2-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="e79a2-125">Boolean</span></span>|<span data-ttu-id="e79a2-p104">省略可能。値の入っているセルのみを使用セルと見なします (書式設定は無視されます)。</span><span class="sxs-lookup"><span data-stu-id="e79a2-p104">Optional. Considers only cells with values as used cells (ignores formatting).</span></span>|

## <a name="request-headers"></a><span data-ttu-id="e79a2-128">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e79a2-128">Request headers</span></span>
| <span data-ttu-id="e79a2-129">名前</span><span class="sxs-lookup"><span data-stu-id="e79a2-129">Name</span></span>       | <span data-ttu-id="e79a2-130">説明</span><span class="sxs-lookup"><span data-stu-id="e79a2-130">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e79a2-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="e79a2-131">Authorization</span></span>  | <span data-ttu-id="e79a2-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e79a2-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e79a2-134">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e79a2-134">Workbook-Session-Id</span></span>  | <span data-ttu-id="e79a2-p106">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="e79a2-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e79a2-137">要求本文</span><span class="sxs-lookup"><span data-stu-id="e79a2-137">Request body</span></span>
<span data-ttu-id="e79a2-138">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e79a2-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e79a2-139">応答</span><span class="sxs-lookup"><span data-stu-id="e79a2-139">Response</span></span>

<span data-ttu-id="e79a2-140">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e79a2-140">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e79a2-141">例</span><span class="sxs-lookup"><span data-stu-id="e79a2-141">Example</span></span>
<span data-ttu-id="e79a2-142">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="e79a2-142">Here is an example that shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e79a2-143">要求</span><span class="sxs-lookup"><span data-stu-id="e79a2-143">Request</span></span>
<span data-ttu-id="e79a2-144">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e79a2-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheet_usedrange"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/UsedRange(valuesOnly=true)
```

##### <a name="response"></a><span data-ttu-id="e79a2-145">応答</span><span class="sxs-lookup"><span data-stu-id="e79a2-145">Response</span></span>
<span data-ttu-id="e79a2-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e79a2-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
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