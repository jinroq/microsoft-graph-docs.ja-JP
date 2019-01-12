---
title: 'TableSort: clear　'
description: テーブルに現在設定されている並べ替えをクリアします。これにより表の順序が変更されることはありませんが、ヘッダーのボタンの状態がクリアされます。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 90ac8b30c3b8513bdd73fa40746268212a8c0df9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912191"
---
# <a name="tablesort-clear"></a><span data-ttu-id="0bc1e-104">TableSort: clear　</span><span class="sxs-lookup"><span data-stu-id="0bc1e-104">TableSort: clear</span></span>

<span data-ttu-id="0bc1e-p102">テーブルに現在設定されている並べ替えをクリアします。これにより表の順序が変更されることはありませんが、ヘッダーのボタンの状態がクリアされます。</span><span class="sxs-lookup"><span data-stu-id="0bc1e-p102">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>
## <a name="permissions"></a><span data-ttu-id="0bc1e-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0bc1e-107">Permissions</span></span>
<span data-ttu-id="0bc1e-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0bc1e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0bc1e-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0bc1e-110">Permission type</span></span>      | <span data-ttu-id="0bc1e-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0bc1e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0bc1e-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0bc1e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0bc1e-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0bc1e-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0bc1e-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0bc1e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0bc1e-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0bc1e-115">Not supported.</span></span>    |
|<span data-ttu-id="0bc1e-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0bc1e-116">Application</span></span> | <span data-ttu-id="0bc1e-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0bc1e-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0bc1e-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0bc1e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/clear
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/clear

```
## <a name="request-headers"></a><span data-ttu-id="0bc1e-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0bc1e-119">Request headers</span></span>
| <span data-ttu-id="0bc1e-120">名前</span><span class="sxs-lookup"><span data-stu-id="0bc1e-120">Name</span></span>       | <span data-ttu-id="0bc1e-121">説明</span><span class="sxs-lookup"><span data-stu-id="0bc1e-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0bc1e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0bc1e-122">Authorization</span></span>  | <span data-ttu-id="0bc1e-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0bc1e-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0bc1e-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0bc1e-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="0bc1e-p105">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="0bc1e-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0bc1e-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="0bc1e-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="0bc1e-129">応答</span><span class="sxs-lookup"><span data-stu-id="0bc1e-129">Response</span></span>

<span data-ttu-id="0bc1e-p106">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="0bc1e-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0bc1e-132">例</span><span class="sxs-lookup"><span data-stu-id="0bc1e-132">Example</span></span>
<span data-ttu-id="0bc1e-133">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="0bc1e-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0bc1e-134">要求</span><span class="sxs-lookup"><span data-stu-id="0bc1e-134">Request</span></span>
<span data-ttu-id="0bc1e-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0bc1e-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablesort_clear"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/sort/clear
```

##### <a name="response"></a><span data-ttu-id="0bc1e-136">応答</span><span class="sxs-lookup"><span data-stu-id="0bc1e-136">Response</span></span>
<span data-ttu-id="0bc1e-137">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="0bc1e-137">Here is an example of the response.</span></span> 
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
  "description": "TableSort: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
