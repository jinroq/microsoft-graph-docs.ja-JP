---
title: 'workbookApplication: 計算'
description: Excel で現在開いているすべてのブックを再計算します。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 2e3a980ae7eab1dd3032ae68b180019ae4c7ceee
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636976"
---
# <a name="workbookapplication-calculate"></a><span data-ttu-id="c6132-103">workbookApplication: 計算</span><span class="sxs-lookup"><span data-stu-id="c6132-103">workbookApplication: calculate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c6132-104">Excel で現在開いているすべてのブックを再計算します。</span><span class="sxs-lookup"><span data-stu-id="c6132-104">Recalculate all currently opened workbooks in Excel.</span></span>
## <a name="permissions"></a><span data-ttu-id="c6132-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c6132-105">Permissions</span></span>
<span data-ttu-id="c6132-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c6132-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6132-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c6132-108">Permission type</span></span>      | <span data-ttu-id="c6132-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c6132-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c6132-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c6132-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c6132-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c6132-111">Not supported.</span></span>    |
|<span data-ttu-id="c6132-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c6132-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c6132-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c6132-113">Not supported.</span></span>    |
|<span data-ttu-id="c6132-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c6132-114">Application</span></span> | <span data-ttu-id="c6132-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c6132-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c6132-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c6132-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/application/calculate

```
## <a name="request-headers"></a><span data-ttu-id="c6132-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c6132-117">Request headers</span></span>
| <span data-ttu-id="c6132-118">名前</span><span class="sxs-lookup"><span data-stu-id="c6132-118">Name</span></span>       | <span data-ttu-id="c6132-119">説明</span><span class="sxs-lookup"><span data-stu-id="c6132-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c6132-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="c6132-120">Authorization</span></span>  | <span data-ttu-id="c6132-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c6132-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c6132-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="c6132-123">Request body</span></span>
<span data-ttu-id="c6132-124">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="c6132-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c6132-125">パラメーター</span><span class="sxs-lookup"><span data-stu-id="c6132-125">Parameter</span></span>    | <span data-ttu-id="c6132-126">型</span><span class="sxs-lookup"><span data-stu-id="c6132-126">Type</span></span>   |<span data-ttu-id="c6132-127">説明</span><span class="sxs-lookup"><span data-stu-id="c6132-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c6132-128">calculationType</span><span class="sxs-lookup"><span data-stu-id="c6132-128">calculationType</span></span>|<span data-ttu-id="c6132-129">string</span><span class="sxs-lookup"><span data-stu-id="c6132-129">string</span></span>|<span data-ttu-id="c6132-130">使用する計算の種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="c6132-130">Specifies the calculation type to use.</span></span>  <span data-ttu-id="c6132-131">可能な値は、`Recalculate`、`Full`、`FullRebuild` です。</span><span class="sxs-lookup"><span data-stu-id="c6132-131">Possible values are: `Recalculate`, `Full`, `FullRebuild`.</span></span>|

## <a name="response"></a><span data-ttu-id="c6132-132">応答</span><span class="sxs-lookup"><span data-stu-id="c6132-132">Response</span></span>

<span data-ttu-id="c6132-p104">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="c6132-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6132-135">例</span><span class="sxs-lookup"><span data-stu-id="c6132-135">Example</span></span>
<span data-ttu-id="c6132-136">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="c6132-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c6132-137">要求</span><span class="sxs-lookup"><span data-stu-id="c6132-137">Request</span></span>
<span data-ttu-id="c6132-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c6132-138">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="c6132-139">応答</span><span class="sxs-lookup"><span data-stu-id="c6132-139">Response</span></span>
<span data-ttu-id="c6132-140">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="c6132-140">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->

```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="c6132-141">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="c6132-141">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c6132-142">Visual</span><span class="sxs-lookup"><span data-stu-id="c6132-142">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/workbookApplication_calculate-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c6132-143">Java</span><span class="sxs-lookup"><span data-stu-id="c6132-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/workbookApplication_calculate-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/workbookapplication-calculate.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/workbookapplication-calculate.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
