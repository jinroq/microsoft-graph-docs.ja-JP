---
title: messageRule を削除する
description: 指定した messageRule オブジェクトを削除します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: ec36f8bdf9155afbd2c91734317e8652459ac895
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35890441"
---
# <a name="delete-messagerule"></a><span data-ttu-id="6522b-103">messageRule を削除する</span><span class="sxs-lookup"><span data-stu-id="6522b-103">Delete messageRule</span></span>


<span data-ttu-id="6522b-104">指定した [messageRule](../resources/messagerule.md) オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="6522b-104">Delete the specified [messageRule](../resources/messagerule.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6522b-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6522b-105">Permissions</span></span>
<span data-ttu-id="6522b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6522b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6522b-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6522b-108">Permission type</span></span>      | <span data-ttu-id="6522b-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6522b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6522b-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6522b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6522b-111">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6522b-111">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="6522b-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6522b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6522b-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6522b-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="6522b-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6522b-114">Application</span></span> | <span data-ttu-id="6522b-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6522b-115">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="6522b-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6522b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/inbox/messageRules/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/inbox/messageRules/{id}
```
## <a name="request-headers"></a><span data-ttu-id="6522b-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6522b-117">Request headers</span></span>
| <span data-ttu-id="6522b-118">名前</span><span class="sxs-lookup"><span data-stu-id="6522b-118">Name</span></span>       | <span data-ttu-id="6522b-119">説明</span><span class="sxs-lookup"><span data-stu-id="6522b-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6522b-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="6522b-120">Authorization</span></span>  | <span data-ttu-id="6522b-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6522b-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="6522b-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="6522b-123">Request body</span></span>
<span data-ttu-id="6522b-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6522b-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="6522b-125">応答</span><span class="sxs-lookup"><span data-stu-id="6522b-125">Response</span></span>
<span data-ttu-id="6522b-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="6522b-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6522b-128">例</span><span class="sxs-lookup"><span data-stu-id="6522b-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6522b-129">要求</span><span class="sxs-lookup"><span data-stu-id="6522b-129">Request</span></span>
<span data-ttu-id="6522b-130">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6522b-130">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6522b-131">プロトコル</span><span class="sxs-lookup"><span data-stu-id="6522b-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["inbox", "AQAAAJ5dZp8="],
  "name": "delete_messagerule"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messageRules/AQAAAJ5dZp8=

```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6522b-132">C#</span><span class="sxs-lookup"><span data-stu-id="6522b-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-messagerule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6522b-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="6522b-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-messagerule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6522b-134">目的-C</span><span class="sxs-lookup"><span data-stu-id="6522b-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-messagerule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="6522b-135">Java</span><span class="sxs-lookup"><span data-stu-id="6522b-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-messagerule-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6522b-136">応答</span><span class="sxs-lookup"><span data-stu-id="6522b-136">Response</span></span>
<span data-ttu-id="6522b-137">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="6522b-137">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "isEmpty": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete rule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
