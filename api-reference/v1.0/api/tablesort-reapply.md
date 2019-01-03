---
title: 'TableSort: reapply　'
description: テーブルに、現在の並べ替えパラメーターを再適用します。
author: lumine2008
ms.openlocfilehash: 4ce369ed95d8940a34b02f6e406042123529cf5e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306861"
---
# <a name="tablesort-reapply"></a><span data-ttu-id="0cd1d-103">TableSort: reapply　</span><span class="sxs-lookup"><span data-stu-id="0cd1d-103">TableSort: reapply</span></span>

<span data-ttu-id="0cd1d-104">テーブルに、現在の並べ替えパラメーターを再適用します。</span><span class="sxs-lookup"><span data-stu-id="0cd1d-104">Reapplies the current sorting parameters to the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="0cd1d-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0cd1d-105">Permissions</span></span>
<span data-ttu-id="0cd1d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0cd1d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0cd1d-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0cd1d-108">Permission type</span></span>      | <span data-ttu-id="0cd1d-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0cd1d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0cd1d-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0cd1d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0cd1d-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0cd1d-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0cd1d-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0cd1d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0cd1d-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0cd1d-113">Not supported.</span></span>    |
|<span data-ttu-id="0cd1d-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0cd1d-114">Application</span></span> | <span data-ttu-id="0cd1d-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0cd1d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0cd1d-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0cd1d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/reapply
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/reapply

```
## <a name="request-headers"></a><span data-ttu-id="0cd1d-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0cd1d-117">Request headers</span></span>
| <span data-ttu-id="0cd1d-118">名前</span><span class="sxs-lookup"><span data-stu-id="0cd1d-118">Name</span></span>       | <span data-ttu-id="0cd1d-119">説明</span><span class="sxs-lookup"><span data-stu-id="0cd1d-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0cd1d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="0cd1d-120">Authorization</span></span>  | <span data-ttu-id="0cd1d-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0cd1d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0cd1d-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0cd1d-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="0cd1d-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="0cd1d-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0cd1d-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="0cd1d-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="0cd1d-127">応答</span><span class="sxs-lookup"><span data-stu-id="0cd1d-127">Response</span></span>

<span data-ttu-id="0cd1d-p104">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="0cd1d-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0cd1d-130">例</span><span class="sxs-lookup"><span data-stu-id="0cd1d-130">Example</span></span>
<span data-ttu-id="0cd1d-131">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="0cd1d-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0cd1d-132">要求</span><span class="sxs-lookup"><span data-stu-id="0cd1d-132">Request</span></span>
<span data-ttu-id="0cd1d-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0cd1d-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablesort_reapply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/sort/reapply
```

##### <a name="response"></a><span data-ttu-id="0cd1d-134">応答</span><span class="sxs-lookup"><span data-stu-id="0cd1d-134">Response</span></span>
<span data-ttu-id="0cd1d-135">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="0cd1d-135">Here is an example of the response.</span></span> 
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
  "description": "TableSort: reapply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->