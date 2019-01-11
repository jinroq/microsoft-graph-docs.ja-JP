---
title: '範囲: 削除'
description: 範囲に関連付けられているセルを削除します。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 1817a1c1481d86e08de4146215da6f6fc8de6a8c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871786"
---
# <a name="range-delete"></a><span data-ttu-id="5e0a1-103">範囲: 削除</span><span class="sxs-lookup"><span data-stu-id="5e0a1-103">Range: delete</span></span>

> <span data-ttu-id="5e0a1-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5e0a1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5e0a1-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5e0a1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5e0a1-106">範囲に関連付けられているセルを削除します。</span><span class="sxs-lookup"><span data-stu-id="5e0a1-106">Deletes the cells associated with the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="5e0a1-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5e0a1-107">Permissions</span></span>
<span data-ttu-id="5e0a1-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5e0a1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e0a1-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5e0a1-110">Permission type</span></span>      | <span data-ttu-id="5e0a1-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5e0a1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5e0a1-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5e0a1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5e0a1-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5e0a1-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5e0a1-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5e0a1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5e0a1-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5e0a1-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5e0a1-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5e0a1-116">Application</span></span> | <span data-ttu-id="5e0a1-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5e0a1-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5e0a1-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5e0a1-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/delete
POST /workbook/worksheets/{id|name}/range(address='<address>')/delete
POST /workbook/tables/{id|name}/columns/{id|name}/range/delete

```
## <a name="request-headers"></a><span data-ttu-id="5e0a1-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5e0a1-119">Request headers</span></span>
| <span data-ttu-id="5e0a1-120">名前</span><span class="sxs-lookup"><span data-stu-id="5e0a1-120">Name</span></span>       | <span data-ttu-id="5e0a1-121">説明</span><span class="sxs-lookup"><span data-stu-id="5e0a1-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5e0a1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5e0a1-122">Authorization</span></span>  | <span data-ttu-id="5e0a1-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5e0a1-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5e0a1-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="5e0a1-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="5e0a1-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="5e0a1-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e0a1-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="5e0a1-128">Request body</span></span>
<span data-ttu-id="5e0a1-129">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="5e0a1-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5e0a1-130">パラメーター</span><span class="sxs-lookup"><span data-stu-id="5e0a1-130">Parameter</span></span>    | <span data-ttu-id="5e0a1-131">Type</span><span class="sxs-lookup"><span data-stu-id="5e0a1-131">Type</span></span>   |<span data-ttu-id="5e0a1-132">説明</span><span class="sxs-lookup"><span data-stu-id="5e0a1-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e0a1-133"><legacyBold>Shift</legacyBold></span><span class="sxs-lookup"><span data-stu-id="5e0a1-133">shift</span></span>|<span data-ttu-id="5e0a1-134">文字列</span><span class="sxs-lookup"><span data-stu-id="5e0a1-134">string</span></span>|<span data-ttu-id="5e0a1-p105">セルをシフトする方向を指定します。可能な値は、`Up`、`Left` です。</span><span class="sxs-lookup"><span data-stu-id="5e0a1-p105">Specifies which way to shift the cells.  Possible values are: `Up`, `Left`.</span></span>|

## <a name="response"></a><span data-ttu-id="5e0a1-137">応答</span><span class="sxs-lookup"><span data-stu-id="5e0a1-137">Response</span></span>

<span data-ttu-id="5e0a1-p106">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="5e0a1-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e0a1-140">例</span><span class="sxs-lookup"><span data-stu-id="5e0a1-140">Example</span></span>
<span data-ttu-id="5e0a1-141">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="5e0a1-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5e0a1-142">要求</span><span class="sxs-lookup"><span data-stu-id="5e0a1-142">Request</span></span>
<span data-ttu-id="5e0a1-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5e0a1-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_delete"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/delete
Content-type: application/json
Content-length: 28

{
  "shift": "shift-value"
}
```

##### <a name="response"></a><span data-ttu-id="5e0a1-144">応答</span><span class="sxs-lookup"><span data-stu-id="5e0a1-144">Response</span></span>
<span data-ttu-id="5e0a1-145">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="5e0a1-145">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
