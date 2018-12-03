---
title: Outlook カテゴリを削除する
description: 指定した outlookCategory オブジェクトを削除します。
ms.openlocfilehash: a240df167918892face0da8932af0f2ff3d23152
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068333"
---
# <a name="delete-outlook-category"></a><span data-ttu-id="0dfbf-103">Outlook カテゴリを削除する</span><span class="sxs-lookup"><span data-stu-id="0dfbf-103">Delete Outlook category</span></span>

> <span data-ttu-id="0dfbf-104">**重要**: [Microsoft Graph で/beta のバージョンの Api を選択し、プレビューでは、変更されることができます。</span><span class="sxs-lookup"><span data-stu-id="0dfbf-104">**Important**: APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0dfbf-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0dfbf-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0dfbf-106">指定した [outlookCategory](../resources/outlookcategory.md) オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="0dfbf-106">Delete the specified [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0dfbf-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0dfbf-107">Permissions</span></span>
<span data-ttu-id="0dfbf-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0dfbf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0dfbf-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0dfbf-110">Permission type</span></span>      | <span data-ttu-id="0dfbf-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0dfbf-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0dfbf-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0dfbf-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0dfbf-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0dfbf-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="0dfbf-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0dfbf-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0dfbf-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0dfbf-115">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="0dfbf-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0dfbf-116">Application</span></span> | <span data-ttu-id="0dfbf-117">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0dfbf-117">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="0dfbf-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0dfbf-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/outlook/masterCategories/{id}
DELETE /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0dfbf-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="0dfbf-119">Optional query parameters</span></span>
<span data-ttu-id="0dfbf-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="0dfbf-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0dfbf-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0dfbf-121">Request headers</span></span>
| <span data-ttu-id="0dfbf-122">名前</span><span class="sxs-lookup"><span data-stu-id="0dfbf-122">Name</span></span>      |<span data-ttu-id="0dfbf-123">説明</span><span class="sxs-lookup"><span data-stu-id="0dfbf-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0dfbf-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0dfbf-124">Authorization</span></span>  | <span data-ttu-id="0dfbf-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0dfbf-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0dfbf-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="0dfbf-127">Request body</span></span>
<span data-ttu-id="0dfbf-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="0dfbf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0dfbf-129">応答</span><span class="sxs-lookup"><span data-stu-id="0dfbf-129">Response</span></span>

<span data-ttu-id="0dfbf-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="0dfbf-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0dfbf-132">例</span><span class="sxs-lookup"><span data-stu-id="0dfbf-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0dfbf-133">要求</span><span class="sxs-lookup"><span data-stu-id="0dfbf-133">Request</span></span>
<span data-ttu-id="0dfbf-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0dfbf-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_outlookcategory"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/outlook/masterCategories('4b1c2495-54c9-4a5e-90a2-0ab0b31987d8')
```
##### <a name="response"></a><span data-ttu-id="0dfbf-135">応答</span><span class="sxs-lookup"><span data-stu-id="0dfbf-135">Response</span></span>
<span data-ttu-id="0dfbf-136">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="0dfbf-136">Here is an example of the response.</span></span>
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