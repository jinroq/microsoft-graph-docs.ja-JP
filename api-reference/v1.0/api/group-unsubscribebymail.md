---
title: 'グループ: unsubscribeByMail'
description: 'このメソッドを呼び出すと、現在のユーザーがそのグループ内の新規投稿、イベント、およびファイルに関するメール通知を受信しなくなります。Office 365 のグループのみをサポートします。 '
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 466df028ac2f65df7a1ffaa173f1d215005032f0
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35460883"
---
# <a name="group-unsubscribebymail"></a><span data-ttu-id="ba101-104">グループ: unsubscribeByMail</span><span class="sxs-lookup"><span data-stu-id="ba101-104">group: unsubscribeByMail</span></span>
<span data-ttu-id="ba101-p102">このメソッドを呼び出すと、現在のユーザーがそのグループ内の新規投稿、イベント、およびファイルに関するメール通知を受信しなくなります。Office 365 のグループのみをサポートします。</span><span class="sxs-lookup"><span data-stu-id="ba101-p102">Calling this method will prevent the current user from receiving email notifications for this group about new posts, events, and files in that group. Supported for Office 365 groups only.</span></span> 

## <a name="permissions"></a><span data-ttu-id="ba101-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ba101-107">Permissions</span></span>
<span data-ttu-id="ba101-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ba101-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba101-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ba101-110">Permission type</span></span>      | <span data-ttu-id="ba101-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ba101-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ba101-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ba101-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ba101-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba101-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ba101-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ba101-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba101-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ba101-115">Not supported.</span></span>    |
|<span data-ttu-id="ba101-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ba101-116">Application</span></span> | <span data-ttu-id="ba101-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ba101-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ba101-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ba101-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/unsubscribeByMail
```
## <a name="request-headers"></a><span data-ttu-id="ba101-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ba101-119">Request headers</span></span>
| <span data-ttu-id="ba101-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ba101-120">Header</span></span>       | <span data-ttu-id="ba101-121">値</span><span class="sxs-lookup"><span data-stu-id="ba101-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ba101-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ba101-122">Authorization</span></span>  | <span data-ttu-id="ba101-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ba101-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ba101-125">Prefer</span><span class="sxs-lookup"><span data-stu-id="ba101-125">Prefer</span></span> | <span data-ttu-id="ba101-126">return=minimal.</span><span class="sxs-lookup"><span data-stu-id="ba101-126">return=minimal.</span></span> <span data-ttu-id="ba101-127">最小応答ヘッダーが要求ヘッダーに含まれている場合、正常な応答で `204 No Content` コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="ba101-127">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="ba101-128">省略可能。</span><span class="sxs-lookup"><span data-stu-id="ba101-128">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="ba101-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="ba101-129">Request body</span></span>
<span data-ttu-id="ba101-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ba101-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ba101-131">応答</span><span class="sxs-lookup"><span data-stu-id="ba101-131">Response</span></span>
<span data-ttu-id="ba101-p106">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="ba101-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba101-134">例</span><span class="sxs-lookup"><span data-stu-id="ba101-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="ba101-135">要求</span><span class="sxs-lookup"><span data-stu-id="ba101-135">Request</span></span>
<span data-ttu-id="ba101-136">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ba101-136">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ba101-137">プロトコル</span><span class="sxs-lookup"><span data-stu-id="ba101-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_unsubscribebymail"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/unsubscribeByMail
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ba101-138">C#</span><span class="sxs-lookup"><span data-stu-id="ba101-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-unsubscribebymail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ba101-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="ba101-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-unsubscribebymail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ba101-140">目的-C</span><span class="sxs-lookup"><span data-stu-id="ba101-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-unsubscribebymail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ba101-141">応答</span><span class="sxs-lookup"><span data-stu-id="ba101-141">Response</span></span>
<span data-ttu-id="ba101-142">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ba101-142">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: unsubscribeByMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
