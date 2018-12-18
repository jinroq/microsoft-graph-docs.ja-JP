---
title: ユーザーの削除
description: ユーザーを削除します。
author: dkershaw10
ms.openlocfilehash: 44e0439a95b0104472101b43adfae39b2c553d58
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301177"
---
# <a name="delete-a-user"></a><span data-ttu-id="4153a-103">ユーザーの削除</span><span class="sxs-lookup"><span data-stu-id="4153a-103">Delete a user</span></span>

<span data-ttu-id="4153a-104">ユーザーを削除します。</span><span class="sxs-lookup"><span data-stu-id="4153a-104">Delete user.</span></span>
## <a name="permissions"></a><span data-ttu-id="4153a-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4153a-105">Permissions</span></span>
<span data-ttu-id="4153a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4153a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4153a-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4153a-108">Permission type</span></span>      | <span data-ttu-id="4153a-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4153a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4153a-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4153a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4153a-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4153a-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4153a-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4153a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4153a-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4153a-113">Not supported.</span></span>    |
|<span data-ttu-id="4153a-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4153a-114">Application</span></span> | <span data-ttu-id="4153a-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4153a-115">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4153a-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4153a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}
```

## <a name="request-headers"></a><span data-ttu-id="4153a-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4153a-117">Request headers</span></span>
| <span data-ttu-id="4153a-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4153a-118">Header</span></span>       | <span data-ttu-id="4153a-119">値</span><span class="sxs-lookup"><span data-stu-id="4153a-119">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="4153a-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="4153a-120">Authorization</span></span>  | <span data-ttu-id="4153a-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4153a-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4153a-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="4153a-123">Request body</span></span>
<span data-ttu-id="4153a-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="4153a-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4153a-125">応答</span><span class="sxs-lookup"><span data-stu-id="4153a-125">Response</span></span>

<span data-ttu-id="4153a-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="4153a-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4153a-128">例</span><span class="sxs-lookup"><span data-stu-id="4153a-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4153a-129">要求</span><span class="sxs-lookup"><span data-stu-id="4153a-129">Request</span></span>
<span data-ttu-id="4153a-130">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4153a-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_user"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/users/{user-id}
```
##### <a name="response"></a><span data-ttu-id="4153a-131">応答</span><span class="sxs-lookup"><span data-stu-id="4153a-131">Response</span></span>
<span data-ttu-id="4153a-132">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="4153a-132">Here is an example of the response.</span></span> 
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
  "description": "Delete user",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->