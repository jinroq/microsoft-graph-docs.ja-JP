---
title: 'アプリケーション: 計算'
description: Excel で現在開いているすべてのブックを再計算します。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: b5db5efda5da15d006188ae55f45b85e1325c38e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921942"
---
# <a name="application-calculate"></a><span data-ttu-id="792ee-103">アプリケーション: 計算</span><span class="sxs-lookup"><span data-stu-id="792ee-103">Application: calculate</span></span>

> <span data-ttu-id="792ee-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="792ee-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="792ee-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="792ee-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="792ee-106">Excel で現在開いているすべてのブックを再計算します。</span><span class="sxs-lookup"><span data-stu-id="792ee-106">Recalculate all currently opened workbooks in Excel.</span></span>
## <a name="permissions"></a><span data-ttu-id="792ee-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="792ee-107">Permissions</span></span>
<span data-ttu-id="792ee-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="792ee-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="792ee-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="792ee-110">Permission type</span></span>      | <span data-ttu-id="792ee-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="792ee-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="792ee-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="792ee-112">Delegated (work or school account)</span></span> | <span data-ttu-id="792ee-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="792ee-113">Not supported.</span></span>    |
|<span data-ttu-id="792ee-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="792ee-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="792ee-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="792ee-115">Not supported.</span></span>    |
|<span data-ttu-id="792ee-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="792ee-116">Application</span></span> | <span data-ttu-id="792ee-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="792ee-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="792ee-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="792ee-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/application/calculate

```
## <a name="request-headers"></a><span data-ttu-id="792ee-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="792ee-119">Request headers</span></span>
| <span data-ttu-id="792ee-120">名前</span><span class="sxs-lookup"><span data-stu-id="792ee-120">Name</span></span>       | <span data-ttu-id="792ee-121">説明</span><span class="sxs-lookup"><span data-stu-id="792ee-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="792ee-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="792ee-122">Authorization</span></span>  | <span data-ttu-id="792ee-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="792ee-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="792ee-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="792ee-125">Request body</span></span>
<span data-ttu-id="792ee-126">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="792ee-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="792ee-127">パラメーター</span><span class="sxs-lookup"><span data-stu-id="792ee-127">Parameter</span></span>    | <span data-ttu-id="792ee-128">型</span><span class="sxs-lookup"><span data-stu-id="792ee-128">Type</span></span>   |<span data-ttu-id="792ee-129">説明</span><span class="sxs-lookup"><span data-stu-id="792ee-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="792ee-130">calculationType</span><span class="sxs-lookup"><span data-stu-id="792ee-130">calculationType</span></span>|<span data-ttu-id="792ee-131">文字列</span><span class="sxs-lookup"><span data-stu-id="792ee-131">string</span></span>|<span data-ttu-id="792ee-132">使用する計算の種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="792ee-132">Specifies the calculation type to use.</span></span>  <span data-ttu-id="792ee-133">可能な値は、`Recalculate`、`Full`、`FullRebuild` です。</span><span class="sxs-lookup"><span data-stu-id="792ee-133">Possible values are: `Recalculate`, `Full`, `FullRebuild`.</span></span>|

## <a name="response"></a><span data-ttu-id="792ee-134">応答</span><span class="sxs-lookup"><span data-stu-id="792ee-134">Response</span></span>

<span data-ttu-id="792ee-p105">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="792ee-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="792ee-137">例</span><span class="sxs-lookup"><span data-stu-id="792ee-137">Example</span></span>
<span data-ttu-id="792ee-138">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="792ee-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="792ee-139">要求</span><span class="sxs-lookup"><span data-stu-id="792ee-139">Request</span></span>
<span data-ttu-id="792ee-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="792ee-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "application_calculate"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/application/calculate
Content-type: application/json
Content-length: 48

{
  "calculationType": "calculationType-value"
}
```

##### <a name="response"></a><span data-ttu-id="792ee-141">応答</span><span class="sxs-lookup"><span data-stu-id="792ee-141">Response</span></span>
<span data-ttu-id="792ee-142">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="792ee-142">Here is an example of the response.</span></span> 
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
  "description": "Application: calculate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
