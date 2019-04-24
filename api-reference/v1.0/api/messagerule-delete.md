---
title: messageRule を削除する
description: 指定した messageRule オブジェクトを削除します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 570970296444b5bb4d5033bf26a03214d9fa8dac
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32585217"
---
# <a name="delete-messagerule"></a><span data-ttu-id="818c5-103">messageRule を削除する</span><span class="sxs-lookup"><span data-stu-id="818c5-103">Delete messageRule</span></span>


<span data-ttu-id="818c5-104">指定した [messageRule](../resources/messagerule.md) オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="818c5-104">Delete the specified [messageRule](../resources/messagerule.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="818c5-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="818c5-105">Permissions</span></span>
<span data-ttu-id="818c5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="818c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="818c5-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="818c5-108">Permission type</span></span>      | <span data-ttu-id="818c5-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="818c5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="818c5-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="818c5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="818c5-111">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="818c5-111">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="818c5-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="818c5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="818c5-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="818c5-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="818c5-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="818c5-114">Application</span></span> | <span data-ttu-id="818c5-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="818c5-115">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="818c5-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="818c5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/inbox/messageRules/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/inbox/messageRules/{id}
```
## <a name="request-headers"></a><span data-ttu-id="818c5-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="818c5-117">Request headers</span></span>
| <span data-ttu-id="818c5-118">名前</span><span class="sxs-lookup"><span data-stu-id="818c5-118">Name</span></span>       | <span data-ttu-id="818c5-119">説明</span><span class="sxs-lookup"><span data-stu-id="818c5-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="818c5-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="818c5-120">Authorization</span></span>  | <span data-ttu-id="818c5-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="818c5-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="818c5-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="818c5-123">Request body</span></span>
<span data-ttu-id="818c5-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="818c5-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="818c5-125">応答</span><span class="sxs-lookup"><span data-stu-id="818c5-125">Response</span></span>
<span data-ttu-id="818c5-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="818c5-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="818c5-128">例</span><span class="sxs-lookup"><span data-stu-id="818c5-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="818c5-129">要求</span><span class="sxs-lookup"><span data-stu-id="818c5-129">Request</span></span>
<span data-ttu-id="818c5-130">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="818c5-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["inbox", "AQAAAJ5dZp8="],
  "name": "delete_messagerule"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messageRules/AQAAAJ5dZp8=

```
##### <a name="response"></a><span data-ttu-id="818c5-131">応答</span><span class="sxs-lookup"><span data-stu-id="818c5-131">Response</span></span>
<span data-ttu-id="818c5-132">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="818c5-132">Here is an example of the response.</span></span> 
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
