---
title: 'TableRow: delete'
description: テーブルから行を削除します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 1760f6fb51dd60556710984bac544058b78a8e6c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950285"
---
# <a name="tablerow-delete"></a><span data-ttu-id="7fde0-103">TableRow: delete</span><span class="sxs-lookup"><span data-stu-id="7fde0-103">TableRow: delete</span></span>

<span data-ttu-id="7fde0-104">テーブルから行を削除します。</span><span class="sxs-lookup"><span data-stu-id="7fde0-104">Deletes the row from the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="7fde0-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7fde0-105">Permissions</span></span>
<span data-ttu-id="7fde0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7fde0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7fde0-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7fde0-108">Permission type</span></span>      | <span data-ttu-id="7fde0-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7fde0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7fde0-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7fde0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7fde0-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7fde0-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7fde0-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7fde0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7fde0-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7fde0-113">Not supported.</span></span>    |
|<span data-ttu-id="7fde0-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7fde0-114">Application</span></span> | <span data-ttu-id="7fde0-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7fde0-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7fde0-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7fde0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows/{index}/delete
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows/{index}/delete

```
## <a name="request-headers"></a><span data-ttu-id="7fde0-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7fde0-117">Request headers</span></span>
| <span data-ttu-id="7fde0-118">名前</span><span class="sxs-lookup"><span data-stu-id="7fde0-118">Name</span></span>       | <span data-ttu-id="7fde0-119">説明</span><span class="sxs-lookup"><span data-stu-id="7fde0-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7fde0-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="7fde0-120">Authorization</span></span>  | <span data-ttu-id="7fde0-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7fde0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7fde0-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7fde0-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="7fde0-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="7fde0-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7fde0-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="7fde0-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="7fde0-127">応答</span><span class="sxs-lookup"><span data-stu-id="7fde0-127">Response</span></span>

<span data-ttu-id="7fde0-p104">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="7fde0-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7fde0-130">例</span><span class="sxs-lookup"><span data-stu-id="7fde0-130">Example</span></span>
<span data-ttu-id="7fde0-131">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="7fde0-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7fde0-132">要求</span><span class="sxs-lookup"><span data-stu-id="7fde0-132">Request</span></span>
<span data-ttu-id="7fde0-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7fde0-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablerow_delete"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows/{index}/delete
```

##### <a name="response"></a><span data-ttu-id="7fde0-134">応答</span><span class="sxs-lookup"><span data-stu-id="7fde0-134">Response</span></span>
<span data-ttu-id="7fde0-135">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="7fde0-135">Here is an example of the response.</span></span> 
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
  "description": "TableRow: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
