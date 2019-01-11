---
title: 'フィルター: 適用'
description: 指定した列に指定されたフィルター条件を適用します。
localization_priority: Normal
ms.openlocfilehash: 3b37344ae3047b54488fa0dd95944c0f34e3bd2b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882902"
---
# <a name="filter-apply"></a><span data-ttu-id="495c5-103">フィルター: 適用</span><span class="sxs-lookup"><span data-stu-id="495c5-103">Filter: apply</span></span>

> <span data-ttu-id="495c5-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="495c5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="495c5-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="495c5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="495c5-106">指定した列に指定されたフィルター条件を適用します。</span><span class="sxs-lookup"><span data-stu-id="495c5-106">Apply the given filter criteria on the given column.</span></span>
## <a name="permissions"></a><span data-ttu-id="495c5-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="495c5-107">Permissions</span></span>
<span data-ttu-id="495c5-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="495c5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="495c5-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="495c5-110">Permission type</span></span>      | <span data-ttu-id="495c5-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="495c5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="495c5-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="495c5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="495c5-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="495c5-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="495c5-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="495c5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="495c5-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="495c5-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="495c5-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="495c5-116">Application</span></span> | <span data-ttu-id="495c5-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="495c5-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="495c5-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="495c5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/filter/apply
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/apply

```
## <a name="request-headers"></a><span data-ttu-id="495c5-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="495c5-119">Request headers</span></span>
| <span data-ttu-id="495c5-120">名前</span><span class="sxs-lookup"><span data-stu-id="495c5-120">Name</span></span>       | <span data-ttu-id="495c5-121">説明</span><span class="sxs-lookup"><span data-stu-id="495c5-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="495c5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="495c5-122">Authorization</span></span>  | <span data-ttu-id="495c5-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="495c5-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="495c5-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="495c5-125">Request body</span></span>
<span data-ttu-id="495c5-126">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="495c5-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="495c5-127">パラメーター</span><span class="sxs-lookup"><span data-stu-id="495c5-127">Parameter</span></span>    | <span data-ttu-id="495c5-128">Type</span><span class="sxs-lookup"><span data-stu-id="495c5-128">Type</span></span>   |<span data-ttu-id="495c5-129">説明</span><span class="sxs-lookup"><span data-stu-id="495c5-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="495c5-130">criteria</span><span class="sxs-lookup"><span data-stu-id="495c5-130">criteria</span></span>|<span data-ttu-id="495c5-131">FilterCriteria</span><span class="sxs-lookup"><span data-stu-id="495c5-131">FilterCriteria</span></span>|<span data-ttu-id="495c5-132">適用する基準。</span><span class="sxs-lookup"><span data-stu-id="495c5-132">The criteria to apply.</span></span>|

## <a name="response"></a><span data-ttu-id="495c5-133">応答</span><span class="sxs-lookup"><span data-stu-id="495c5-133">Response</span></span>

<span data-ttu-id="495c5-p104">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="495c5-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="495c5-136">例</span><span class="sxs-lookup"><span data-stu-id="495c5-136">Example</span></span>
<span data-ttu-id="495c5-137">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="495c5-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="495c5-138">要求</span><span class="sxs-lookup"><span data-stu-id="495c5-138">Request</span></span>
<span data-ttu-id="495c5-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="495c5-139">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="495c5-140">応答</span><span class="sxs-lookup"><span data-stu-id="495c5-140">Response</span></span>
<span data-ttu-id="495c5-141">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="495c5-141">Here is an example of the response.</span></span> 
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
