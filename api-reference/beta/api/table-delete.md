---
title: 'Table: delete'
description: テーブルを削除します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: dda1ddcef2c267272410555d564e5a13758eb12f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35991094"
---
# <a name="table-delete"></a><span data-ttu-id="9604c-103">Table: delete</span><span class="sxs-lookup"><span data-stu-id="9604c-103">Table: delete</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9604c-104">テーブルを削除します。</span><span class="sxs-lookup"><span data-stu-id="9604c-104">Deletes the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="9604c-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9604c-105">Permissions</span></span>
<span data-ttu-id="9604c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9604c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9604c-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9604c-108">Permission type</span></span>      | <span data-ttu-id="9604c-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9604c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9604c-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9604c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9604c-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9604c-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9604c-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9604c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9604c-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9604c-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9604c-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9604c-114">Application</span></span> | <span data-ttu-id="9604c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9604c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9604c-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9604c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/delete
POST /workbook/worksheets/{id|name}/tables/{id|name}/delete

```
## <a name="request-headers"></a><span data-ttu-id="9604c-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9604c-117">Request headers</span></span>
| <span data-ttu-id="9604c-118">名前</span><span class="sxs-lookup"><span data-stu-id="9604c-118">Name</span></span>       | <span data-ttu-id="9604c-119">説明</span><span class="sxs-lookup"><span data-stu-id="9604c-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9604c-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="9604c-120">Authorization</span></span>  | <span data-ttu-id="9604c-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9604c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9604c-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9604c-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="9604c-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="9604c-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9604c-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="9604c-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="9604c-127">応答</span><span class="sxs-lookup"><span data-stu-id="9604c-127">Response</span></span>

<span data-ttu-id="9604c-p104">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="9604c-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9604c-130">例</span><span class="sxs-lookup"><span data-stu-id="9604c-130">Example</span></span>
<span data-ttu-id="9604c-131">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="9604c-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9604c-132">要求</span><span class="sxs-lookup"><span data-stu-id="9604c-132">Request</span></span>
<span data-ttu-id="9604c-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9604c-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "table_delete"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/delete
```

##### <a name="response"></a><span data-ttu-id="9604c-134">応答</span><span class="sxs-lookup"><span data-stu-id="9604c-134">Response</span></span>
<span data-ttu-id="9604c-135">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="9604c-135">Here is an example of the response.</span></span> 
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
<!--
{
  "type": "#page.annotation",
  "description": "Table: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
