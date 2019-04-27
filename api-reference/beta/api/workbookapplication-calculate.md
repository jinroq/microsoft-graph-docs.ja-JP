---
title: 'workbookApplication: 計算'
description: Excel で現在開いているすべてのブックを再計算します。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: fae86c0a8c1511abb1780e03b36ed4edcc329e1b
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348409"
---
# <a name="workbookapplication-calculate"></a><span data-ttu-id="b9cd8-103">workbookApplication: 計算</span><span class="sxs-lookup"><span data-stu-id="b9cd8-103">workbookApplication: calculate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9cd8-104">Excel で現在開いているすべてのブックを再計算します。</span><span class="sxs-lookup"><span data-stu-id="b9cd8-104">Recalculate all currently opened workbooks in Excel.</span></span>
## <a name="permissions"></a><span data-ttu-id="b9cd8-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b9cd8-105">Permissions</span></span>
<span data-ttu-id="b9cd8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b9cd8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9cd8-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b9cd8-108">Permission type</span></span>      | <span data-ttu-id="b9cd8-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b9cd8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b9cd8-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b9cd8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b9cd8-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b9cd8-111">Not supported.</span></span>    |
|<span data-ttu-id="b9cd8-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b9cd8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9cd8-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b9cd8-113">Not supported.</span></span>    |
|<span data-ttu-id="b9cd8-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b9cd8-114">Application</span></span> | <span data-ttu-id="b9cd8-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b9cd8-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b9cd8-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b9cd8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/application/calculate

```
## <a name="request-headers"></a><span data-ttu-id="b9cd8-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b9cd8-117">Request headers</span></span>
| <span data-ttu-id="b9cd8-118">名前</span><span class="sxs-lookup"><span data-stu-id="b9cd8-118">Name</span></span>       | <span data-ttu-id="b9cd8-119">説明</span><span class="sxs-lookup"><span data-stu-id="b9cd8-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b9cd8-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9cd8-120">Authorization</span></span>  | <span data-ttu-id="b9cd8-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b9cd8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b9cd8-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="b9cd8-123">Request body</span></span>
<span data-ttu-id="b9cd8-124">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="b9cd8-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b9cd8-125">パラメーター</span><span class="sxs-lookup"><span data-stu-id="b9cd8-125">Parameter</span></span>    | <span data-ttu-id="b9cd8-126">型</span><span class="sxs-lookup"><span data-stu-id="b9cd8-126">Type</span></span>   |<span data-ttu-id="b9cd8-127">説明</span><span class="sxs-lookup"><span data-stu-id="b9cd8-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b9cd8-128">calculationType</span><span class="sxs-lookup"><span data-stu-id="b9cd8-128">calculationType</span></span>|<span data-ttu-id="b9cd8-129">string</span><span class="sxs-lookup"><span data-stu-id="b9cd8-129">string</span></span>|<span data-ttu-id="b9cd8-130">使用する計算の種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="b9cd8-130">Specifies the calculation type to use.</span></span>  <span data-ttu-id="b9cd8-131">可能な値は、`Recalculate`、`Full`、`FullRebuild` です。</span><span class="sxs-lookup"><span data-stu-id="b9cd8-131">Possible values are: `Recalculate`, `Full`, `FullRebuild`.</span></span>|

## <a name="response"></a><span data-ttu-id="b9cd8-132">応答</span><span class="sxs-lookup"><span data-stu-id="b9cd8-132">Response</span></span>

<span data-ttu-id="b9cd8-p104">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="b9cd8-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9cd8-135">例</span><span class="sxs-lookup"><span data-stu-id="b9cd8-135">Example</span></span>
<span data-ttu-id="b9cd8-136">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="b9cd8-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b9cd8-137">要求</span><span class="sxs-lookup"><span data-stu-id="b9cd8-137">Request</span></span>
<span data-ttu-id="b9cd8-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b9cd8-138">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="b9cd8-139">応答</span><span class="sxs-lookup"><span data-stu-id="b9cd8-139">Response</span></span>
<span data-ttu-id="b9cd8-140">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="b9cd8-140">Here is an example of the response.</span></span> 
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
  "suppressions": []
}
-->
