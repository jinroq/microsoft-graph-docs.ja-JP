---
title: 'グループ: subscribeByMail'
description: このメソッドを呼び出すと、現在のユーザーがそのグループ内の新規投稿、イベント、およびファイルに関するメール通知を受信できるようになります。 Office 365 グループのみをサポートします。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 0a334daa005947099da324aab31ccc2a1da6b6e0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32501963"
---
# <a name="group-subscribebymail"></a><span data-ttu-id="6a062-104">グループ: subscribeByMail</span><span class="sxs-lookup"><span data-stu-id="6a062-104">group: subscribeByMail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a062-105">このメソッドを呼び出すと、現在のユーザーがそのグループ内の新規投稿、イベント、およびファイルに関するメール通知を受信できるようになります。</span><span class="sxs-lookup"><span data-stu-id="6a062-105">Calling this method will enable the current user to receive email notifications for this group, about new posts, events, and files in that group.</span></span> <span data-ttu-id="6a062-106">Office 365 グループのみをサポートします。</span><span class="sxs-lookup"><span data-stu-id="6a062-106">Supported for Office 365 Groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="6a062-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6a062-107">Permissions</span></span>
<span data-ttu-id="6a062-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6a062-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a062-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6a062-110">Permission type</span></span>      | <span data-ttu-id="6a062-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6a062-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6a062-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6a062-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6a062-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a062-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="6a062-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6a062-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a062-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6a062-115">Not supported.</span></span>    |
|<span data-ttu-id="6a062-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6a062-116">Application</span></span> | <span data-ttu-id="6a062-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6a062-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6a062-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6a062-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/subscribeByMail
```
## <a name="request-headers"></a><span data-ttu-id="6a062-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6a062-119">Request headers</span></span>
| <span data-ttu-id="6a062-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6a062-120">Header</span></span>       | <span data-ttu-id="6a062-121">値</span><span class="sxs-lookup"><span data-stu-id="6a062-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6a062-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a062-122">Authorization</span></span>  | <span data-ttu-id="6a062-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6a062-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6a062-125">Prefer</span><span class="sxs-lookup"><span data-stu-id="6a062-125">Prefer</span></span> | <span data-ttu-id="6a062-126">return=minimal.</span><span class="sxs-lookup"><span data-stu-id="6a062-126">return=minimal.</span></span> <span data-ttu-id="6a062-127">最小応答ヘッダーが要求ヘッダーに含まれている場合、正常な応答で `204 No Content` コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="6a062-127">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="6a062-128">省略可能。</span><span class="sxs-lookup"><span data-stu-id="6a062-128">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="6a062-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="6a062-129">Request body</span></span>

## <a name="response"></a><span data-ttu-id="6a062-130">応答</span><span class="sxs-lookup"><span data-stu-id="6a062-130">Response</span></span>
<span data-ttu-id="6a062-p106">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="6a062-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a062-133">例</span><span class="sxs-lookup"><span data-stu-id="6a062-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="6a062-134">要求</span><span class="sxs-lookup"><span data-stu-id="6a062-134">Request</span></span>
<span data-ttu-id="6a062-135">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6a062-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_subscribebymail"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/subscribeByMail
```

#### <a name="response"></a><span data-ttu-id="6a062-136">応答</span><span class="sxs-lookup"><span data-stu-id="6a062-136">Response</span></span>
<span data-ttu-id="6a062-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6a062-137">The following is an example of the response.</span></span> 
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
    "Error: /api-reference/beta/api/group-subscribebymail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
