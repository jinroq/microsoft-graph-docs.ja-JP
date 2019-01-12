---
title: '範囲: 削除'
description: 範囲に関連付けられているセルを削除します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 2a3ea63884964f1c1eb2b423c459fcae3ba6bfb1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931343"
---
# <a name="range-delete"></a><span data-ttu-id="7d6aa-103">範囲: 削除</span><span class="sxs-lookup"><span data-stu-id="7d6aa-103">Range: delete</span></span>

> <span data-ttu-id="7d6aa-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7d6aa-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7d6aa-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7d6aa-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7d6aa-106">範囲に関連付けられているセルを削除します。</span><span class="sxs-lookup"><span data-stu-id="7d6aa-106">Deletes the cells associated with the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="7d6aa-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7d6aa-107">Permissions</span></span>
<span data-ttu-id="7d6aa-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7d6aa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d6aa-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7d6aa-110">Permission type</span></span>      | <span data-ttu-id="7d6aa-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7d6aa-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7d6aa-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7d6aa-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7d6aa-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7d6aa-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7d6aa-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7d6aa-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d6aa-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7d6aa-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7d6aa-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7d6aa-116">Application</span></span> | <span data-ttu-id="7d6aa-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7d6aa-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7d6aa-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7d6aa-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/delete
POST /workbook/worksheets/{id|name}/range(address='<address>')/delete
POST /workbook/tables/{id|name}/columns/{id|name}/range/delete

```
## <a name="request-headers"></a><span data-ttu-id="7d6aa-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7d6aa-119">Request headers</span></span>
| <span data-ttu-id="7d6aa-120">名前</span><span class="sxs-lookup"><span data-stu-id="7d6aa-120">Name</span></span>       | <span data-ttu-id="7d6aa-121">説明</span><span class="sxs-lookup"><span data-stu-id="7d6aa-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7d6aa-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7d6aa-122">Authorization</span></span>  | <span data-ttu-id="7d6aa-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7d6aa-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7d6aa-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7d6aa-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="7d6aa-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="7d6aa-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d6aa-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="7d6aa-128">Request body</span></span>
<span data-ttu-id="7d6aa-129">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="7d6aa-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7d6aa-130">パラメーター</span><span class="sxs-lookup"><span data-stu-id="7d6aa-130">Parameter</span></span>    | <span data-ttu-id="7d6aa-131">Type</span><span class="sxs-lookup"><span data-stu-id="7d6aa-131">Type</span></span>   |<span data-ttu-id="7d6aa-132">説明</span><span class="sxs-lookup"><span data-stu-id="7d6aa-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7d6aa-133"><legacyBold>Shift</legacyBold></span><span class="sxs-lookup"><span data-stu-id="7d6aa-133">shift</span></span>|<span data-ttu-id="7d6aa-134">文字列</span><span class="sxs-lookup"><span data-stu-id="7d6aa-134">string</span></span>|<span data-ttu-id="7d6aa-p105">セルをシフトする方向を指定します。可能な値は、`Up`、`Left` です。</span><span class="sxs-lookup"><span data-stu-id="7d6aa-p105">Specifies which way to shift the cells.  Possible values are: `Up`, `Left`.</span></span>|

## <a name="response"></a><span data-ttu-id="7d6aa-137">応答</span><span class="sxs-lookup"><span data-stu-id="7d6aa-137">Response</span></span>

<span data-ttu-id="7d6aa-p106">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="7d6aa-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d6aa-140">例</span><span class="sxs-lookup"><span data-stu-id="7d6aa-140">Example</span></span>
<span data-ttu-id="7d6aa-141">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="7d6aa-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7d6aa-142">要求</span><span class="sxs-lookup"><span data-stu-id="7d6aa-142">Request</span></span>
<span data-ttu-id="7d6aa-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7d6aa-143">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="7d6aa-144">応答</span><span class="sxs-lookup"><span data-stu-id="7d6aa-144">Response</span></span>
<span data-ttu-id="7d6aa-145">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="7d6aa-145">Here is an example of the response.</span></span> 
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
