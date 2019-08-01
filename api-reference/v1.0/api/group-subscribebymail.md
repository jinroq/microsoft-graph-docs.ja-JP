---
title: 'グループ: subscribeByMail'
description: このメソッドを呼び出すと、現在のユーザーがそのグループ内の新規投稿、イベント、およびファイルに関するメール通知を受信できるようになります。Office 365 のグループのみをサポートします。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: ba29352f6ce0b913f0a9af70484a123952945343
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36014726"
---
# <a name="group-subscribebymail"></a><span data-ttu-id="b8330-104">グループ: subscribeByMail</span><span class="sxs-lookup"><span data-stu-id="b8330-104">group: subscribeByMail</span></span>
<span data-ttu-id="b8330-p102">このメソッドを呼び出すと、現在のユーザーがそのグループ内の新規投稿、イベント、およびファイルに関するメール通知を受信できるようになります。Office 365 のグループのみをサポートします。</span><span class="sxs-lookup"><span data-stu-id="b8330-p102">Calling this method will enable the current user to receive email notifications for this group, about new posts, events, and files in that group. Supported for Office 365 groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="b8330-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b8330-107">Permissions</span></span>
<span data-ttu-id="b8330-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b8330-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8330-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b8330-110">Permission type</span></span>      | <span data-ttu-id="b8330-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b8330-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b8330-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b8330-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b8330-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8330-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b8330-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b8330-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8330-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b8330-115">Not supported.</span></span>    |
|<span data-ttu-id="b8330-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b8330-116">Application</span></span> | <span data-ttu-id="b8330-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b8330-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b8330-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b8330-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/subscribeByMail
```
## <a name="request-headers"></a><span data-ttu-id="b8330-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b8330-119">Request headers</span></span>
| <span data-ttu-id="b8330-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b8330-120">Header</span></span>       | <span data-ttu-id="b8330-121">値</span><span class="sxs-lookup"><span data-stu-id="b8330-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b8330-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b8330-122">Authorization</span></span>  | <span data-ttu-id="b8330-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b8330-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b8330-125">Prefer</span><span class="sxs-lookup"><span data-stu-id="b8330-125">Prefer</span></span> | <span data-ttu-id="b8330-126">return=minimal.</span><span class="sxs-lookup"><span data-stu-id="b8330-126">return=minimal.</span></span> <span data-ttu-id="b8330-127">最小応答ヘッダーが要求ヘッダーに含まれている場合、正常な応答で `204 No Content` コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="b8330-127">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="b8330-128">省略可能。</span><span class="sxs-lookup"><span data-stu-id="b8330-128">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="b8330-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="b8330-129">Request body</span></span>
<span data-ttu-id="b8330-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b8330-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b8330-131">応答</span><span class="sxs-lookup"><span data-stu-id="b8330-131">Response</span></span>
<span data-ttu-id="b8330-p106">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="b8330-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8330-134">例</span><span class="sxs-lookup"><span data-stu-id="b8330-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="b8330-135">要求</span><span class="sxs-lookup"><span data-stu-id="b8330-135">Request</span></span>
<span data-ttu-id="b8330-136">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b8330-136">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b8330-137">プロトコル</span><span class="sxs-lookup"><span data-stu-id="b8330-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_subscribebymail"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/subscribeByMail
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b8330-138">C#</span><span class="sxs-lookup"><span data-stu-id="b8330-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-subscribebymail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b8330-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="b8330-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-subscribebymail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b8330-140">目的-C</span><span class="sxs-lookup"><span data-stu-id="b8330-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-subscribebymail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b8330-141">Java</span><span class="sxs-lookup"><span data-stu-id="b8330-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-subscribebymail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b8330-142">応答</span><span class="sxs-lookup"><span data-stu-id="b8330-142">Response</span></span>
<span data-ttu-id="b8330-143">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b8330-143">The following is an example of the response.</span></span> 
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
  "description": "group: subscribeByMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
