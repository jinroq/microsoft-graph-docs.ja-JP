---
title: Outlook カテゴリを削除する
description: 指定した outlookCategory オブジェクトを削除します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 482db944d3adbeb7b7d283a87dcf98973c4bc03d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949557"
---
# <a name="delete-outlook-category"></a><span data-ttu-id="b1fc0-103">Outlook カテゴリを削除する</span><span class="sxs-lookup"><span data-stu-id="b1fc0-103">Delete Outlook category</span></span>

> <span data-ttu-id="b1fc0-104">**重要**: [Microsoft Graph で/beta のバージョンの Api を選択し、プレビューでは、変更されることができます。</span><span class="sxs-lookup"><span data-stu-id="b1fc0-104">**Important**: APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b1fc0-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b1fc0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b1fc0-106">指定した [outlookCategory](../resources/outlookcategory.md) オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="b1fc0-106">Delete the specified [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b1fc0-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b1fc0-107">Permissions</span></span>
<span data-ttu-id="b1fc0-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b1fc0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1fc0-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b1fc0-110">Permission type</span></span>      | <span data-ttu-id="b1fc0-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b1fc0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b1fc0-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b1fc0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b1fc0-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b1fc0-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="b1fc0-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b1fc0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b1fc0-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b1fc0-115">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="b1fc0-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b1fc0-116">Application</span></span> | <span data-ttu-id="b1fc0-117">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b1fc0-117">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b1fc0-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b1fc0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/outlook/masterCategories/{id}
DELETE /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b1fc0-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b1fc0-119">Request headers</span></span>
| <span data-ttu-id="b1fc0-120">名前</span><span class="sxs-lookup"><span data-stu-id="b1fc0-120">Name</span></span>      |<span data-ttu-id="b1fc0-121">説明</span><span class="sxs-lookup"><span data-stu-id="b1fc0-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b1fc0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1fc0-122">Authorization</span></span>  | <span data-ttu-id="b1fc0-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b1fc0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b1fc0-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="b1fc0-125">Request body</span></span>
<span data-ttu-id="b1fc0-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b1fc0-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b1fc0-127">応答</span><span class="sxs-lookup"><span data-stu-id="b1fc0-127">Response</span></span>

<span data-ttu-id="b1fc0-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="b1fc0-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1fc0-130">例</span><span class="sxs-lookup"><span data-stu-id="b1fc0-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b1fc0-131">要求</span><span class="sxs-lookup"><span data-stu-id="b1fc0-131">Request</span></span>
<span data-ttu-id="b1fc0-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b1fc0-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_outlookcategory"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/outlook/masterCategories('4b1c2495-54c9-4a5e-90a2-0ab0b31987d8')
```
##### <a name="response"></a><span data-ttu-id="b1fc0-133">応答</span><span class="sxs-lookup"><span data-stu-id="b1fc0-133">Response</span></span>
<span data-ttu-id="b1fc0-134">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="b1fc0-134">Here is an example of the response.</span></span>
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
