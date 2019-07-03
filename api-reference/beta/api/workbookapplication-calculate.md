---
title: 'workbookApplication: 計算'
description: Excel で現在開いているすべてのブックを再計算します。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: fc82d01c7304ca566534d650f7fdda8dc6ca295e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35448487"
---
# <a name="workbookapplication-calculate"></a><span data-ttu-id="b7c43-103">workbookApplication: 計算</span><span class="sxs-lookup"><span data-stu-id="b7c43-103">workbookApplication: calculate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7c43-104">Excel で現在開いているすべてのブックを再計算します。</span><span class="sxs-lookup"><span data-stu-id="b7c43-104">Recalculate all currently opened workbooks in Excel.</span></span>
## <a name="permissions"></a><span data-ttu-id="b7c43-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b7c43-105">Permissions</span></span>
<span data-ttu-id="b7c43-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b7c43-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7c43-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b7c43-108">Permission type</span></span>      | <span data-ttu-id="b7c43-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b7c43-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b7c43-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b7c43-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b7c43-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b7c43-111">Not supported.</span></span>    |
|<span data-ttu-id="b7c43-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b7c43-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7c43-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b7c43-113">Not supported.</span></span>    |
|<span data-ttu-id="b7c43-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b7c43-114">Application</span></span> | <span data-ttu-id="b7c43-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b7c43-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b7c43-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b7c43-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/application/calculate

```
## <a name="request-headers"></a><span data-ttu-id="b7c43-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b7c43-117">Request headers</span></span>
| <span data-ttu-id="b7c43-118">名前</span><span class="sxs-lookup"><span data-stu-id="b7c43-118">Name</span></span>       | <span data-ttu-id="b7c43-119">説明</span><span class="sxs-lookup"><span data-stu-id="b7c43-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b7c43-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="b7c43-120">Authorization</span></span>  | <span data-ttu-id="b7c43-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b7c43-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b7c43-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="b7c43-123">Request body</span></span>
<span data-ttu-id="b7c43-124">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="b7c43-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b7c43-125">パラメーター</span><span class="sxs-lookup"><span data-stu-id="b7c43-125">Parameter</span></span>    | <span data-ttu-id="b7c43-126">型</span><span class="sxs-lookup"><span data-stu-id="b7c43-126">Type</span></span>   |<span data-ttu-id="b7c43-127">説明</span><span class="sxs-lookup"><span data-stu-id="b7c43-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b7c43-128">calculationType</span><span class="sxs-lookup"><span data-stu-id="b7c43-128">calculationType</span></span>|<span data-ttu-id="b7c43-129">string</span><span class="sxs-lookup"><span data-stu-id="b7c43-129">string</span></span>|<span data-ttu-id="b7c43-130">使用する計算の種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="b7c43-130">Specifies the calculation type to use.</span></span>  <span data-ttu-id="b7c43-131">可能な値は、`Recalculate`、`Full`、`FullRebuild` です。</span><span class="sxs-lookup"><span data-stu-id="b7c43-131">Possible values are: `Recalculate`, `Full`, `FullRebuild`.</span></span>|

## <a name="response"></a><span data-ttu-id="b7c43-132">応答</span><span class="sxs-lookup"><span data-stu-id="b7c43-132">Response</span></span>

<span data-ttu-id="b7c43-p104">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="b7c43-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7c43-135">例</span><span class="sxs-lookup"><span data-stu-id="b7c43-135">Example</span></span>
<span data-ttu-id="b7c43-136">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="b7c43-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b7c43-137">要求</span><span class="sxs-lookup"><span data-stu-id="b7c43-137">Request</span></span>
<span data-ttu-id="b7c43-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b7c43-138">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b7c43-139">プロトコル</span><span class="sxs-lookup"><span data-stu-id="b7c43-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "workbookApplication_calculate"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/application/calculate
Content-type: application/json
Content-length: 48

{
  "calculationType": "calculationType-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b7c43-140">C#</span><span class="sxs-lookup"><span data-stu-id="b7c43-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookapplication-calculate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b7c43-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="b7c43-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookapplication-calculate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b7c43-142">目的-C</span><span class="sxs-lookup"><span data-stu-id="b7c43-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookapplication-calculate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b7c43-143">応答</span><span class="sxs-lookup"><span data-stu-id="b7c43-143">Response</span></span>
<span data-ttu-id="b7c43-144">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="b7c43-144">Here is an example of the response.</span></span> 
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
  "description": "workbookApplication: calculate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
