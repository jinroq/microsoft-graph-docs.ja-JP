---
title: 'Table: delete'
description: テーブルを削除します。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 80af89dc41adf7458558377e2ea187126993424e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849400"
---
# <a name="table-delete"></a><span data-ttu-id="881a3-103">Table: delete</span><span class="sxs-lookup"><span data-stu-id="881a3-103">Table: delete</span></span>

<span data-ttu-id="881a3-104">テーブルを削除します。</span><span class="sxs-lookup"><span data-stu-id="881a3-104">Deletes the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="881a3-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="881a3-105">Permissions</span></span>
<span data-ttu-id="881a3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="881a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="881a3-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="881a3-108">Permission type</span></span>      | <span data-ttu-id="881a3-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="881a3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="881a3-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="881a3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="881a3-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="881a3-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="881a3-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="881a3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="881a3-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="881a3-113">Not supported.</span></span>    |
|<span data-ttu-id="881a3-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="881a3-114">Application</span></span> | <span data-ttu-id="881a3-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="881a3-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="881a3-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="881a3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/delete
POST /workbook/worksheets/{id|name}/tables/{id|name}/delete

```
## <a name="request-headers"></a><span data-ttu-id="881a3-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="881a3-117">Request headers</span></span>
| <span data-ttu-id="881a3-118">名前</span><span class="sxs-lookup"><span data-stu-id="881a3-118">Name</span></span>       | <span data-ttu-id="881a3-119">説明</span><span class="sxs-lookup"><span data-stu-id="881a3-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="881a3-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="881a3-120">Authorization</span></span>  | <span data-ttu-id="881a3-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="881a3-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="881a3-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="881a3-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="881a3-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="881a3-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="881a3-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="881a3-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="881a3-127">応答</span><span class="sxs-lookup"><span data-stu-id="881a3-127">Response</span></span>

<span data-ttu-id="881a3-p104">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="881a3-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="881a3-130">例</span><span class="sxs-lookup"><span data-stu-id="881a3-130">Example</span></span>
<span data-ttu-id="881a3-131">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="881a3-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="881a3-132">要求</span><span class="sxs-lookup"><span data-stu-id="881a3-132">Request</span></span>
<span data-ttu-id="881a3-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="881a3-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "table_delete"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/delete
```

##### <a name="response"></a><span data-ttu-id="881a3-134">応答</span><span class="sxs-lookup"><span data-stu-id="881a3-134">Response</span></span>
<span data-ttu-id="881a3-135">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="881a3-135">Here is an example of the response.</span></span> 
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
  "description": "Table: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
