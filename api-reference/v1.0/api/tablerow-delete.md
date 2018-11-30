---
title: 'TableRow: delete'
description: テーブルから行を削除します。
ms.openlocfilehash: ca70e0d7822f881e2be024eb0de2966684ef8b47
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023705"
---
# <a name="tablerow-delete"></a><span data-ttu-id="f42aa-103">TableRow: delete</span><span class="sxs-lookup"><span data-stu-id="f42aa-103">TableRow: delete</span></span>

<span data-ttu-id="f42aa-104">テーブルから行を削除します。</span><span class="sxs-lookup"><span data-stu-id="f42aa-104">Deletes the row from the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="f42aa-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f42aa-105">Permissions</span></span>
<span data-ttu-id="f42aa-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f42aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f42aa-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f42aa-108">Permission type</span></span>      | <span data-ttu-id="f42aa-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f42aa-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f42aa-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f42aa-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f42aa-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f42aa-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f42aa-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f42aa-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f42aa-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f42aa-113">Not supported.</span></span>    |
|<span data-ttu-id="f42aa-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f42aa-114">Application</span></span> | <span data-ttu-id="f42aa-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f42aa-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f42aa-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f42aa-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows/{index}/delete
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows/{index}/delete

```
## <a name="request-headers"></a><span data-ttu-id="f42aa-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f42aa-117">Request headers</span></span>
| <span data-ttu-id="f42aa-118">名前</span><span class="sxs-lookup"><span data-stu-id="f42aa-118">Name</span></span>       | <span data-ttu-id="f42aa-119">説明</span><span class="sxs-lookup"><span data-stu-id="f42aa-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f42aa-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="f42aa-120">Authorization</span></span>  | <span data-ttu-id="f42aa-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f42aa-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f42aa-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f42aa-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="f42aa-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="f42aa-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f42aa-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="f42aa-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="f42aa-127">応答</span><span class="sxs-lookup"><span data-stu-id="f42aa-127">Response</span></span>

<span data-ttu-id="f42aa-p104">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="f42aa-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f42aa-130">例</span><span class="sxs-lookup"><span data-stu-id="f42aa-130">Example</span></span>
<span data-ttu-id="f42aa-131">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="f42aa-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f42aa-132">要求</span><span class="sxs-lookup"><span data-stu-id="f42aa-132">Request</span></span>
<span data-ttu-id="f42aa-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f42aa-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablerow_delete"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows/{index}/delete
```

##### <a name="response"></a><span data-ttu-id="f42aa-134">応答</span><span class="sxs-lookup"><span data-stu-id="f42aa-134">Response</span></span>
<span data-ttu-id="f42aa-135">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="f42aa-135">Here is an example of the response.</span></span> 
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