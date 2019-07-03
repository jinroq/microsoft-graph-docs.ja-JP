---
title: チャネルを削除する
description: チャネルを削除します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: b587ddb85f7a7911ffb2e964b45a6d3dacbf17b3
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35438539"
---
# <a name="delete-channel"></a><span data-ttu-id="a32cc-103">チャネルを削除する</span><span class="sxs-lookup"><span data-stu-id="a32cc-103">Delete channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a32cc-104">[チャネル](../resources/channel.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="a32cc-104">Delete the [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="a32cc-105">**注**: アプリケーションのアクセス許可とこの API には既知の問題があります。</span><span class="sxs-lookup"><span data-stu-id="a32cc-105">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="a32cc-106">詳細については、「[既知の問題の一覧](/graph/known-issues#application-permissions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a32cc-106">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

## <a name="permissions"></a><span data-ttu-id="a32cc-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a32cc-107">Permissions</span></span>
<span data-ttu-id="a32cc-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a32cc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a32cc-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a32cc-110">Permission type</span></span>      | <span data-ttu-id="a32cc-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a32cc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a32cc-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a32cc-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a32cc-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a32cc-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a32cc-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a32cc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a32cc-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a32cc-115">Not supported.</span></span>    |
|<span data-ttu-id="a32cc-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a32cc-116">Application</span></span> | <span data-ttu-id="a32cc-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a32cc-117">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="a32cc-118">**注**: この API は、管理者のアクセス許可をサポートします。</span><span class="sxs-lookup"><span data-stu-id="a32cc-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="a32cc-119">グローバル管理者と Microsoft Teams サービス管理者は、メンバーではないチームにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="a32cc-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="a32cc-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a32cc-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/channels/{id}
```
## <a name="request-headers"></a><span data-ttu-id="a32cc-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a32cc-121">Request headers</span></span>
| <span data-ttu-id="a32cc-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a32cc-122">Header</span></span>       | <span data-ttu-id="a32cc-123">値</span><span class="sxs-lookup"><span data-stu-id="a32cc-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a32cc-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a32cc-124">Authorization</span></span>  | <span data-ttu-id="a32cc-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a32cc-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a32cc-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="a32cc-127">Request body</span></span>
<span data-ttu-id="a32cc-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a32cc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a32cc-129">応答</span><span class="sxs-lookup"><span data-stu-id="a32cc-129">Response</span></span>

<span data-ttu-id="a32cc-p105">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="a32cc-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a32cc-132">例</span><span class="sxs-lookup"><span data-stu-id="a32cc-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a32cc-133">要求</span><span class="sxs-lookup"><span data-stu-id="a32cc-133">Request</span></span>
<span data-ttu-id="a32cc-134">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a32cc-134">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a32cc-135">プロトコル</span><span class="sxs-lookup"><span data-stu-id="a32cc-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_channel"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a32cc-136">C#</span><span class="sxs-lookup"><span data-stu-id="a32cc-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-channel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a32cc-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="a32cc-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-channel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a32cc-138">目的-C</span><span class="sxs-lookup"><span data-stu-id="a32cc-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a32cc-139">応答</span><span class="sxs-lookup"><span data-stu-id="a32cc-139">Response</span></span>

<span data-ttu-id="a32cc-140">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a32cc-140">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
