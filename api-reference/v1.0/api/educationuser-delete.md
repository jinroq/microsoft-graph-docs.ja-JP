---
title: educationUser を削除する
description: ユーザーを削除します。
ms.openlocfilehash: d9e3cab7d34cdf418b3553d69881bb951217ae22
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021267"
---
# <a name="delete-educationuser"></a><span data-ttu-id="2b42b-103">educationUser を削除する</span><span class="sxs-lookup"><span data-stu-id="2b42b-103">Delete educationUser</span></span>

<span data-ttu-id="2b42b-104">ユーザーを削除します。</span><span class="sxs-lookup"><span data-stu-id="2b42b-104">Delete a user.</span></span>


## <a name="permissions"></a><span data-ttu-id="2b42b-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2b42b-105">Permissions</span></span>
<span data-ttu-id="2b42b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2b42b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b42b-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2b42b-108">Permission type</span></span>      | <span data-ttu-id="2b42b-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2b42b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2b42b-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2b42b-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="2b42b-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2b42b-111">Not supported.</span></span>  |
|<span data-ttu-id="2b42b-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2b42b-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="2b42b-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2b42b-113">Not supported.</span></span>  |
|<span data-ttu-id="2b42b-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2b42b-114">Application</span></span> | <span data-ttu-id="2b42b-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b42b-115">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2b42b-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2b42b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/users/{id}
```
## <a name="request-headers"></a><span data-ttu-id="2b42b-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2b42b-117">Request headers</span></span>
| <span data-ttu-id="2b42b-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2b42b-118">Header</span></span>       | <span data-ttu-id="2b42b-119">値</span><span class="sxs-lookup"><span data-stu-id="2b42b-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2b42b-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b42b-120">Authorization</span></span>  | <span data-ttu-id="2b42b-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2b42b-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2b42b-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="2b42b-123">Request body</span></span>
<span data-ttu-id="2b42b-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2b42b-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="2b42b-125">応答</span><span class="sxs-lookup"><span data-stu-id="2b42b-125">Response</span></span>
<span data-ttu-id="2b42b-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="2b42b-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b42b-128">例</span><span class="sxs-lookup"><span data-stu-id="2b42b-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2b42b-129">要求</span><span class="sxs-lookup"><span data-stu-id="2b42b-129">Request</span></span>
<span data-ttu-id="2b42b-130">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2b42b-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationuser"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/users/{user-id}
```
##### <a name="response"></a><span data-ttu-id="2b42b-131">応答</span><span class="sxs-lookup"><span data-stu-id="2b42b-131">Response</span></span>
<span data-ttu-id="2b42b-132">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2b42b-132">The following is an example of the response.</span></span> 
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
  "description": "Delete educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->