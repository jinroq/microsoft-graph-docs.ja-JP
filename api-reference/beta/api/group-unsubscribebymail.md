---
title: 'グループ: unsubscribeByMail'
description: 'このメソッドを呼び出すと、現在のユーザーは、そのグループの新しい投稿、イベント、およびファイルに関するこのグループの電子メール通知を受信することを無効にします。 Office 365 グループに対してのみサポートされています。 '
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 36b6c906b2def7a1e19cdc05125ad13e94f2b39e
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36420575"
---
# <a name="group-unsubscribebymail"></a><span data-ttu-id="b0ebb-104">グループ: unsubscribeByMail</span><span class="sxs-lookup"><span data-stu-id="b0ebb-104">group: unsubscribeByMail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0ebb-105">このメソッドを呼び出すと、現在のユーザーは、そのグループの新しい投稿、イベント、およびファイルに関するこのグループの電子メール通知を受信することを無効にします。</span><span class="sxs-lookup"><span data-stu-id="b0ebb-105">Calling this method will disable the current user to receive email notifications for this group about new posts, events, and files in that group.</span></span> <span data-ttu-id="b0ebb-106">Office 365 グループに対してのみサポートされています。</span><span class="sxs-lookup"><span data-stu-id="b0ebb-106">Supported for Office 365 groups only.</span></span> 

## <a name="permissions"></a><span data-ttu-id="b0ebb-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b0ebb-107">Permissions</span></span>
<span data-ttu-id="b0ebb-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b0ebb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0ebb-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b0ebb-110">Permission type</span></span>      | <span data-ttu-id="b0ebb-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b0ebb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b0ebb-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b0ebb-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b0ebb-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0ebb-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b0ebb-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b0ebb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b0ebb-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b0ebb-115">Not supported.</span></span>    |
|<span data-ttu-id="b0ebb-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b0ebb-116">Application</span></span> | <span data-ttu-id="b0ebb-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0ebb-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b0ebb-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b0ebb-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/unsubscribeByMail
```

## <a name="request-headers"></a><span data-ttu-id="b0ebb-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b0ebb-119">Request headers</span></span>
| <span data-ttu-id="b0ebb-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b0ebb-120">Header</span></span>       | <span data-ttu-id="b0ebb-121">値</span><span class="sxs-lookup"><span data-stu-id="b0ebb-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b0ebb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0ebb-122">Authorization</span></span>  | <span data-ttu-id="b0ebb-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b0ebb-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b0ebb-125">Prefer</span><span class="sxs-lookup"><span data-stu-id="b0ebb-125">Prefer</span></span> | <span data-ttu-id="b0ebb-126">return=minimal.</span><span class="sxs-lookup"><span data-stu-id="b0ebb-126">return=minimal.</span></span> <span data-ttu-id="b0ebb-127">最小応答ヘッダーが要求ヘッダーに含まれている場合、正常な応答で `204 No Content` コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="b0ebb-127">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="b0ebb-128">省略可能。</span><span class="sxs-lookup"><span data-stu-id="b0ebb-128">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="b0ebb-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="b0ebb-129">Request body</span></span>
 <span data-ttu-id="b0ebb-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b0ebb-130">Do not supply a request body for this method.</span></span> 

## <a name="response"></a><span data-ttu-id="b0ebb-131">応答</span><span class="sxs-lookup"><span data-stu-id="b0ebb-131">Response</span></span>
<span data-ttu-id="b0ebb-p106">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="b0ebb-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0ebb-134">例</span><span class="sxs-lookup"><span data-stu-id="b0ebb-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="b0ebb-135">要求</span><span class="sxs-lookup"><span data-stu-id="b0ebb-135">Request</span></span>
<span data-ttu-id="b0ebb-136">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b0ebb-136">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b0ebb-137">プロトコル</span><span class="sxs-lookup"><span data-stu-id="b0ebb-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_unsubscribebymail"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/unsubscribeByMail
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b0ebb-138">C#</span><span class="sxs-lookup"><span data-stu-id="b0ebb-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-unsubscribebymail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b0ebb-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b0ebb-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-unsubscribebymail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b0ebb-140">目的-C</span><span class="sxs-lookup"><span data-stu-id="b0ebb-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-unsubscribebymail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b0ebb-141">応答</span><span class="sxs-lookup"><span data-stu-id="b0ebb-141">Response</span></span>
<span data-ttu-id="b0ebb-142">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b0ebb-142">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "group: unsubscribeByMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
