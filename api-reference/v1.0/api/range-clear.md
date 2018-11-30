---
title: '範囲: クリア'
description: 範囲の値、書式、塗りつぶし、罫線などをクリアします。
ms.openlocfilehash: c4a320827031eed62727ef464551cd410d71b610
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023267"
---
# <a name="range-clear"></a><span data-ttu-id="ed313-103">範囲: クリア</span><span class="sxs-lookup"><span data-stu-id="ed313-103">Range: clear</span></span>

<span data-ttu-id="ed313-104">範囲の値、書式、塗りつぶし、罫線などをクリアします。</span><span class="sxs-lookup"><span data-stu-id="ed313-104">Clear range values, format, fill, border, etc.</span></span>
## <a name="permissions"></a><span data-ttu-id="ed313-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ed313-105">Permissions</span></span>
<span data-ttu-id="ed313-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ed313-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed313-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ed313-108">Permission type</span></span>      | <span data-ttu-id="ed313-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ed313-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ed313-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ed313-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ed313-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ed313-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ed313-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ed313-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ed313-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ed313-113">Not supported.</span></span>    |
|<span data-ttu-id="ed313-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ed313-114">Application</span></span> | <span data-ttu-id="ed313-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ed313-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ed313-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ed313-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/clear
POST /workbook/worksheets/{id|name}/range(address='<address>')/clear
POST /workbook/tables/{id|name}/columns/{id|name}/range/clear

```
## <a name="request-headers"></a><span data-ttu-id="ed313-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ed313-117">Request headers</span></span>
| <span data-ttu-id="ed313-118">名前</span><span class="sxs-lookup"><span data-stu-id="ed313-118">Name</span></span>       | <span data-ttu-id="ed313-119">説明</span><span class="sxs-lookup"><span data-stu-id="ed313-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ed313-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed313-120">Authorization</span></span>  | <span data-ttu-id="ed313-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ed313-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ed313-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ed313-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="ed313-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="ed313-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed313-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="ed313-126">Request body</span></span>
<span data-ttu-id="ed313-127">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="ed313-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ed313-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="ed313-128">Parameter</span></span>    | <span data-ttu-id="ed313-129">型</span><span class="sxs-lookup"><span data-stu-id="ed313-129">Type</span></span>   |<span data-ttu-id="ed313-130">説明</span><span class="sxs-lookup"><span data-stu-id="ed313-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ed313-131">applyTo</span><span class="sxs-lookup"><span data-stu-id="ed313-131">applyTo</span></span>|<span data-ttu-id="ed313-132">文字列</span><span class="sxs-lookup"><span data-stu-id="ed313-132">string</span></span>|<span data-ttu-id="ed313-133">省略可能。</span><span class="sxs-lookup"><span data-stu-id="ed313-133">Optional.</span></span> <span data-ttu-id="ed313-134">クリア アクションの種類を決定します。</span><span class="sxs-lookup"><span data-stu-id="ed313-134">Determines the type of clear action.</span></span>  <span data-ttu-id="ed313-135">可能な値: `All`、 `Formats`、 `Contents`。</span><span class="sxs-lookup"><span data-stu-id="ed313-135">The possible values are: `All`, `Formats`, `Contents`.</span></span>|

## <a name="response"></a><span data-ttu-id="ed313-136">応答</span><span class="sxs-lookup"><span data-stu-id="ed313-136">Response</span></span>

<span data-ttu-id="ed313-p105">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="ed313-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed313-139">例</span><span class="sxs-lookup"><span data-stu-id="ed313-139">Example</span></span>
<span data-ttu-id="ed313-140">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="ed313-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ed313-141">要求</span><span class="sxs-lookup"><span data-stu-id="ed313-141">Request</span></span>
<span data-ttu-id="ed313-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ed313-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_clear"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/clear
Content-type: application/json
Content-length: 32

{
  "applyTo": "applyTo-value"
}
```

##### <a name="response"></a><span data-ttu-id="ed313-143">応答</span><span class="sxs-lookup"><span data-stu-id="ed313-143">Response</span></span>
<span data-ttu-id="ed313-144">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="ed313-144">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->