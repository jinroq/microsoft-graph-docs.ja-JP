---
title: 'フィルター: 適用'
description: 指定した列に指定されたフィルター条件を適用します。
ms.openlocfilehash: e799b4e4b5f94664e9420e810075205691e1bd96
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066356"
---
# <a name="filter-apply"></a><span data-ttu-id="ec5d0-103">フィルター: 適用</span><span class="sxs-lookup"><span data-stu-id="ec5d0-103">Filter: apply</span></span>

> <span data-ttu-id="ec5d0-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ec5d0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ec5d0-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ec5d0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ec5d0-106">指定した列に指定されたフィルター条件を適用します。</span><span class="sxs-lookup"><span data-stu-id="ec5d0-106">Apply the given filter criteria on the given column.</span></span>
## <a name="permissions"></a><span data-ttu-id="ec5d0-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ec5d0-107">Permissions</span></span>
<span data-ttu-id="ec5d0-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ec5d0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec5d0-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ec5d0-110">Permission type</span></span>      | <span data-ttu-id="ec5d0-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ec5d0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ec5d0-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ec5d0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ec5d0-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ec5d0-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ec5d0-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ec5d0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec5d0-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ec5d0-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ec5d0-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ec5d0-116">Application</span></span> | <span data-ttu-id="ec5d0-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ec5d0-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ec5d0-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ec5d0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/filter/apply
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/apply

```
## <a name="request-headers"></a><span data-ttu-id="ec5d0-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ec5d0-119">Request headers</span></span>
| <span data-ttu-id="ec5d0-120">名前</span><span class="sxs-lookup"><span data-stu-id="ec5d0-120">Name</span></span>       | <span data-ttu-id="ec5d0-121">説明</span><span class="sxs-lookup"><span data-stu-id="ec5d0-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ec5d0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ec5d0-122">Authorization</span></span>  | <span data-ttu-id="ec5d0-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ec5d0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ec5d0-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="ec5d0-125">Request body</span></span>
<span data-ttu-id="ec5d0-126">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="ec5d0-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ec5d0-127">パラメーター</span><span class="sxs-lookup"><span data-stu-id="ec5d0-127">Parameter</span></span>    | <span data-ttu-id="ec5d0-128">型</span><span class="sxs-lookup"><span data-stu-id="ec5d0-128">Type</span></span>   |<span data-ttu-id="ec5d0-129">説明</span><span class="sxs-lookup"><span data-stu-id="ec5d0-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ec5d0-130">criteria</span><span class="sxs-lookup"><span data-stu-id="ec5d0-130">criteria</span></span>|<span data-ttu-id="ec5d0-131">FilterCriteria</span><span class="sxs-lookup"><span data-stu-id="ec5d0-131">FilterCriteria</span></span>|<span data-ttu-id="ec5d0-132">適用する基準。</span><span class="sxs-lookup"><span data-stu-id="ec5d0-132">The criteria to apply.</span></span>|

## <a name="response"></a><span data-ttu-id="ec5d0-133">応答</span><span class="sxs-lookup"><span data-stu-id="ec5d0-133">Response</span></span>

<span data-ttu-id="ec5d0-p104">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="ec5d0-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec5d0-136">例</span><span class="sxs-lookup"><span data-stu-id="ec5d0-136">Example</span></span>
<span data-ttu-id="ec5d0-137">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="ec5d0-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ec5d0-138">要求</span><span class="sxs-lookup"><span data-stu-id="ec5d0-138">Request</span></span>
<span data-ttu-id="ec5d0-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ec5d0-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "filter_apply"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/apply
Content-type: application/json
Content-length: 321

{
  "criteria": {
    "criterion1": "criterion1-value",
    "criterion2": "criterion2-value",
    "color": "color-value",
    "operator": {
    },
    "icon": {
      "set": "set-value",
      "index": 99
    },
    "dynamicCriteria": "dynamicCriteria-value",
    "values": {
    },
    "filterOn": "filterOn-value"
  }
}
```

##### <a name="response"></a><span data-ttu-id="ec5d0-140">応答</span><span class="sxs-lookup"><span data-stu-id="ec5d0-140">Response</span></span>
<span data-ttu-id="ec5d0-141">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="ec5d0-141">Here is an example of the response.</span></span> 
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
  "description": "Filter: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->