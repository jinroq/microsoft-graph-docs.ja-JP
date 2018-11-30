---
title: messageRule を削除する
description: 指定した messageRule オブジェクトを削除します。
ms.openlocfilehash: 6e71372a94683292b2335e7572e6445e33faef19
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066397"
---
# <a name="delete-messagerule"></a><span data-ttu-id="8a846-103">messageRule を削除する</span><span class="sxs-lookup"><span data-stu-id="8a846-103">Delete messageRule</span></span>

> <span data-ttu-id="8a846-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8a846-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8a846-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8a846-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8a846-106">指定した [messageRule](../resources/messagerule.md) オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="8a846-106">Delete the specified [messageRule](../resources/messagerule.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8a846-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8a846-107">Permissions</span></span>
<span data-ttu-id="8a846-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8a846-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a846-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8a846-110">Permission type</span></span>      | <span data-ttu-id="8a846-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8a846-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8a846-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8a846-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8a846-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8a846-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="8a846-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8a846-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a846-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8a846-115">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="8a846-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8a846-116">Application</span></span> | <span data-ttu-id="8a846-117">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8a846-117">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8a846-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8a846-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/inbox/messagerules/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/inbox/messagerules/{id}
```
## <a name="request-headers"></a><span data-ttu-id="8a846-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8a846-119">Request headers</span></span>
| <span data-ttu-id="8a846-120">名前</span><span class="sxs-lookup"><span data-stu-id="8a846-120">Name</span></span>       | <span data-ttu-id="8a846-121">説明</span><span class="sxs-lookup"><span data-stu-id="8a846-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8a846-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8a846-122">Authorization</span></span>  | <span data-ttu-id="8a846-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8a846-p103">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="8a846-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="8a846-125">Request body</span></span>
<span data-ttu-id="8a846-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="8a846-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="8a846-127">応答</span><span class="sxs-lookup"><span data-stu-id="8a846-127">Response</span></span>
<span data-ttu-id="8a846-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="8a846-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a846-130">例</span><span class="sxs-lookup"><span data-stu-id="8a846-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8a846-131">要求</span><span class="sxs-lookup"><span data-stu-id="8a846-131">Request</span></span>
<span data-ttu-id="8a846-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8a846-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_messagerule"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/mailfolders/inbox/messagerules('AQAAAJ5dZp8=')

```
##### <a name="response"></a><span data-ttu-id="8a846-133">応答</span><span class="sxs-lookup"><span data-stu-id="8a846-133">Response</span></span>
<span data-ttu-id="8a846-134">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="8a846-134">Here is an example of the response.</span></span> 
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
  "tocPath": ""
}-->