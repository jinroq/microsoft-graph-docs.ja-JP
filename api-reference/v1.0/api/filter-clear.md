---
title: 'フィルター: クリア'
description: 指定した列のフィルターをクリアします。
ms.openlocfilehash: 85a9249cf70ffdd44b8b84e0d28bec63ca743ca1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022152"
---
# <a name="filter-clear"></a><span data-ttu-id="6e21d-103">フィルター: クリア</span><span class="sxs-lookup"><span data-stu-id="6e21d-103">Filter: clear</span></span>

<span data-ttu-id="6e21d-104">指定した列のフィルターをクリアします。</span><span class="sxs-lookup"><span data-stu-id="6e21d-104">Clear the filter on the given column.</span></span>
## <a name="permissions"></a><span data-ttu-id="6e21d-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6e21d-105">Permissions</span></span>
<span data-ttu-id="6e21d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6e21d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e21d-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6e21d-108">Permission type</span></span>      | <span data-ttu-id="6e21d-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6e21d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6e21d-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6e21d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6e21d-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6e21d-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6e21d-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6e21d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e21d-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6e21d-113">Not supported.</span></span>    |
|<span data-ttu-id="6e21d-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6e21d-114">Application</span></span> | <span data-ttu-id="6e21d-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6e21d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6e21d-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6e21d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/filter/clear
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/clear

```
## <a name="request-headers"></a><span data-ttu-id="6e21d-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6e21d-117">Request headers</span></span>
| <span data-ttu-id="6e21d-118">名前</span><span class="sxs-lookup"><span data-stu-id="6e21d-118">Name</span></span>       | <span data-ttu-id="6e21d-119">説明</span><span class="sxs-lookup"><span data-stu-id="6e21d-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6e21d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e21d-120">Authorization</span></span>  | <span data-ttu-id="6e21d-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6e21d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6e21d-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="6e21d-123">Request body</span></span>
<span data-ttu-id="6e21d-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6e21d-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6e21d-125">応答</span><span class="sxs-lookup"><span data-stu-id="6e21d-125">Response</span></span>

<span data-ttu-id="6e21d-p103">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="6e21d-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e21d-128">例</span><span class="sxs-lookup"><span data-stu-id="6e21d-128">Example</span></span>
<span data-ttu-id="6e21d-129">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="6e21d-129">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="6e21d-130">要求</span><span class="sxs-lookup"><span data-stu-id="6e21d-130">Request</span></span>
<span data-ttu-id="6e21d-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6e21d-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "filter_clear"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/clear
```

##### <a name="response"></a><span data-ttu-id="6e21d-132">応答</span><span class="sxs-lookup"><span data-stu-id="6e21d-132">Response</span></span>
<span data-ttu-id="6e21d-133">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="6e21d-133">Here is an example of the response.</span></span> 
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
  "description": "Filter: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->