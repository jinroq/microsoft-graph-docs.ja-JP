---
title: 'フィルター: 適用'
description: 指定した列に指定されたフィルター条件を適用します。
localization_priority: Normal
ms.openlocfilehash: e7223c1b3d7cd75356c459f366c1a230eeb06e59
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32524261"
---
# <a name="filter-apply"></a><span data-ttu-id="80e68-103">フィルター: 適用</span><span class="sxs-lookup"><span data-stu-id="80e68-103">Filter: apply</span></span>

<span data-ttu-id="80e68-104">指定した列に指定されたフィルター条件を適用します。</span><span class="sxs-lookup"><span data-stu-id="80e68-104">Apply the given filter criteria on the given column.</span></span>
## <a name="permissions"></a><span data-ttu-id="80e68-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="80e68-105">Permissions</span></span>
<span data-ttu-id="80e68-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="80e68-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80e68-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="80e68-108">Permission type</span></span>      | <span data-ttu-id="80e68-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="80e68-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="80e68-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="80e68-110">Delegated (work or school account)</span></span> | <span data-ttu-id="80e68-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="80e68-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="80e68-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="80e68-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="80e68-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="80e68-113">Not supported.</span></span>    |
|<span data-ttu-id="80e68-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="80e68-114">Application</span></span> | <span data-ttu-id="80e68-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="80e68-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="80e68-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="80e68-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/filter/apply
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/apply

```
## <a name="request-headers"></a><span data-ttu-id="80e68-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="80e68-117">Request headers</span></span>
| <span data-ttu-id="80e68-118">名前</span><span class="sxs-lookup"><span data-stu-id="80e68-118">Name</span></span>       | <span data-ttu-id="80e68-119">説明</span><span class="sxs-lookup"><span data-stu-id="80e68-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="80e68-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="80e68-120">Authorization</span></span>  | <span data-ttu-id="80e68-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="80e68-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="80e68-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="80e68-123">Request body</span></span>
<span data-ttu-id="80e68-124">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="80e68-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="80e68-125">パラメーター</span><span class="sxs-lookup"><span data-stu-id="80e68-125">Parameter</span></span>    | <span data-ttu-id="80e68-126">型</span><span class="sxs-lookup"><span data-stu-id="80e68-126">Type</span></span>   |<span data-ttu-id="80e68-127">説明</span><span class="sxs-lookup"><span data-stu-id="80e68-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="80e68-128">criteria</span><span class="sxs-lookup"><span data-stu-id="80e68-128">criteria</span></span>|<span data-ttu-id="80e68-129">WorkbookFilterCriteria</span><span class="sxs-lookup"><span data-stu-id="80e68-129">WorkbookFilterCriteria</span></span>|<span data-ttu-id="80e68-130">適用する基準。</span><span class="sxs-lookup"><span data-stu-id="80e68-130">The criteria to apply.</span></span>|

## <a name="response"></a><span data-ttu-id="80e68-131">応答</span><span class="sxs-lookup"><span data-stu-id="80e68-131">Response</span></span>

<span data-ttu-id="80e68-p103">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="80e68-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80e68-134">例</span><span class="sxs-lookup"><span data-stu-id="80e68-134">Example</span></span>
<span data-ttu-id="80e68-135">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="80e68-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="80e68-136">要求</span><span class="sxs-lookup"><span data-stu-id="80e68-136">Request</span></span>
<span data-ttu-id="80e68-137">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="80e68-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "filter_apply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/apply
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

##### <a name="response"></a><span data-ttu-id="80e68-138">応答</span><span class="sxs-lookup"><span data-stu-id="80e68-138">Response</span></span>
<span data-ttu-id="80e68-139">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="80e68-139">Here is an example of the response.</span></span> 
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
  "description": "Filter: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
