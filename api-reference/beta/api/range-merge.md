---
title: '範囲: マージ'
description: 範囲内のセルをワークシートの 1 つの領域にマージします。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 151163604bc7eada167daebdb325857cc6e87ce4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990524"
---
# <a name="range-merge"></a><span data-ttu-id="b7628-103">範囲: マージ</span><span class="sxs-lookup"><span data-stu-id="b7628-103">Range: merge</span></span>

> <span data-ttu-id="b7628-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b7628-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b7628-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b7628-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b7628-106">範囲内のセルをワークシートの 1 つの領域にマージします。</span><span class="sxs-lookup"><span data-stu-id="b7628-106">Merge the range cells into one region in the worksheet.</span></span>
## <a name="permissions"></a><span data-ttu-id="b7628-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b7628-107">Permissions</span></span>
<span data-ttu-id="b7628-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b7628-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7628-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b7628-110">Permission type</span></span>      | <span data-ttu-id="b7628-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b7628-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b7628-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b7628-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b7628-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b7628-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b7628-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b7628-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7628-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b7628-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b7628-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b7628-116">Application</span></span> | <span data-ttu-id="b7628-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b7628-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b7628-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b7628-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/merge
POST /workbook/worksheets/{id|name}/range(address='<address>')/merge
POST /workbook/tables/{id|name}/columns/{id|name}/range/merge

```
## <a name="request-headers"></a><span data-ttu-id="b7628-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b7628-119">Request headers</span></span>
| <span data-ttu-id="b7628-120">名前</span><span class="sxs-lookup"><span data-stu-id="b7628-120">Name</span></span>       | <span data-ttu-id="b7628-121">説明</span><span class="sxs-lookup"><span data-stu-id="b7628-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b7628-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b7628-122">Authorization</span></span>  | <span data-ttu-id="b7628-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b7628-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b7628-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="b7628-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="b7628-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="b7628-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7628-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="b7628-128">Request body</span></span>
<span data-ttu-id="b7628-129">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="b7628-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b7628-130">パラメーター</span><span class="sxs-lookup"><span data-stu-id="b7628-130">Parameter</span></span>    | <span data-ttu-id="b7628-131">Type</span><span class="sxs-lookup"><span data-stu-id="b7628-131">Type</span></span>   |<span data-ttu-id="b7628-132">説明</span><span class="sxs-lookup"><span data-stu-id="b7628-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b7628-133">across</span><span class="sxs-lookup"><span data-stu-id="b7628-133">across</span></span>|<span data-ttu-id="b7628-134">ブール値</span><span class="sxs-lookup"><span data-stu-id="b7628-134">boolean</span></span>|<span data-ttu-id="b7628-p105">省略可能。指定した範囲のセルを行ごとに結合して、行ごとに別のセルを作成する場合は True に設定します。既定値は False です。</span><span class="sxs-lookup"><span data-stu-id="b7628-p105">Optional. Set true to merge cells in each row of the specified range as separate merged cells. The default value is false.</span></span>|

## <a name="response"></a><span data-ttu-id="b7628-138">応答</span><span class="sxs-lookup"><span data-stu-id="b7628-138">Response</span></span>

<span data-ttu-id="b7628-p106">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="b7628-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7628-141">例</span><span class="sxs-lookup"><span data-stu-id="b7628-141">Example</span></span>
<span data-ttu-id="b7628-142">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="b7628-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b7628-143">要求</span><span class="sxs-lookup"><span data-stu-id="b7628-143">Request</span></span>
<span data-ttu-id="b7628-144">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b7628-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_merge"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/merge
Content-type: application/json
Content-length: 20

{
  "across": true
}
```

##### <a name="response"></a><span data-ttu-id="b7628-145">応答</span><span class="sxs-lookup"><span data-stu-id="b7628-145">Response</span></span>
<span data-ttu-id="b7628-146">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="b7628-146">Here is an example of the response.</span></span> 
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
  "description": "Range: merge",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
