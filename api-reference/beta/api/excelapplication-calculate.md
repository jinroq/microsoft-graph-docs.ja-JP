---
title: 'アプリケーション: 計算'
description: Excel で現在開いているすべてのブックを再計算します。
ms.openlocfilehash: 5d2d0d5603f70691d2c73548bd7a20acc03c340e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071052"
---
# <a name="application-calculate"></a><span data-ttu-id="6465f-103">アプリケーション: 計算</span><span class="sxs-lookup"><span data-stu-id="6465f-103">Application: calculate</span></span>

> <span data-ttu-id="6465f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6465f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6465f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6465f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6465f-106">Excel で現在開いているすべてのブックを再計算します。</span><span class="sxs-lookup"><span data-stu-id="6465f-106">Recalculate all currently opened workbooks in Excel.</span></span>
## <a name="permissions"></a><span data-ttu-id="6465f-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6465f-107">Permissions</span></span>
<span data-ttu-id="6465f-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6465f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6465f-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6465f-110">Permission type</span></span>      | <span data-ttu-id="6465f-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6465f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6465f-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6465f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6465f-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6465f-113">Not supported.</span></span>    |
|<span data-ttu-id="6465f-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6465f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6465f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6465f-115">Not supported.</span></span>    |
|<span data-ttu-id="6465f-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6465f-116">Application</span></span> | <span data-ttu-id="6465f-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6465f-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6465f-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6465f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/application/calculate

```
## <a name="request-headers"></a><span data-ttu-id="6465f-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6465f-119">Request headers</span></span>
| <span data-ttu-id="6465f-120">名前</span><span class="sxs-lookup"><span data-stu-id="6465f-120">Name</span></span>       | <span data-ttu-id="6465f-121">説明</span><span class="sxs-lookup"><span data-stu-id="6465f-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6465f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6465f-122">Authorization</span></span>  | <span data-ttu-id="6465f-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6465f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6465f-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="6465f-125">Request body</span></span>
<span data-ttu-id="6465f-126">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="6465f-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6465f-127">パラメーター</span><span class="sxs-lookup"><span data-stu-id="6465f-127">Parameter</span></span>    | <span data-ttu-id="6465f-128">型</span><span class="sxs-lookup"><span data-stu-id="6465f-128">Type</span></span>   |<span data-ttu-id="6465f-129">説明</span><span class="sxs-lookup"><span data-stu-id="6465f-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6465f-130">calculationType</span><span class="sxs-lookup"><span data-stu-id="6465f-130">calculationType</span></span>|<span data-ttu-id="6465f-131">文字列</span><span class="sxs-lookup"><span data-stu-id="6465f-131">string</span></span>|<span data-ttu-id="6465f-132">使用する計算の種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="6465f-132">Specifies the calculation type to use.</span></span>  <span data-ttu-id="6465f-133">可能な値は、`Recalculate`、`Full`、`FullRebuild` です。</span><span class="sxs-lookup"><span data-stu-id="6465f-133">Possible values are: `Recalculate`, `Full`, `FullRebuild`.</span></span>|

## <a name="response"></a><span data-ttu-id="6465f-134">応答</span><span class="sxs-lookup"><span data-stu-id="6465f-134">Response</span></span>

<span data-ttu-id="6465f-p105">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="6465f-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6465f-137">例</span><span class="sxs-lookup"><span data-stu-id="6465f-137">Example</span></span>
<span data-ttu-id="6465f-138">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="6465f-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="6465f-139">要求</span><span class="sxs-lookup"><span data-stu-id="6465f-139">Request</span></span>
<span data-ttu-id="6465f-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6465f-140">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="6465f-141">応答</span><span class="sxs-lookup"><span data-stu-id="6465f-141">Response</span></span>
<span data-ttu-id="6465f-142">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="6465f-142">Here is an example of the response.</span></span> 
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