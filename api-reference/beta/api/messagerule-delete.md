---
title: messageRule を削除する
description: 指定した messageRule オブジェクトを削除します。
author: angelgolfer-ms
ms.openlocfilehash: e10cebf6b2758a21a8bf70e505edcebb7f27082c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27305377"
---
# <a name="delete-messagerule"></a><span data-ttu-id="c34fd-103">messageRule を削除する</span><span class="sxs-lookup"><span data-stu-id="c34fd-103">Delete messageRule</span></span>

> <span data-ttu-id="c34fd-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c34fd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c34fd-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c34fd-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c34fd-106">指定した [messageRule](../resources/messagerule.md) オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="c34fd-106">Delete the specified [messageRule](../resources/messagerule.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c34fd-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c34fd-107">Permissions</span></span>
<span data-ttu-id="c34fd-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c34fd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c34fd-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c34fd-110">Permission type</span></span>      | <span data-ttu-id="c34fd-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c34fd-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c34fd-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c34fd-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c34fd-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c34fd-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="c34fd-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c34fd-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c34fd-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c34fd-115">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="c34fd-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c34fd-116">Application</span></span> | <span data-ttu-id="c34fd-117">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c34fd-117">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c34fd-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c34fd-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/inbox/messagerules/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/inbox/messagerules/{id}
```
## <a name="request-headers"></a><span data-ttu-id="c34fd-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c34fd-119">Request headers</span></span>
| <span data-ttu-id="c34fd-120">名前</span><span class="sxs-lookup"><span data-stu-id="c34fd-120">Name</span></span>       | <span data-ttu-id="c34fd-121">説明</span><span class="sxs-lookup"><span data-stu-id="c34fd-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c34fd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c34fd-122">Authorization</span></span>  | <span data-ttu-id="c34fd-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c34fd-p103">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="c34fd-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="c34fd-125">Request body</span></span>
<span data-ttu-id="c34fd-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c34fd-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="c34fd-127">応答</span><span class="sxs-lookup"><span data-stu-id="c34fd-127">Response</span></span>
<span data-ttu-id="c34fd-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="c34fd-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c34fd-130">例</span><span class="sxs-lookup"><span data-stu-id="c34fd-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c34fd-131">要求</span><span class="sxs-lookup"><span data-stu-id="c34fd-131">Request</span></span>
<span data-ttu-id="c34fd-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c34fd-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_messagerule"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/mailfolders/inbox/messagerules('AQAAAJ5dZp8=')

```
##### <a name="response"></a><span data-ttu-id="c34fd-133">応答</span><span class="sxs-lookup"><span data-stu-id="c34fd-133">Response</span></span>
<span data-ttu-id="c34fd-134">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="c34fd-134">Here is an example of the response.</span></span> 
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