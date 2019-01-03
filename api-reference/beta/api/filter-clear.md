---
title: 'フィルター: クリア'
description: 指定した列のフィルターをクリアします。
ms.openlocfilehash: ae71723ed3ca9074bb7a71ea131fd7103f3714af
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068248"
---
# <a name="filter-clear"></a><span data-ttu-id="58d3c-103">フィルター: クリア</span><span class="sxs-lookup"><span data-stu-id="58d3c-103">Filter: clear</span></span>

> <span data-ttu-id="58d3c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="58d3c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="58d3c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="58d3c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="58d3c-106">指定した列のフィルターをクリアします。</span><span class="sxs-lookup"><span data-stu-id="58d3c-106">Clear the filter on the given column.</span></span>
## <a name="permissions"></a><span data-ttu-id="58d3c-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="58d3c-107">Permissions</span></span>
<span data-ttu-id="58d3c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="58d3c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58d3c-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="58d3c-110">Permission type</span></span>      | <span data-ttu-id="58d3c-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="58d3c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="58d3c-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="58d3c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="58d3c-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="58d3c-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="58d3c-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="58d3c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58d3c-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="58d3c-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="58d3c-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="58d3c-116">Application</span></span> | <span data-ttu-id="58d3c-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="58d3c-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="58d3c-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="58d3c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/filter/clear
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/clear

```
## <a name="request-headers"></a><span data-ttu-id="58d3c-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="58d3c-119">Request headers</span></span>
| <span data-ttu-id="58d3c-120">名前</span><span class="sxs-lookup"><span data-stu-id="58d3c-120">Name</span></span>       | <span data-ttu-id="58d3c-121">説明</span><span class="sxs-lookup"><span data-stu-id="58d3c-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="58d3c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="58d3c-122">Authorization</span></span>  | <span data-ttu-id="58d3c-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="58d3c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="58d3c-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="58d3c-125">Request body</span></span>

## <a name="response"></a><span data-ttu-id="58d3c-126">応答</span><span class="sxs-lookup"><span data-stu-id="58d3c-126">Response</span></span>

<span data-ttu-id="58d3c-p104">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="58d3c-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58d3c-129">例</span><span class="sxs-lookup"><span data-stu-id="58d3c-129">Example</span></span>
<span data-ttu-id="58d3c-130">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="58d3c-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="58d3c-131">要求</span><span class="sxs-lookup"><span data-stu-id="58d3c-131">Request</span></span>
<span data-ttu-id="58d3c-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="58d3c-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "filter_clear"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/clear
```

##### <a name="response"></a><span data-ttu-id="58d3c-133">応答</span><span class="sxs-lookup"><span data-stu-id="58d3c-133">Response</span></span>
<span data-ttu-id="58d3c-134">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="58d3c-134">Here is an example of the response.</span></span> 
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
  "description": "Filter: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->