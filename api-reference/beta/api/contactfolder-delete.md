---
title: Delete contactFolder
description: 既定の contactFolder 以外の contactFolder を削除します。
author: angelgolfer-ms
ms.openlocfilehash: 26ff5f9a2ef78d33fd60b498e891f031891b6f17
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334014"
---
# <a name="delete-contactfolder"></a><span data-ttu-id="23982-103">Delete contactFolder</span><span class="sxs-lookup"><span data-stu-id="23982-103">Delete contactFolder</span></span>

> <span data-ttu-id="23982-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="23982-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="23982-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="23982-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="23982-106">既定の contactFolder 以外の contactFolder を削除します。</span><span class="sxs-lookup"><span data-stu-id="23982-106">Delete contactFolder other than the default contactFolder.</span></span>
## <a name="permissions"></a><span data-ttu-id="23982-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="23982-107">Permissions</span></span>
<span data-ttu-id="23982-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="23982-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23982-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="23982-110">Permission type</span></span>      | <span data-ttu-id="23982-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="23982-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="23982-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="23982-112">Delegated (work or school account)</span></span> | <span data-ttu-id="23982-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="23982-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="23982-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="23982-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23982-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="23982-115">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="23982-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="23982-116">Application</span></span> | <span data-ttu-id="23982-117">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="23982-117">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="23982-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="23982-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/contactFolders/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="23982-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="23982-119">Request headers</span></span>
| <span data-ttu-id="23982-120">名前</span><span class="sxs-lookup"><span data-stu-id="23982-120">Name</span></span>       | <span data-ttu-id="23982-121">種類</span><span class="sxs-lookup"><span data-stu-id="23982-121">Type</span></span> | <span data-ttu-id="23982-122">説明</span><span class="sxs-lookup"><span data-stu-id="23982-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="23982-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="23982-123">Authorization</span></span>  | <span data-ttu-id="23982-124">string</span><span class="sxs-lookup"><span data-stu-id="23982-124">string</span></span>  | <span data-ttu-id="23982-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="23982-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="23982-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="23982-127">Request body</span></span>
<span data-ttu-id="23982-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="23982-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="23982-129">応答</span><span class="sxs-lookup"><span data-stu-id="23982-129">Response</span></span>

<span data-ttu-id="23982-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="23982-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23982-132">例</span><span class="sxs-lookup"><span data-stu-id="23982-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="23982-133">要求</span><span class="sxs-lookup"><span data-stu-id="23982-133">Request</span></span>
<span data-ttu-id="23982-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="23982-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_contactfolder"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/contactFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="23982-135">応答</span><span class="sxs-lookup"><span data-stu-id="23982-135">Response</span></span>
<span data-ttu-id="23982-136">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="23982-136">Here is an example of the response.</span></span> 
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
  "description": "Delete contactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->