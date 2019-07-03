---
title: セッションを更新する
description: 'この API を使用して、既存のブックのセッションを更新します。 '
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: bc511ad5650915c2f9c8dbeb032924710430eb44
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35448501"
---
# <a name="refresh-session"></a><span data-ttu-id="3eab7-103">セッションを更新する</span><span class="sxs-lookup"><span data-stu-id="3eab7-103">Refresh Session</span></span>

<span data-ttu-id="3eab7-104">この API を使用して、既存のブックのセッションを更新します。</span><span class="sxs-lookup"><span data-stu-id="3eab7-104">Use this API to refresh an existing workbook session.</span></span> 

## <a name="permissions"></a><span data-ttu-id="3eab7-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3eab7-105">Permissions</span></span>
<span data-ttu-id="3eab7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3eab7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3eab7-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3eab7-108">Permission type</span></span>      | <span data-ttu-id="3eab7-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3eab7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3eab7-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3eab7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3eab7-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3eab7-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3eab7-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3eab7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3eab7-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3eab7-113">Not supported.</span></span>    |
|<span data-ttu-id="3eab7-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3eab7-114">Application</span></span> | <span data-ttu-id="3eab7-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3eab7-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3eab7-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3eab7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/refreshSession
workbook-session-id: {session-id}
```
## <a name="request-headers"></a><span data-ttu-id="3eab7-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3eab7-117">Request headers</span></span>
| <span data-ttu-id="3eab7-118">名前</span><span class="sxs-lookup"><span data-stu-id="3eab7-118">Name</span></span>       | <span data-ttu-id="3eab7-119">説明</span><span class="sxs-lookup"><span data-stu-id="3eab7-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3eab7-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="3eab7-120">Authorization</span></span>  | <span data-ttu-id="3eab7-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3eab7-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3eab7-123">workbook-session-id</span><span class="sxs-lookup"><span data-stu-id="3eab7-123">workbook-session-id</span></span> | <span data-ttu-id="3eab7-124">更新するブック セッションの ID</span><span class="sxs-lookup"><span data-stu-id="3eab7-124">Workbook session Id to be refreshed</span></span> |

## <a name="request-body"></a><span data-ttu-id="3eab7-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="3eab7-125">Request body</span></span>
<span data-ttu-id="3eab7-126">この API は、要求本文を必要としません。</span><span class="sxs-lookup"><span data-stu-id="3eab7-126">This API does not require any request body.</span></span>

## <a name="response"></a><span data-ttu-id="3eab7-127">応答</span><span class="sxs-lookup"><span data-stu-id="3eab7-127">Response</span></span>

<span data-ttu-id="3eab7-128">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="3eab7-128">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3eab7-129">例</span><span class="sxs-lookup"><span data-stu-id="3eab7-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3eab7-130">要求</span><span class="sxs-lookup"><span data-stu-id="3eab7-130">Request</span></span>
<span data-ttu-id="3eab7-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3eab7-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3eab7-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="3eab7-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "refresh_excel_session"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/refreshSession
Content-type: application/json
workbook-session-id: {session-id}
Content-length: 0

{

}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3eab7-133">C#</span><span class="sxs-lookup"><span data-stu-id="3eab7-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/refresh-excel-session-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3eab7-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="3eab7-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/refresh-excel-session-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3eab7-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="3eab7-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/refresh-excel-session-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="3eab7-136">workbook-session-id ヘッダーが必要となることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="3eab7-136">Note that workbook-session-id header is required.</span></span> 


##### <a name="response"></a><span data-ttu-id="3eab7-137">応答</span><span class="sxs-lookup"><span data-stu-id="3eab7-137">Response</span></span>
<span data-ttu-id="3eab7-138">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="3eab7-138">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
