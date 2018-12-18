---
title: '範囲: マージ'
description: 範囲内のセルをワークシートの 1 つの領域にマージします。
author: lumine2008
ms.openlocfilehash: 87fc6fab83f1f03d40a1363277bfec511839bad6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27312776"
---
# <a name="range-merge"></a><span data-ttu-id="69d33-103">範囲: マージ</span><span class="sxs-lookup"><span data-stu-id="69d33-103">Range: merge</span></span>

<span data-ttu-id="69d33-104">範囲内のセルをワークシートの 1 つの領域にマージします。</span><span class="sxs-lookup"><span data-stu-id="69d33-104">Merge the range cells into one region in the worksheet.</span></span>
## <a name="permissions"></a><span data-ttu-id="69d33-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="69d33-105">Permissions</span></span>
<span data-ttu-id="69d33-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="69d33-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69d33-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="69d33-108">Permission type</span></span>      | <span data-ttu-id="69d33-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="69d33-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="69d33-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="69d33-110">Delegated (work or school account)</span></span> | <span data-ttu-id="69d33-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="69d33-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="69d33-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="69d33-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="69d33-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="69d33-113">Not supported.</span></span>    |
|<span data-ttu-id="69d33-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="69d33-114">Application</span></span> | <span data-ttu-id="69d33-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="69d33-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="69d33-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="69d33-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/merge
POST /workbook/worksheets/{id|name}/range(address='<address>')/merge
POST /workbook/tables/{id|name}/columns/{id|name}/range/merge

```
## <a name="request-headers"></a><span data-ttu-id="69d33-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="69d33-117">Request headers</span></span>
| <span data-ttu-id="69d33-118">名前</span><span class="sxs-lookup"><span data-stu-id="69d33-118">Name</span></span>       | <span data-ttu-id="69d33-119">説明</span><span class="sxs-lookup"><span data-stu-id="69d33-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="69d33-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="69d33-120">Authorization</span></span>  | <span data-ttu-id="69d33-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="69d33-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="69d33-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="69d33-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="69d33-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="69d33-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="69d33-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="69d33-126">Request body</span></span>
<span data-ttu-id="69d33-127">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="69d33-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="69d33-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="69d33-128">Parameter</span></span>    | <span data-ttu-id="69d33-129">種類</span><span class="sxs-lookup"><span data-stu-id="69d33-129">Type</span></span>   |<span data-ttu-id="69d33-130">説明</span><span class="sxs-lookup"><span data-stu-id="69d33-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="69d33-131">across</span><span class="sxs-lookup"><span data-stu-id="69d33-131">across</span></span>|<span data-ttu-id="69d33-132">ブール値</span><span class="sxs-lookup"><span data-stu-id="69d33-132">boolean</span></span>|<span data-ttu-id="69d33-p104">省略可能。指定した範囲のセルを行ごとに結合して、行ごとに別のセルを作成する場合は True に設定します。既定値は False です。</span><span class="sxs-lookup"><span data-stu-id="69d33-p104">Optional. Set true to merge cells in each row of the specified range as separate merged cells. The default value is false.</span></span>|

## <a name="response"></a><span data-ttu-id="69d33-136">応答</span><span class="sxs-lookup"><span data-stu-id="69d33-136">Response</span></span>

<span data-ttu-id="69d33-p105">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="69d33-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69d33-139">例</span><span class="sxs-lookup"><span data-stu-id="69d33-139">Example</span></span>
<span data-ttu-id="69d33-140">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="69d33-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="69d33-141">要求</span><span class="sxs-lookup"><span data-stu-id="69d33-141">Request</span></span>
<span data-ttu-id="69d33-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="69d33-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_merge"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/merge
Content-type: application/json
Content-length: 20

{
  "across": true
}
```

##### <a name="response"></a><span data-ttu-id="69d33-143">応答</span><span class="sxs-lookup"><span data-stu-id="69d33-143">Response</span></span>
<span data-ttu-id="69d33-144">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="69d33-144">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
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