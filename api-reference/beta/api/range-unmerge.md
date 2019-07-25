---
title: '範囲: 結合解除'
description: 範囲内のセルを結合解除して別々のセルにします。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: d0230892eda37fb3a5d1d18342085da8b779c415
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35874710"
---
# <a name="range-unmerge"></a><span data-ttu-id="bcc72-103">範囲: 結合解除</span><span class="sxs-lookup"><span data-stu-id="bcc72-103">Range: unmerge</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bcc72-104">範囲内のセルを結合解除して別々のセルにします。</span><span class="sxs-lookup"><span data-stu-id="bcc72-104">Unmerge the range cells into separate cells.</span></span>
## <a name="permissions"></a><span data-ttu-id="bcc72-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="bcc72-105">Permissions</span></span>
<span data-ttu-id="bcc72-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bcc72-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bcc72-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bcc72-108">Permission type</span></span>      | <span data-ttu-id="bcc72-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="bcc72-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bcc72-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bcc72-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bcc72-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bcc72-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bcc72-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bcc72-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bcc72-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bcc72-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bcc72-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bcc72-114">Application</span></span> | <span data-ttu-id="bcc72-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bcc72-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bcc72-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bcc72-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/unmerge
POST /workbook/worksheets/{id|name}/range(address='<address>')/unmerge
POST /workbook/tables/{id|name}/columns/{id|name}/range/unmerge

```
## <a name="request-headers"></a><span data-ttu-id="bcc72-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bcc72-117">Request headers</span></span>
| <span data-ttu-id="bcc72-118">名前</span><span class="sxs-lookup"><span data-stu-id="bcc72-118">Name</span></span>       | <span data-ttu-id="bcc72-119">説明</span><span class="sxs-lookup"><span data-stu-id="bcc72-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="bcc72-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="bcc72-120">Authorization</span></span>  | <span data-ttu-id="bcc72-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="bcc72-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bcc72-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="bcc72-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="bcc72-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="bcc72-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bcc72-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="bcc72-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="bcc72-127">応答</span><span class="sxs-lookup"><span data-stu-id="bcc72-127">Response</span></span>

<span data-ttu-id="bcc72-p104">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="bcc72-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bcc72-130">例</span><span class="sxs-lookup"><span data-stu-id="bcc72-130">Example</span></span>
<span data-ttu-id="bcc72-131">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="bcc72-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="bcc72-132">要求</span><span class="sxs-lookup"><span data-stu-id="bcc72-132">Request</span></span>
<span data-ttu-id="bcc72-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bcc72-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="bcc72-134">プロトコル</span><span class="sxs-lookup"><span data-stu-id="bcc72-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "range_unmerge"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/unmerge
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bcc72-135">C#</span><span class="sxs-lookup"><span data-stu-id="bcc72-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-unmerge-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bcc72-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="bcc72-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-unmerge-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bcc72-137">目的-C</span><span class="sxs-lookup"><span data-stu-id="bcc72-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-unmerge-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="bcc72-138">Java</span><span class="sxs-lookup"><span data-stu-id="bcc72-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-unmerge-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="bcc72-139">応答</span><span class="sxs-lookup"><span data-stu-id="bcc72-139">Response</span></span>
<span data-ttu-id="bcc72-140">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="bcc72-140">Here is an example of the response.</span></span> 
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
  "description": "Range: unmerge",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
