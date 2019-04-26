---
title: Outlook カテゴリを削除する
description: 指定した outlookCategory オブジェクトを削除します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 5c909176634d64245d5ff5521c0da68b02e8777b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561370"
---
# <a name="delete-outlook-category"></a><span data-ttu-id="6ec1f-103">Outlook カテゴリを削除する</span><span class="sxs-lookup"><span data-stu-id="6ec1f-103">Delete Outlook category</span></span>


<span data-ttu-id="6ec1f-104">指定した [outlookCategory](../resources/outlookcategory.md) オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="6ec1f-104">Delete the specified [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6ec1f-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6ec1f-105">Permissions</span></span>
<span data-ttu-id="6ec1f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6ec1f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ec1f-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6ec1f-108">Permission type</span></span>      | <span data-ttu-id="6ec1f-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6ec1f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6ec1f-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6ec1f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6ec1f-111">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6ec1f-111">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="6ec1f-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6ec1f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6ec1f-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6ec1f-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="6ec1f-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6ec1f-114">Application</span></span> | <span data-ttu-id="6ec1f-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6ec1f-115">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="6ec1f-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6ec1f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/outlook/masterCategories/{id}
DELETE /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6ec1f-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6ec1f-117">Request headers</span></span>
| <span data-ttu-id="6ec1f-118">名前</span><span class="sxs-lookup"><span data-stu-id="6ec1f-118">Name</span></span>      |<span data-ttu-id="6ec1f-119">説明</span><span class="sxs-lookup"><span data-stu-id="6ec1f-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6ec1f-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="6ec1f-120">Authorization</span></span>  | <span data-ttu-id="6ec1f-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6ec1f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6ec1f-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="6ec1f-123">Request body</span></span>
<span data-ttu-id="6ec1f-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6ec1f-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6ec1f-125">応答</span><span class="sxs-lookup"><span data-stu-id="6ec1f-125">Response</span></span>

<span data-ttu-id="6ec1f-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="6ec1f-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ec1f-128">例</span><span class="sxs-lookup"><span data-stu-id="6ec1f-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6ec1f-129">要求</span><span class="sxs-lookup"><span data-stu-id="6ec1f-129">Request</span></span>
<span data-ttu-id="6ec1f-130">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6ec1f-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["4b1c2495-54c9-4a5e-90a2-0ab0b31987d8"],
  "name": "delete_outlookcategory"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/outlook/masterCategories/4b1c2495-54c9-4a5e-90a2-0ab0b31987d8
```
##### <a name="response"></a><span data-ttu-id="6ec1f-131">応答</span><span class="sxs-lookup"><span data-stu-id="6ec1f-131">Response</span></span>
<span data-ttu-id="6ec1f-132">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="6ec1f-132">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "name": "delete_outlookcategory",
  "isEmpty": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
