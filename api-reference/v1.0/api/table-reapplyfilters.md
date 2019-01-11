---
title: 'Table: reapplyFilters'
description: 現在テーブルにあるすべてのフィルターを再適用します。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: ffeb1881cecc932e9c8c7bb70672a6f03fefc534
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27808163"
---
# <a name="table-reapplyfilters"></a><span data-ttu-id="66fe1-103">Table: reapplyFilters</span><span class="sxs-lookup"><span data-stu-id="66fe1-103">Table: reapplyFilters</span></span>

<span data-ttu-id="66fe1-104">現在テーブルにあるすべてのフィルターを再適用します。</span><span class="sxs-lookup"><span data-stu-id="66fe1-104">Reapplies all the filters currently on the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="66fe1-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="66fe1-105">Permissions</span></span>
<span data-ttu-id="66fe1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="66fe1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66fe1-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="66fe1-108">Permission type</span></span>      | <span data-ttu-id="66fe1-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="66fe1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="66fe1-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="66fe1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="66fe1-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="66fe1-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="66fe1-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="66fe1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66fe1-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="66fe1-113">Not supported.</span></span>    |
|<span data-ttu-id="66fe1-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="66fe1-114">Application</span></span> | <span data-ttu-id="66fe1-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="66fe1-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="66fe1-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="66fe1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/reapplyFilters
POST /workbook/worksheets/{id|name}/tables/{id|name}/reapplyFilters

```
## <a name="request-headers"></a><span data-ttu-id="66fe1-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="66fe1-117">Request headers</span></span>
| <span data-ttu-id="66fe1-118">名前</span><span class="sxs-lookup"><span data-stu-id="66fe1-118">Name</span></span>       | <span data-ttu-id="66fe1-119">説明</span><span class="sxs-lookup"><span data-stu-id="66fe1-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="66fe1-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="66fe1-120">Authorization</span></span>  | <span data-ttu-id="66fe1-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="66fe1-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="66fe1-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="66fe1-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="66fe1-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="66fe1-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="66fe1-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="66fe1-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="66fe1-127">応答</span><span class="sxs-lookup"><span data-stu-id="66fe1-127">Response</span></span>

<span data-ttu-id="66fe1-p104">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="66fe1-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66fe1-130">例</span><span class="sxs-lookup"><span data-stu-id="66fe1-130">Example</span></span>
<span data-ttu-id="66fe1-131">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="66fe1-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="66fe1-132">要求</span><span class="sxs-lookup"><span data-stu-id="66fe1-132">Request</span></span>
<span data-ttu-id="66fe1-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="66fe1-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "table_reapplyfilters"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/reapplyFilters
```

##### <a name="response"></a><span data-ttu-id="66fe1-134">応答</span><span class="sxs-lookup"><span data-stu-id="66fe1-134">Response</span></span>
<span data-ttu-id="66fe1-135">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="66fe1-135">Here is an example of the response.</span></span> 
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
  "description": "Table: reapplyFilters",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
