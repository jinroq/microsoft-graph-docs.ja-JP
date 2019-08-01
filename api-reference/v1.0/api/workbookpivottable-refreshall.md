---
title: 'workbookPivotTable: refreshAll'
description: 指定されたワークシート内のピボットテーブルを更新します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 8a8eaf706e34a91383c327a1c47ca4f6e14597d2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36026402"
---
# <a name="workbookpivottable-refreshall"></a><span data-ttu-id="15f1b-103">workbookPivotTable: refreshAll</span><span class="sxs-lookup"><span data-stu-id="15f1b-103">workbookPivotTable: refreshAll</span></span>

<span data-ttu-id="15f1b-104">指定されたワークシート内のピボットテーブルを更新します。</span><span class="sxs-lookup"><span data-stu-id="15f1b-104">Refreshes the PivotTable within a given worksheet.</span></span>

## <a name="permissions"></a><span data-ttu-id="15f1b-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="15f1b-105">Permissions</span></span>
<span data-ttu-id="15f1b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="15f1b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15f1b-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="15f1b-108">Permission type</span></span>      | <span data-ttu-id="15f1b-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="15f1b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="15f1b-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="15f1b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="15f1b-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="15f1b-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="15f1b-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="15f1b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15f1b-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="15f1b-113">Not supported.</span></span>    |
|<span data-ttu-id="15f1b-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="15f1b-114">Application</span></span> | <span data-ttu-id="15f1b-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="15f1b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="15f1b-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="15f1b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/pivotTables/refreshAll

```
## <a name="request-headers"></a><span data-ttu-id="15f1b-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="15f1b-117">Request headers</span></span>
| <span data-ttu-id="15f1b-118">名前</span><span class="sxs-lookup"><span data-stu-id="15f1b-118">Name</span></span>       | <span data-ttu-id="15f1b-119">説明</span><span class="sxs-lookup"><span data-stu-id="15f1b-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="15f1b-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="15f1b-120">Authorization</span></span>  | <span data-ttu-id="15f1b-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="15f1b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="15f1b-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="15f1b-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="15f1b-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="15f1b-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="15f1b-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="15f1b-126">Request body</span></span>

### <a name="response"></a><span data-ttu-id="15f1b-127">応答</span><span class="sxs-lookup"><span data-stu-id="15f1b-127">Response</span></span>
<span data-ttu-id="15f1b-p104">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="15f1b-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15f1b-130">例</span><span class="sxs-lookup"><span data-stu-id="15f1b-130">Example</span></span>
<span data-ttu-id="15f1b-131">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="15f1b-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="15f1b-132">要求</span><span class="sxs-lookup"><span data-stu-id="15f1b-132">Request</span></span>
<span data-ttu-id="15f1b-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="15f1b-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="15f1b-134">プロトコル</span><span class="sxs-lookup"><span data-stu-id="15f1b-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "workbookpivottable_refreshall"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/pivotTables/refreshAll
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="15f1b-135">C#</span><span class="sxs-lookup"><span data-stu-id="15f1b-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookpivottable-refreshall-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="15f1b-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="15f1b-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookpivottable-refreshall-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="15f1b-137">目的-C</span><span class="sxs-lookup"><span data-stu-id="15f1b-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookpivottable-refreshall-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="15f1b-138">Java</span><span class="sxs-lookup"><span data-stu-id="15f1b-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookpivottable-refreshall-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="15f1b-139">応答</span><span class="sxs-lookup"><span data-stu-id="15f1b-139">Response</span></span>
<span data-ttu-id="15f1b-140">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="15f1b-140">Here is an example of the response.</span></span>
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
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
