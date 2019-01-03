---
title: 'TableSort: clear　'
description: テーブルに現在設定されている並べ替えをクリアします。これにより表の順序が変更されることはありませんが、ヘッダーのボタンの状態がクリアされます。
ms.openlocfilehash: f93b640188faedc228c56b6e13497ade84190765
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073351"
---
# <a name="tablesort-clear"></a><span data-ttu-id="05759-104">TableSort: clear　</span><span class="sxs-lookup"><span data-stu-id="05759-104">TableSort: clear</span></span>

> <span data-ttu-id="05759-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="05759-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="05759-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="05759-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="05759-p103">テーブルに現在設定されている並べ替えをクリアします。これにより表の順序が変更されることはありませんが、ヘッダーのボタンの状態がクリアされます。</span><span class="sxs-lookup"><span data-stu-id="05759-p103">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>
## <a name="permissions"></a><span data-ttu-id="05759-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="05759-109">Permissions</span></span>
<span data-ttu-id="05759-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="05759-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05759-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="05759-112">Permission type</span></span>      | <span data-ttu-id="05759-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="05759-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="05759-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="05759-114">Delegated (work or school account)</span></span> | <span data-ttu-id="05759-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="05759-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="05759-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="05759-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="05759-117">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="05759-117">Files.ReadWrite</span></span>    |
|<span data-ttu-id="05759-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="05759-118">Application</span></span> | <span data-ttu-id="05759-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="05759-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="05759-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="05759-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/clear
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/clear

```
## <a name="request-headers"></a><span data-ttu-id="05759-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="05759-121">Request headers</span></span>
| <span data-ttu-id="05759-122">名前</span><span class="sxs-lookup"><span data-stu-id="05759-122">Name</span></span>       | <span data-ttu-id="05759-123">説明</span><span class="sxs-lookup"><span data-stu-id="05759-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="05759-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="05759-124">Authorization</span></span>  | <span data-ttu-id="05759-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="05759-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="05759-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="05759-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="05759-p106">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="05759-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="05759-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="05759-130">Request body</span></span>

## <a name="response"></a><span data-ttu-id="05759-131">応答</span><span class="sxs-lookup"><span data-stu-id="05759-131">Response</span></span>

<span data-ttu-id="05759-p107">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="05759-p107">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05759-134">例</span><span class="sxs-lookup"><span data-stu-id="05759-134">Example</span></span>
<span data-ttu-id="05759-135">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="05759-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="05759-136">要求</span><span class="sxs-lookup"><span data-stu-id="05759-136">Request</span></span>
<span data-ttu-id="05759-137">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="05759-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablesort_clear"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/sort/clear
```

##### <a name="response"></a><span data-ttu-id="05759-138">応答</span><span class="sxs-lookup"><span data-stu-id="05759-138">Response</span></span>
<span data-ttu-id="05759-139">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="05759-139">Here is an example of the response.</span></span> 
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
  "description": "TableSort: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->