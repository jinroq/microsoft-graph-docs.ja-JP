---
title: 'RangeFormat: autofitRows'
description: 現在の列のデータに基づいて、現在の範囲の行の高さを最適な高さに変更します。
ms.openlocfilehash: 8aa8f47f1bea169cf8d72d386ced207953f08f2c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024286"
---
# <a name="rangeformat-autofitrows"></a><span data-ttu-id="5a66e-103">RangeFormat: autofitRows</span><span class="sxs-lookup"><span data-stu-id="5a66e-103">RangeFormat: autofitRows</span></span>

<span data-ttu-id="5a66e-104">現在の列のデータに基づいて、現在の範囲の行の高さを最適な高さに変更します。</span><span class="sxs-lookup"><span data-stu-id="5a66e-104">Changes the height of the rows of the current range to achieve the best fit, based on the current data in the columns.</span></span>
## <a name="permissions"></a><span data-ttu-id="5a66e-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5a66e-105">Permissions</span></span>
<span data-ttu-id="5a66e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5a66e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a66e-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5a66e-108">Permission type</span></span>      | <span data-ttu-id="5a66e-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5a66e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5a66e-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5a66e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5a66e-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a66e-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5a66e-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5a66e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5a66e-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5a66e-113">Not supported.</span></span>    |
|<span data-ttu-id="5a66e-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5a66e-114">Application</span></span> | <span data-ttu-id="5a66e-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5a66e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5a66e-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5a66e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/format/autofitRows
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/autofitRows
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/autofitRows

```
## <a name="request-headers"></a><span data-ttu-id="5a66e-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5a66e-117">Request headers</span></span>
| <span data-ttu-id="5a66e-118">名前</span><span class="sxs-lookup"><span data-stu-id="5a66e-118">Name</span></span>       | <span data-ttu-id="5a66e-119">説明</span><span class="sxs-lookup"><span data-stu-id="5a66e-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5a66e-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a66e-120">Authorization</span></span>  | <span data-ttu-id="5a66e-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5a66e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5a66e-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="5a66e-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="5a66e-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="5a66e-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5a66e-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="5a66e-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="5a66e-127">応答</span><span class="sxs-lookup"><span data-stu-id="5a66e-127">Response</span></span>

<span data-ttu-id="5a66e-p104">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="5a66e-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a66e-130">例</span><span class="sxs-lookup"><span data-stu-id="5a66e-130">Example</span></span>
<span data-ttu-id="5a66e-131">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="5a66e-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5a66e-132">要求</span><span class="sxs-lookup"><span data-stu-id="5a66e-132">Request</span></span>
<span data-ttu-id="5a66e-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5a66e-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "rangeformat_autofitrows"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/autofitRows
```

##### <a name="response"></a><span data-ttu-id="5a66e-134">応答</span><span class="sxs-lookup"><span data-stu-id="5a66e-134">Response</span></span>
<span data-ttu-id="5a66e-135">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="5a66e-135">Here is an example of the response.</span></span> 
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
  "description": "RangeFormat: autofitRows",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->