---
title: '範囲: クリア'
description: 範囲の値、書式、塗りつぶし、罫線などをクリアします。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: a32c21763c18371d3f0efe649b795135d4752b87
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991630"
---
# <a name="range-clear"></a><span data-ttu-id="92be1-103">範囲: クリア</span><span class="sxs-lookup"><span data-stu-id="92be1-103">Range: clear</span></span>

> <span data-ttu-id="92be1-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="92be1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="92be1-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="92be1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="92be1-106">範囲の値、書式、塗りつぶし、罫線などをクリアします。</span><span class="sxs-lookup"><span data-stu-id="92be1-106">Clear range values, format, fill, border, etc.</span></span>
## <a name="permissions"></a><span data-ttu-id="92be1-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="92be1-107">Permissions</span></span>
<span data-ttu-id="92be1-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="92be1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92be1-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="92be1-110">Permission type</span></span>      | <span data-ttu-id="92be1-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="92be1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="92be1-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="92be1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="92be1-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="92be1-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="92be1-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="92be1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="92be1-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="92be1-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="92be1-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="92be1-116">Application</span></span> | <span data-ttu-id="92be1-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="92be1-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="92be1-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="92be1-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/clear
POST /workbook/worksheets/{id|name}/range(address='<address>')/clear
POST /workbook/tables/{id|name}/columns/{id|name}/range/clear

```
## <a name="request-headers"></a><span data-ttu-id="92be1-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="92be1-119">Request headers</span></span>
| <span data-ttu-id="92be1-120">名前</span><span class="sxs-lookup"><span data-stu-id="92be1-120">Name</span></span>       | <span data-ttu-id="92be1-121">説明</span><span class="sxs-lookup"><span data-stu-id="92be1-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="92be1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="92be1-122">Authorization</span></span>  | <span data-ttu-id="92be1-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="92be1-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="92be1-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="92be1-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="92be1-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="92be1-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="92be1-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="92be1-128">Request body</span></span>
<span data-ttu-id="92be1-129">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="92be1-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="92be1-130">パラメーター</span><span class="sxs-lookup"><span data-stu-id="92be1-130">Parameter</span></span>    | <span data-ttu-id="92be1-131">Type</span><span class="sxs-lookup"><span data-stu-id="92be1-131">Type</span></span>   |<span data-ttu-id="92be1-132">説明</span><span class="sxs-lookup"><span data-stu-id="92be1-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="92be1-133">applyTo</span><span class="sxs-lookup"><span data-stu-id="92be1-133">applyTo</span></span>|<span data-ttu-id="92be1-134">文字列</span><span class="sxs-lookup"><span data-stu-id="92be1-134">string</span></span>|<span data-ttu-id="92be1-p105">省略可能。クリア操作の種類を決定します。可能な値は、`All`、`Formats`、`Contents` です。</span><span class="sxs-lookup"><span data-stu-id="92be1-p105">Optional. Determines the type of clear action.  Possible values are: `All`, `Formats`, `Contents`.</span></span>|

## <a name="response"></a><span data-ttu-id="92be1-138">応答</span><span class="sxs-lookup"><span data-stu-id="92be1-138">Response</span></span>

<span data-ttu-id="92be1-p106">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="92be1-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92be1-141">例</span><span class="sxs-lookup"><span data-stu-id="92be1-141">Example</span></span>
<span data-ttu-id="92be1-142">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="92be1-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="92be1-143">要求</span><span class="sxs-lookup"><span data-stu-id="92be1-143">Request</span></span>
<span data-ttu-id="92be1-144">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="92be1-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_clear"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/clear
Content-type: application/json
Content-length: 32

{
  "applyTo": "applyTo-value"
}
```

##### <a name="response"></a><span data-ttu-id="92be1-145">応答</span><span class="sxs-lookup"><span data-stu-id="92be1-145">Response</span></span>
<span data-ttu-id="92be1-146">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="92be1-146">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
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
