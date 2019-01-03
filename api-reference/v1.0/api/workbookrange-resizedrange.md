---
title: 'workbookRange: resizedRange'
description: 現在の範囲オブジェクトに似た (ただし、右下隅がいくつかの行と列で拡張 (または縮小) されている) 範囲オブジェクトを取得します。
ms.openlocfilehash: 167aef7a1d7c975298b80d9e27aad7043b276b35
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021077"
---
# <a name="workbookrange-resizedrange"></a><span data-ttu-id="25ec3-103">workbookRange: resizedRange</span><span class="sxs-lookup"><span data-stu-id="25ec3-103">workbookRange: resizedRange</span></span>
<span data-ttu-id="25ec3-104">現在の範囲オブジェクトに似た (ただし、右下隅がいくつかの行と列で拡張 (または縮小) されている) 範囲オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="25ec3-104">Gets a range object similar to the current range object, but with its bottom-right corner expanded (or contracted) by some number of rows and columns.</span></span>

## <a name="permissions"></a><span data-ttu-id="25ec3-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="25ec3-105">Permissions</span></span>
<span data-ttu-id="25ec3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="25ec3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25ec3-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="25ec3-108">Permission type</span></span>      | <span data-ttu-id="25ec3-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="25ec3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="25ec3-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="25ec3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="25ec3-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="25ec3-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="25ec3-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="25ec3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="25ec3-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="25ec3-113">Not supported.</span></span>    |
|<span data-ttu-id="25ec3-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="25ec3-114">Application</span></span> | <span data-ttu-id="25ec3-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="25ec3-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="25ec3-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="25ec3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/resizedRange(deltaRows={n}, deltaColumns={n})

```

## <a name="function-parameters"></a><span data-ttu-id="25ec3-117">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="25ec3-117">Function parameters</span></span>

| <span data-ttu-id="25ec3-118">パラメーター</span><span class="sxs-lookup"><span data-stu-id="25ec3-118">Parameter</span></span>    | <span data-ttu-id="25ec3-119">型</span><span class="sxs-lookup"><span data-stu-id="25ec3-119">Type</span></span>   |<span data-ttu-id="25ec3-120">説明</span><span class="sxs-lookup"><span data-stu-id="25ec3-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="25ec3-121">deltaRows</span><span class="sxs-lookup"><span data-stu-id="25ec3-121">deltaRows</span></span>|<span data-ttu-id="25ec3-122">Int32</span><span class="sxs-lookup"><span data-stu-id="25ec3-122">Int32</span></span>|<span data-ttu-id="25ec3-p102">現在の範囲を基準にして、右下隅を拡張する行の数です。範囲を拡張するには正の数値、または範囲を縮小するには負の数値を使用します</span><span class="sxs-lookup"><span data-stu-id="25ec3-p102">The number of rows by which to expand the bottom-right corner, relative to the current range. Use a positive number to expand the range, or a negative number to decrease it</span></span>|
|<span data-ttu-id="25ec3-125">deltaColumns</span><span class="sxs-lookup"><span data-stu-id="25ec3-125">deltaColumns</span></span>|<span data-ttu-id="25ec3-126">Int32</span><span class="sxs-lookup"><span data-stu-id="25ec3-126">Int32</span></span>|<span data-ttu-id="25ec3-127">現在の範囲を基準にして、右下隅を拡張する列の数です。</span><span class="sxs-lookup"><span data-stu-id="25ec3-127">The number of columns by which to expand the bottom-right corner, relative to the current range.</span></span> <span data-ttu-id="25ec3-128">範囲を拡張するのには正の数または負の数を減らしてを使用します。</span><span class="sxs-lookup"><span data-stu-id="25ec3-128">Use a positive number to expand the range, or a negative number to decrease it.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="25ec3-129">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="25ec3-129">Request headers</span></span>
| <span data-ttu-id="25ec3-130">名前</span><span class="sxs-lookup"><span data-stu-id="25ec3-130">Name</span></span>       | <span data-ttu-id="25ec3-131">説明</span><span class="sxs-lookup"><span data-stu-id="25ec3-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="25ec3-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="25ec3-132">Authorization</span></span>  | <span data-ttu-id="25ec3-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="25ec3-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="25ec3-135">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="25ec3-135">Workbook-Session-Id</span></span>  | <span data-ttu-id="25ec3-p105">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="25ec3-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="25ec3-138">要求本文</span><span class="sxs-lookup"><span data-stu-id="25ec3-138">Request body</span></span>
<span data-ttu-id="25ec3-139">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="25ec3-139">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="25ec3-140">応答</span><span class="sxs-lookup"><span data-stu-id="25ec3-140">Response</span></span>
<span data-ttu-id="25ec3-141">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [workbookRange](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="25ec3-141">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="25ec3-142">例</span><span class="sxs-lookup"><span data-stu-id="25ec3-142">Example</span></span>
<span data-ttu-id="25ec3-143">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="25ec3-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="25ec3-144">要求</span><span class="sxs-lookup"><span data-stu-id="25ec3-144">Request</span></span>
<span data-ttu-id="25ec3-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="25ec3-145">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_resizedrange",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/resizedRange(deltaRows={n}, deltaColumns={n})
```

##### <a name="response"></a><span data-ttu-id="25ec3-146">応答</span><span class="sxs-lookup"><span data-stu-id="25ec3-146">Response</span></span>
<span data-ttu-id="25ec3-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="25ec3-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
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
<!-- {
  "type": "#page.annotation",
  "description": "workbookRange: resizedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->