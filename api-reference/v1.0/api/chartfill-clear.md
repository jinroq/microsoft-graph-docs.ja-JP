---
title: 'ChartFill: clear'
description: グラフ要素の塗りつぶしの色をクリアします。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 30e56f09c3fa2a98ac8cef2177f0f568accb6e17
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27841532"
---
# <a name="chartfill-clear"></a><span data-ttu-id="d7f19-103">ChartFill: clear</span><span class="sxs-lookup"><span data-stu-id="d7f19-103">ChartFill: clear</span></span>

<span data-ttu-id="d7f19-104">グラフ要素の塗りつぶしの色をクリアします。</span><span class="sxs-lookup"><span data-stu-id="d7f19-104">Clear the fill color of a chart element.</span></span>
## <a name="permissions"></a><span data-ttu-id="d7f19-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d7f19-105">Permissions</span></span>
<span data-ttu-id="d7f19-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d7f19-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7f19-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d7f19-108">Permission type</span></span>      | <span data-ttu-id="d7f19-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d7f19-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d7f19-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d7f19-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d7f19-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d7f19-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d7f19-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d7f19-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7f19-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d7f19-113">Not supported.</span></span>    |
|<span data-ttu-id="d7f19-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d7f19-114">Application</span></span> | <span data-ttu-id="d7f19-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d7f19-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d7f19-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d7f19-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/format/fill/clear
POST /workbook/worksheets/{id|name}/charts/{name}/title/format/fill/clear
POST /workbook/worksheets/{id|name}/charts/{name}/legend/format/fill/clear

```
## <a name="request-headers"></a><span data-ttu-id="d7f19-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d7f19-117">Request headers</span></span>
| <span data-ttu-id="d7f19-118">名前</span><span class="sxs-lookup"><span data-stu-id="d7f19-118">Name</span></span>       | <span data-ttu-id="d7f19-119">説明</span><span class="sxs-lookup"><span data-stu-id="d7f19-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d7f19-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7f19-120">Authorization</span></span>  | <span data-ttu-id="d7f19-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d7f19-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d7f19-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d7f19-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="d7f19-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="d7f19-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7f19-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="d7f19-126">Request body</span></span>
<span data-ttu-id="d7f19-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d7f19-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d7f19-128">応答</span><span class="sxs-lookup"><span data-stu-id="d7f19-128">Response</span></span>

<span data-ttu-id="d7f19-p104">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="d7f19-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7f19-131">例</span><span class="sxs-lookup"><span data-stu-id="d7f19-131">Example</span></span>
<span data-ttu-id="d7f19-132">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="d7f19-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d7f19-133">要求</span><span class="sxs-lookup"><span data-stu-id="d7f19-133">Request</span></span>
<span data-ttu-id="d7f19-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d7f19-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartfill_clear"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/format/fill/clear
```

##### <a name="response"></a><span data-ttu-id="d7f19-135">応答</span><span class="sxs-lookup"><span data-stu-id="d7f19-135">Response</span></span>
<span data-ttu-id="d7f19-136">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="d7f19-136">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartFill: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
