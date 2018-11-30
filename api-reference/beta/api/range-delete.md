---
title: '範囲: 削除'
description: 範囲に関連付けられているセルを削除します。
ms.openlocfilehash: eb0de43411145442b7ffb4b6b6ccf7af9b333520
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068062"
---
# <a name="range-delete"></a><span data-ttu-id="dcae9-103">範囲: 削除</span><span class="sxs-lookup"><span data-stu-id="dcae9-103">Range: delete</span></span>

> <span data-ttu-id="dcae9-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="dcae9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dcae9-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dcae9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dcae9-106">範囲に関連付けられているセルを削除します。</span><span class="sxs-lookup"><span data-stu-id="dcae9-106">Deletes the cells associated with the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="dcae9-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="dcae9-107">Permissions</span></span>
<span data-ttu-id="dcae9-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dcae9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dcae9-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="dcae9-110">Permission type</span></span>      | <span data-ttu-id="dcae9-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="dcae9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dcae9-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="dcae9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="dcae9-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dcae9-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="dcae9-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="dcae9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dcae9-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dcae9-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="dcae9-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="dcae9-116">Application</span></span> | <span data-ttu-id="dcae9-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dcae9-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dcae9-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="dcae9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/delete
POST /workbook/worksheets/{id|name}/range(address='<address>')/delete
POST /workbook/tables/{id|name}/columns/{id|name}/range/delete

```
## <a name="request-headers"></a><span data-ttu-id="dcae9-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dcae9-119">Request headers</span></span>
| <span data-ttu-id="dcae9-120">名前</span><span class="sxs-lookup"><span data-stu-id="dcae9-120">Name</span></span>       | <span data-ttu-id="dcae9-121">説明</span><span class="sxs-lookup"><span data-stu-id="dcae9-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="dcae9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="dcae9-122">Authorization</span></span>  | <span data-ttu-id="dcae9-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="dcae9-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dcae9-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="dcae9-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="dcae9-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="dcae9-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dcae9-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="dcae9-128">Request body</span></span>
<span data-ttu-id="dcae9-129">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="dcae9-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="dcae9-130">パラメーター</span><span class="sxs-lookup"><span data-stu-id="dcae9-130">Parameter</span></span>    | <span data-ttu-id="dcae9-131">型</span><span class="sxs-lookup"><span data-stu-id="dcae9-131">Type</span></span>   |<span data-ttu-id="dcae9-132">説明</span><span class="sxs-lookup"><span data-stu-id="dcae9-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dcae9-133"><legacyBold>Shift</legacyBold></span><span class="sxs-lookup"><span data-stu-id="dcae9-133">shift</span></span>|<span data-ttu-id="dcae9-134">文字列</span><span class="sxs-lookup"><span data-stu-id="dcae9-134">string</span></span>|<span data-ttu-id="dcae9-p105">セルをシフトする方向を指定します。可能な値は、`Up`、`Left` です。</span><span class="sxs-lookup"><span data-stu-id="dcae9-p105">Specifies which way to shift the cells.  Possible values are: `Up`, `Left`.</span></span>|

## <a name="response"></a><span data-ttu-id="dcae9-137">応答</span><span class="sxs-lookup"><span data-stu-id="dcae9-137">Response</span></span>

<span data-ttu-id="dcae9-p106">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="dcae9-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dcae9-140">例</span><span class="sxs-lookup"><span data-stu-id="dcae9-140">Example</span></span>
<span data-ttu-id="dcae9-141">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="dcae9-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="dcae9-142">要求</span><span class="sxs-lookup"><span data-stu-id="dcae9-142">Request</span></span>
<span data-ttu-id="dcae9-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="dcae9-143">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="dcae9-144">応答</span><span class="sxs-lookup"><span data-stu-id="dcae9-144">Response</span></span>
<span data-ttu-id="dcae9-145">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="dcae9-145">Here is an example of the response.</span></span> 
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