---
title: ユーザーの削除
description: ユーザーを削除します。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e9a840f83c2bb8806464473ead09deffb30c5a9a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27969430"
---
# <a name="delete-a-user"></a><span data-ttu-id="482a5-103">ユーザーの削除</span><span class="sxs-lookup"><span data-stu-id="482a5-103">Delete a user</span></span>

> <span data-ttu-id="482a5-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="482a5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="482a5-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="482a5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="482a5-106">ユーザーを削除します。</span><span class="sxs-lookup"><span data-stu-id="482a5-106">Delete user.</span></span>
## <a name="permissions"></a><span data-ttu-id="482a5-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="482a5-107">Permissions</span></span>
<span data-ttu-id="482a5-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="482a5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="482a5-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="482a5-110">Permission type</span></span>      | <span data-ttu-id="482a5-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="482a5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="482a5-112">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="482a5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="482a5-113">User.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="482a5-113">User.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="482a5-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="482a5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="482a5-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="482a5-115">Not supported.</span></span>    |
|<span data-ttu-id="482a5-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="482a5-116">Application</span></span> | <span data-ttu-id="482a5-117">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="482a5-117">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="482a5-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="482a5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}
```

## <a name="request-headers"></a><span data-ttu-id="482a5-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="482a5-119">Request headers</span></span>
| <span data-ttu-id="482a5-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="482a5-120">Header</span></span>       | <span data-ttu-id="482a5-121">値</span><span class="sxs-lookup"><span data-stu-id="482a5-121">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="482a5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="482a5-122">Authorization</span></span>  | <span data-ttu-id="482a5-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="482a5-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="482a5-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="482a5-125">Request body</span></span>
<span data-ttu-id="482a5-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="482a5-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="482a5-127">応答</span><span class="sxs-lookup"><span data-stu-id="482a5-127">Response</span></span>

<span data-ttu-id="482a5-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="482a5-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="482a5-130">例</span><span class="sxs-lookup"><span data-stu-id="482a5-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="482a5-131">要求</span><span class="sxs-lookup"><span data-stu-id="482a5-131">Request</span></span>
<span data-ttu-id="482a5-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="482a5-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_user"
}-->
```http
DELETE https://graph.microsoft.com/beta/users/ba9a3254-9f18-4209-aeb3-9e42a35b5be4 
```
##### <a name="response"></a><span data-ttu-id="482a5-133">応答</span><span class="sxs-lookup"><span data-stu-id="482a5-133">Response</span></span>
<span data-ttu-id="482a5-134">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="482a5-134">Here is an example of the response.</span></span> 
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
