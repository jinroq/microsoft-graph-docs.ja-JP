---
title: 'グループ: unsubscribeByMail'
description: 'このメソッドを呼び出すと、現在のユーザーは、そのグループの新しい投稿、イベント、およびファイルに関するこのグループの電子メール通知を受信することを無効にします。 Office 365 グループに対してのみサポートされています。 '
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: a6673100e83f6702ed6bb45bbaae93d9dc07082d
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33592609"
---
# <a name="group-unsubscribebymail"></a><span data-ttu-id="9acc8-104">グループ: unsubscribeByMail</span><span class="sxs-lookup"><span data-stu-id="9acc8-104">group: unsubscribeByMail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9acc8-105">このメソッドを呼び出すと、現在のユーザーは、そのグループの新しい投稿、イベント、およびファイルに関するこのグループの電子メール通知を受信することを無効にします。</span><span class="sxs-lookup"><span data-stu-id="9acc8-105">Calling this method will disable the current user to receive email notifications for this group about new posts, events, and files in that group.</span></span> <span data-ttu-id="9acc8-106">Office 365 グループに対してのみサポートされています。</span><span class="sxs-lookup"><span data-stu-id="9acc8-106">Supported for Office 365 groups only.</span></span> 

## <a name="permissions"></a><span data-ttu-id="9acc8-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9acc8-107">Permissions</span></span>
<span data-ttu-id="9acc8-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9acc8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9acc8-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9acc8-110">Permission type</span></span>      | <span data-ttu-id="9acc8-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9acc8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9acc8-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9acc8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9acc8-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9acc8-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9acc8-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9acc8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9acc8-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9acc8-115">Not supported.</span></span>    |
|<span data-ttu-id="9acc8-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9acc8-116">Application</span></span> | <span data-ttu-id="9acc8-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9acc8-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9acc8-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9acc8-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/unsubscribeByMail
```

## <a name="request-headers"></a><span data-ttu-id="9acc8-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9acc8-119">Request headers</span></span>
| <span data-ttu-id="9acc8-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9acc8-120">Header</span></span>       | <span data-ttu-id="9acc8-121">値</span><span class="sxs-lookup"><span data-stu-id="9acc8-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9acc8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9acc8-122">Authorization</span></span>  | <span data-ttu-id="9acc8-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9acc8-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9acc8-125">Prefer</span><span class="sxs-lookup"><span data-stu-id="9acc8-125">Prefer</span></span> | <span data-ttu-id="9acc8-126">return=minimal.</span><span class="sxs-lookup"><span data-stu-id="9acc8-126">return=minimal.</span></span> <span data-ttu-id="9acc8-127">最小応答ヘッダーが要求ヘッダーに含まれている場合、正常な応答で `204 No Content` コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="9acc8-127">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="9acc8-128">省略可能。</span><span class="sxs-lookup"><span data-stu-id="9acc8-128">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="9acc8-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="9acc8-129">Request body</span></span>
 <span data-ttu-id="9acc8-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="9acc8-130">Do not supply a request body for this method.</span></span> 

## <a name="response"></a><span data-ttu-id="9acc8-131">応答</span><span class="sxs-lookup"><span data-stu-id="9acc8-131">Response</span></span>
<span data-ttu-id="9acc8-p106">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="9acc8-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9acc8-134">例</span><span class="sxs-lookup"><span data-stu-id="9acc8-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="9acc8-135">要求</span><span class="sxs-lookup"><span data-stu-id="9acc8-135">Request</span></span>
<span data-ttu-id="9acc8-136">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9acc8-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_unsubscribebymail"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/unsubscribeByMail
```

#### <a name="response"></a><span data-ttu-id="9acc8-137">応答</span><span class="sxs-lookup"><span data-stu-id="9acc8-137">Response</span></span>
<span data-ttu-id="9acc8-138">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9acc8-138">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="9acc8-139">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="9acc8-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="9acc8-140">Visual</span><span class="sxs-lookup"><span data-stu-id="9acc8-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/group_unsubscribebymail-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9acc8-141">Java</span><span class="sxs-lookup"><span data-stu-id="9acc8-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/group_unsubscribebymail-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/group-unsubscribebymail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-unsubscribebymail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
