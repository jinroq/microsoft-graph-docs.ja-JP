---
title: '範囲: マージ'
description: 範囲内のセルをワークシートの 1 つの領域にマージします。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: ef2ace7b963402b2be3dfd92c11c27029aeeed3c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33337037"
---
# <a name="range-merge"></a><span data-ttu-id="999e7-103">範囲: マージ</span><span class="sxs-lookup"><span data-stu-id="999e7-103">Range: merge</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="999e7-104">範囲内のセルをワークシートの 1 つの領域にマージします。</span><span class="sxs-lookup"><span data-stu-id="999e7-104">Merge the range cells into one region in the worksheet.</span></span>
## <a name="permissions"></a><span data-ttu-id="999e7-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="999e7-105">Permissions</span></span>
<span data-ttu-id="999e7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="999e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="999e7-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="999e7-108">Permission type</span></span>      | <span data-ttu-id="999e7-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="999e7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="999e7-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="999e7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="999e7-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="999e7-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="999e7-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="999e7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="999e7-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="999e7-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="999e7-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="999e7-114">Application</span></span> | <span data-ttu-id="999e7-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="999e7-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="999e7-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="999e7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/merge
POST /workbook/worksheets/{id|name}/range(address='<address>')/merge
POST /workbook/tables/{id|name}/columns/{id|name}/range/merge

```
## <a name="request-headers"></a><span data-ttu-id="999e7-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="999e7-117">Request headers</span></span>
| <span data-ttu-id="999e7-118">名前</span><span class="sxs-lookup"><span data-stu-id="999e7-118">Name</span></span>       | <span data-ttu-id="999e7-119">説明</span><span class="sxs-lookup"><span data-stu-id="999e7-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="999e7-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="999e7-120">Authorization</span></span>  | <span data-ttu-id="999e7-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="999e7-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="999e7-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="999e7-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="999e7-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="999e7-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="999e7-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="999e7-126">Request body</span></span>
<span data-ttu-id="999e7-127">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="999e7-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="999e7-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="999e7-128">Parameter</span></span>    | <span data-ttu-id="999e7-129">型</span><span class="sxs-lookup"><span data-stu-id="999e7-129">Type</span></span>   |<span data-ttu-id="999e7-130">説明</span><span class="sxs-lookup"><span data-stu-id="999e7-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="999e7-131">across</span><span class="sxs-lookup"><span data-stu-id="999e7-131">across</span></span>|<span data-ttu-id="999e7-132">ブール値</span><span class="sxs-lookup"><span data-stu-id="999e7-132">boolean</span></span>|<span data-ttu-id="999e7-p104">省略可能。指定した範囲のセルを行ごとに結合して、行ごとに別のセルを作成する場合は True に設定します。既定値は False です。</span><span class="sxs-lookup"><span data-stu-id="999e7-p104">Optional. Set true to merge cells in each row of the specified range as separate merged cells. The default value is false.</span></span>|

## <a name="response"></a><span data-ttu-id="999e7-136">応答</span><span class="sxs-lookup"><span data-stu-id="999e7-136">Response</span></span>

<span data-ttu-id="999e7-p105">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="999e7-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="999e7-139">例</span><span class="sxs-lookup"><span data-stu-id="999e7-139">Example</span></span>
<span data-ttu-id="999e7-140">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="999e7-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="999e7-141">要求</span><span class="sxs-lookup"><span data-stu-id="999e7-141">Request</span></span>
<span data-ttu-id="999e7-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="999e7-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_merge"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/merge
Content-type: application/json
Content-length: 20

{
  "across": true
}
```

##### <a name="response"></a><span data-ttu-id="999e7-143">応答</span><span class="sxs-lookup"><span data-stu-id="999e7-143">Response</span></span>
<span data-ttu-id="999e7-144">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="999e7-144">Here is an example of the response.</span></span> 
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
<!--
{
  "type": "#page.annotation",
  "description": "Range: merge",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
