---
title: 'Table: reapplyFilters'
description: 現在テーブルにあるすべてのフィルターを再適用します。
author: lumine2008
ms.openlocfilehash: 3a6b4f7ca8db046c5009fb710122c5b15e57030b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27362112"
---
# <a name="table-reapplyfilters"></a><span data-ttu-id="4ab26-103">Table: reapplyFilters</span><span class="sxs-lookup"><span data-stu-id="4ab26-103">Table: reapplyFilters</span></span>

> <span data-ttu-id="4ab26-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4ab26-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4ab26-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4ab26-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4ab26-106">現在テーブルにあるすべてのフィルターを再適用します。</span><span class="sxs-lookup"><span data-stu-id="4ab26-106">Reapplies all the filters currently on the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="4ab26-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4ab26-107">Permissions</span></span>
<span data-ttu-id="4ab26-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4ab26-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ab26-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4ab26-110">Permission type</span></span>      | <span data-ttu-id="4ab26-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4ab26-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4ab26-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4ab26-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4ab26-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4ab26-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4ab26-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4ab26-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ab26-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4ab26-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4ab26-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4ab26-116">Application</span></span> | <span data-ttu-id="4ab26-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4ab26-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4ab26-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4ab26-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/reapplyFilters
POST /workbook/worksheets/{id|name}/tables/{id|name}/reapplyFilters

```
## <a name="request-headers"></a><span data-ttu-id="4ab26-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4ab26-119">Request headers</span></span>
| <span data-ttu-id="4ab26-120">名前</span><span class="sxs-lookup"><span data-stu-id="4ab26-120">Name</span></span>       | <span data-ttu-id="4ab26-121">説明</span><span class="sxs-lookup"><span data-stu-id="4ab26-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4ab26-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ab26-122">Authorization</span></span>  | <span data-ttu-id="4ab26-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4ab26-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4ab26-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="4ab26-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="4ab26-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="4ab26-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ab26-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="4ab26-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="4ab26-129">応答</span><span class="sxs-lookup"><span data-stu-id="4ab26-129">Response</span></span>

<span data-ttu-id="4ab26-p105">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="4ab26-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ab26-132">例</span><span class="sxs-lookup"><span data-stu-id="4ab26-132">Example</span></span>
<span data-ttu-id="4ab26-133">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="4ab26-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4ab26-134">要求</span><span class="sxs-lookup"><span data-stu-id="4ab26-134">Request</span></span>
<span data-ttu-id="4ab26-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4ab26-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "table_reapplyfilters"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/reapplyFilters
```

##### <a name="response"></a><span data-ttu-id="4ab26-136">応答</span><span class="sxs-lookup"><span data-stu-id="4ab26-136">Response</span></span>
<span data-ttu-id="4ab26-137">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="4ab26-137">Here is an example of the response.</span></span> 
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
  "description": "Table: reapplyFilters",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->