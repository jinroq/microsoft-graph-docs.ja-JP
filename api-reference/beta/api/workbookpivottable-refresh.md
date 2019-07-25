---
title: 'workbookPivotTable: refresh'
description: ピボットテーブルを更新します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: ff537d8a00f3893a78fb6fbd0c19ad9deac3ae8e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35866450"
---
# <a name="workbookpivottable-refresh"></a><span data-ttu-id="5c9a5-103">workbookPivotTable: refresh</span><span class="sxs-lookup"><span data-stu-id="5c9a5-103">workbookPivotTable: refresh</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c9a5-104">ピボットテーブルを更新します。</span><span class="sxs-lookup"><span data-stu-id="5c9a5-104">Refreshes the PivotTable.</span></span>


## <a name="permissions"></a><span data-ttu-id="5c9a5-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5c9a5-105">Permissions</span></span>
<span data-ttu-id="5c9a5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5c9a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5c9a5-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5c9a5-108">Permission type</span></span>      | <span data-ttu-id="5c9a5-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5c9a5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5c9a5-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5c9a5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5c9a5-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5c9a5-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5c9a5-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5c9a5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c9a5-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5c9a5-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5c9a5-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5c9a5-114">Application</span></span> | <span data-ttu-id="5c9a5-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5c9a5-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5c9a5-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5c9a5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/pivotTables/{id}/refresh
```
## <a name="request-headers"></a><span data-ttu-id="5c9a5-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5c9a5-117">Request headers</span></span>
| <span data-ttu-id="5c9a5-118">名前</span><span class="sxs-lookup"><span data-stu-id="5c9a5-118">Name</span></span>       | <span data-ttu-id="5c9a5-119">説明</span><span class="sxs-lookup"><span data-stu-id="5c9a5-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5c9a5-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="5c9a5-120">Authorization</span></span>  | <span data-ttu-id="5c9a5-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5c9a5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5c9a5-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="5c9a5-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="5c9a5-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="5c9a5-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c9a5-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="5c9a5-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="5c9a5-127">応答</span><span class="sxs-lookup"><span data-stu-id="5c9a5-127">Response</span></span>

<span data-ttu-id="5c9a5-p104">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="5c9a5-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c9a5-130">例</span><span class="sxs-lookup"><span data-stu-id="5c9a5-130">Example</span></span>
<span data-ttu-id="5c9a5-131">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="5c9a5-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5c9a5-132">要求</span><span class="sxs-lookup"><span data-stu-id="5c9a5-132">Request</span></span>
<span data-ttu-id="5c9a5-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5c9a5-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5c9a5-134">プロトコル</span><span class="sxs-lookup"><span data-stu-id="5c9a5-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "workbookpivottable_refresh"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/pivotTables/{id}/refresh
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5c9a5-135">C#</span><span class="sxs-lookup"><span data-stu-id="5c9a5-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookpivottable-refresh-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5c9a5-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="5c9a5-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookpivottable-refresh-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5c9a5-137">目的-C</span><span class="sxs-lookup"><span data-stu-id="5c9a5-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookpivottable-refresh-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="5c9a5-138">Java</span><span class="sxs-lookup"><span data-stu-id="5c9a5-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookpivottable-refresh-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5c9a5-139">応答</span><span class="sxs-lookup"><span data-stu-id="5c9a5-139">Response</span></span>
<span data-ttu-id="5c9a5-140">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="5c9a5-140">Here is an example of the response.</span></span>
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
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
