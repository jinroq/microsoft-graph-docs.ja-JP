---
title: Delete contactFolder
description: 既定の contactFolder 以外の contactFolder を削除します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: f15cf3e08c01e7bf622fa17dd8ce59017ddb4f8c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566228"
---
# <a name="delete-contactfolder"></a><span data-ttu-id="1b37d-103">Delete contactFolder</span><span class="sxs-lookup"><span data-stu-id="1b37d-103">Delete contactFolder</span></span>

<span data-ttu-id="1b37d-104">既定の contactFolder 以外の contactFolder を削除します。</span><span class="sxs-lookup"><span data-stu-id="1b37d-104">Delete contactFolder other than the default contactFolder.</span></span>
## <a name="permissions"></a><span data-ttu-id="1b37d-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1b37d-105">Permissions</span></span>
<span data-ttu-id="1b37d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1b37d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b37d-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1b37d-108">Permission type</span></span>      | <span data-ttu-id="1b37d-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1b37d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1b37d-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1b37d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1b37d-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1b37d-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="1b37d-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1b37d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b37d-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1b37d-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="1b37d-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1b37d-114">Application</span></span> | <span data-ttu-id="1b37d-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1b37d-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="1b37d-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1b37d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/contactFolders/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="1b37d-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1b37d-117">Request headers</span></span>
| <span data-ttu-id="1b37d-118">名前</span><span class="sxs-lookup"><span data-stu-id="1b37d-118">Name</span></span>       | <span data-ttu-id="1b37d-119">型</span><span class="sxs-lookup"><span data-stu-id="1b37d-119">Type</span></span> | <span data-ttu-id="1b37d-120">説明</span><span class="sxs-lookup"><span data-stu-id="1b37d-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1b37d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1b37d-121">Authorization</span></span>  | <span data-ttu-id="1b37d-122">string</span><span class="sxs-lookup"><span data-stu-id="1b37d-122">string</span></span>  | <span data-ttu-id="1b37d-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1b37d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1b37d-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="1b37d-125">Request body</span></span>
<span data-ttu-id="1b37d-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1b37d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1b37d-127">応答</span><span class="sxs-lookup"><span data-stu-id="1b37d-127">Response</span></span>

<span data-ttu-id="1b37d-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="1b37d-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b37d-130">例</span><span class="sxs-lookup"><span data-stu-id="1b37d-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1b37d-131">要求</span><span class="sxs-lookup"><span data-stu-id="1b37d-131">Request</span></span>
<span data-ttu-id="1b37d-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1b37d-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_contactfolder"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/contactFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="1b37d-133">応答</span><span class="sxs-lookup"><span data-stu-id="1b37d-133">Response</span></span>
<span data-ttu-id="1b37d-134">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="1b37d-134">Here is an example of the response.</span></span> 
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
