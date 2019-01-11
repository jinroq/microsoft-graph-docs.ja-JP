---
title: 'TableSort: clear　'
description: テーブルに現在設定されている並べ替えをクリアします。これにより表の順序が変更されることはありませんが、ヘッダーのボタンの状態がクリアされます。
localization_priority: Normal
ms.openlocfilehash: 1d7d695bfc1d1e6d951f44e0e3e7cde21c4e5904
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27841329"
---
# <a name="tablesort-clear"></a><span data-ttu-id="e53ab-104">TableSort: clear　</span><span class="sxs-lookup"><span data-stu-id="e53ab-104">TableSort: clear</span></span>

> <span data-ttu-id="e53ab-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e53ab-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e53ab-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e53ab-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e53ab-p103">テーブルに現在設定されている並べ替えをクリアします。これにより表の順序が変更されることはありませんが、ヘッダーのボタンの状態がクリアされます。</span><span class="sxs-lookup"><span data-stu-id="e53ab-p103">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>
## <a name="permissions"></a><span data-ttu-id="e53ab-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e53ab-109">Permissions</span></span>
<span data-ttu-id="e53ab-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e53ab-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e53ab-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e53ab-112">Permission type</span></span>      | <span data-ttu-id="e53ab-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e53ab-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e53ab-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e53ab-114">Delegated (work or school account)</span></span> | <span data-ttu-id="e53ab-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e53ab-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e53ab-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e53ab-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e53ab-117">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e53ab-117">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e53ab-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e53ab-118">Application</span></span> | <span data-ttu-id="e53ab-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e53ab-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e53ab-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e53ab-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/clear
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/clear

```
## <a name="request-headers"></a><span data-ttu-id="e53ab-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e53ab-121">Request headers</span></span>
| <span data-ttu-id="e53ab-122">名前</span><span class="sxs-lookup"><span data-stu-id="e53ab-122">Name</span></span>       | <span data-ttu-id="e53ab-123">説明</span><span class="sxs-lookup"><span data-stu-id="e53ab-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e53ab-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e53ab-124">Authorization</span></span>  | <span data-ttu-id="e53ab-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e53ab-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e53ab-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e53ab-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="e53ab-p106">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="e53ab-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e53ab-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="e53ab-130">Request body</span></span>

## <a name="response"></a><span data-ttu-id="e53ab-131">応答</span><span class="sxs-lookup"><span data-stu-id="e53ab-131">Response</span></span>

<span data-ttu-id="e53ab-p107">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="e53ab-p107">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e53ab-134">例</span><span class="sxs-lookup"><span data-stu-id="e53ab-134">Example</span></span>
<span data-ttu-id="e53ab-135">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="e53ab-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e53ab-136">要求</span><span class="sxs-lookup"><span data-stu-id="e53ab-136">Request</span></span>
<span data-ttu-id="e53ab-137">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e53ab-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablesort_clear"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/sort/clear
```

##### <a name="response"></a><span data-ttu-id="e53ab-138">応答</span><span class="sxs-lookup"><span data-stu-id="e53ab-138">Response</span></span>
<span data-ttu-id="e53ab-139">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="e53ab-139">Here is an example of the response.</span></span> 
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
