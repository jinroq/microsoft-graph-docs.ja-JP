---
title: チャネルを削除する
description: チャネルを削除します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e4e84fb7e011a6a4a56dea7a71748fac85f17e07
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35882300"
---
# <a name="delete-channel"></a><span data-ttu-id="8b564-103">チャネルを削除する</span><span class="sxs-lookup"><span data-stu-id="8b564-103">Delete channel</span></span>



<span data-ttu-id="8b564-104">[チャネル](../resources/channel.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="8b564-104">Delete the [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="8b564-105">**注**: アプリケーションのアクセス許可とこの API には既知の問題があります。</span><span class="sxs-lookup"><span data-stu-id="8b564-105">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="8b564-106">詳細については、「[既知の問題の一覧](/graph/known-issues#application-permissions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8b564-106">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

> <span data-ttu-id="8b564-107">**注**: 削除されたチャネル内のデータは、チーム所有者が削除されたチャネルを回復できるように、数週間にわたって引き続き保存されます。</span><span class="sxs-lookup"><span data-stu-id="8b564-107">**Note**: The data in deleted channels will continue to be stored for several weeks to allow team owner to recovery deleted channel.</span></span> <span data-ttu-id="8b564-108">その間、同じ displayName で新しいチャネルを作成することはできません。</span><span class="sxs-lookup"><span data-stu-id="8b564-108">During that time, a new channel with the same displayName may not be created.</span></span>

## <a name="permissions"></a><span data-ttu-id="8b564-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8b564-109">Permissions</span></span>
<span data-ttu-id="8b564-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8b564-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b564-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8b564-112">Permission type</span></span>      | <span data-ttu-id="8b564-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8b564-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8b564-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8b564-114">Delegated (work or school account)</span></span> | <span data-ttu-id="8b564-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b564-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8b564-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8b564-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b564-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8b564-117">Not supported.</span></span>    |
|<span data-ttu-id="8b564-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8b564-118">Application</span></span> | <span data-ttu-id="8b564-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b564-119">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="8b564-120">**注**: この API は、管理者のアクセス許可をサポートします。</span><span class="sxs-lookup"><span data-stu-id="8b564-120">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="8b564-121">グローバル管理者と Microsoft Teams サービス管理者は、メンバーではないチームにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="8b564-121">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="8b564-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8b564-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/channels/{id}
```
## <a name="request-headers"></a><span data-ttu-id="8b564-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8b564-123">Request headers</span></span>
| <span data-ttu-id="8b564-124">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8b564-124">Header</span></span>       | <span data-ttu-id="8b564-125">値</span><span class="sxs-lookup"><span data-stu-id="8b564-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8b564-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="8b564-126">Authorization</span></span>  | <span data-ttu-id="8b564-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8b564-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8b564-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="8b564-129">Request body</span></span>
<span data-ttu-id="8b564-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="8b564-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8b564-131">応答</span><span class="sxs-lookup"><span data-stu-id="8b564-131">Response</span></span>

<span data-ttu-id="8b564-p106">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="8b564-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8b564-134">例</span><span class="sxs-lookup"><span data-stu-id="8b564-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8b564-135">要求</span><span class="sxs-lookup"><span data-stu-id="8b564-135">Request</span></span>
<span data-ttu-id="8b564-136">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8b564-136">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8b564-137">プロトコル</span><span class="sxs-lookup"><span data-stu-id="8b564-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_channel"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8b564-138">C#</span><span class="sxs-lookup"><span data-stu-id="8b564-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-channel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8b564-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="8b564-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-channel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8b564-140">目的-C</span><span class="sxs-lookup"><span data-stu-id="8b564-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8b564-141">Java</span><span class="sxs-lookup"><span data-stu-id="8b564-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-channel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8b564-142">応答</span><span class="sxs-lookup"><span data-stu-id="8b564-142">Response</span></span>

<span data-ttu-id="8b564-143">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8b564-143">The following is an example of the response.</span></span> 
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
  "description": "Delete channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
