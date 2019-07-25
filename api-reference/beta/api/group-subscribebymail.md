---
title: 'グループ: subscribeByMail'
description: このメソッドを呼び出すと、現在のユーザーがそのグループ内の新規投稿、イベント、およびファイルに関するメール通知を受信できるようになります。 Office 365 グループのみをサポートします。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 12503de3c37cfa6e77affdd8125fe9cc7e431232
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35857935"
---
# <a name="group-subscribebymail"></a><span data-ttu-id="da956-104">グループ: subscribeByMail</span><span class="sxs-lookup"><span data-stu-id="da956-104">group: subscribeByMail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da956-105">このメソッドを呼び出すと、現在のユーザーがそのグループ内の新規投稿、イベント、およびファイルに関するメール通知を受信できるようになります。</span><span class="sxs-lookup"><span data-stu-id="da956-105">Calling this method will enable the current user to receive email notifications for this group, about new posts, events, and files in that group.</span></span> <span data-ttu-id="da956-106">Office 365 グループのみをサポートします。</span><span class="sxs-lookup"><span data-stu-id="da956-106">Supported for Office 365 Groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="da956-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="da956-107">Permissions</span></span>
<span data-ttu-id="da956-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="da956-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da956-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="da956-110">Permission type</span></span>      | <span data-ttu-id="da956-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="da956-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="da956-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="da956-112">Delegated (work or school account)</span></span> | <span data-ttu-id="da956-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da956-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="da956-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="da956-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da956-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="da956-115">Not supported.</span></span>    |
|<span data-ttu-id="da956-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="da956-116">Application</span></span> | <span data-ttu-id="da956-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="da956-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="da956-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="da956-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/subscribeByMail
```
## <a name="request-headers"></a><span data-ttu-id="da956-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="da956-119">Request headers</span></span>
| <span data-ttu-id="da956-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="da956-120">Header</span></span>       | <span data-ttu-id="da956-121">値</span><span class="sxs-lookup"><span data-stu-id="da956-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="da956-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="da956-122">Authorization</span></span>  | <span data-ttu-id="da956-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="da956-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="da956-125">Prefer</span><span class="sxs-lookup"><span data-stu-id="da956-125">Prefer</span></span> | <span data-ttu-id="da956-126">return=minimal.</span><span class="sxs-lookup"><span data-stu-id="da956-126">return=minimal.</span></span> <span data-ttu-id="da956-127">最小応答ヘッダーが要求ヘッダーに含まれている場合、正常な応答で `204 No Content` コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="da956-127">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="da956-128">省略可能。</span><span class="sxs-lookup"><span data-stu-id="da956-128">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="da956-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="da956-129">Request body</span></span>

## <a name="response"></a><span data-ttu-id="da956-130">応答</span><span class="sxs-lookup"><span data-stu-id="da956-130">Response</span></span>
<span data-ttu-id="da956-p106">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="da956-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da956-133">例</span><span class="sxs-lookup"><span data-stu-id="da956-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="da956-134">要求</span><span class="sxs-lookup"><span data-stu-id="da956-134">Request</span></span>
<span data-ttu-id="da956-135">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="da956-135">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="da956-136">プロトコル</span><span class="sxs-lookup"><span data-stu-id="da956-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_subscribebymail"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/subscribeByMail
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="da956-137">C#</span><span class="sxs-lookup"><span data-stu-id="da956-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-subscribebymail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="da956-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="da956-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-subscribebymail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="da956-139">目的-C</span><span class="sxs-lookup"><span data-stu-id="da956-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-subscribebymail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="da956-140">Java</span><span class="sxs-lookup"><span data-stu-id="da956-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-subscribebymail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="da956-141">応答</span><span class="sxs-lookup"><span data-stu-id="da956-141">Response</span></span>
<span data-ttu-id="da956-142">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="da956-142">The following is an example of the response.</span></span> 
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
  "description": "group: subscribeByMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
