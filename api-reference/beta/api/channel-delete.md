---
title: チャネルを削除します。
description: チャネルを削除します。
ms.openlocfilehash: 8f34db306ae42493cf23f29117aece6fd4942c2b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066376"
---
# <a name="delete-channel"></a><span data-ttu-id="08ad7-103">チャネルを削除します。</span><span class="sxs-lookup"><span data-stu-id="08ad7-103">Delete channel</span></span>

> <span data-ttu-id="08ad7-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="08ad7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="08ad7-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="08ad7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="08ad7-106">[チャネル](../resources/channel.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="08ad7-106">Delete the [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="08ad7-107">**注**: アプリケーションのアクセス許可とこの API に関する既知の問題があります。</span><span class="sxs-lookup"><span data-stu-id="08ad7-107">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="08ad7-108">詳細についてはの[既知の問題点のリスト](/graph/known-issues#application-permissions)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="08ad7-108">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

## <a name="permissions"></a><span data-ttu-id="08ad7-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="08ad7-109">Permissions</span></span>
<span data-ttu-id="08ad7-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="08ad7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08ad7-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="08ad7-112">Permission type</span></span>      | <span data-ttu-id="08ad7-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="08ad7-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="08ad7-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="08ad7-114">Delegated (work or school account)</span></span> | <span data-ttu-id="08ad7-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08ad7-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="08ad7-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="08ad7-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08ad7-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="08ad7-117">Not supported.</span></span>    |
|<span data-ttu-id="08ad7-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="08ad7-118">Application</span></span> | <span data-ttu-id="08ad7-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08ad7-119">Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="08ad7-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="08ad7-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/channels/{id}
```
## <a name="request-headers"></a><span data-ttu-id="08ad7-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="08ad7-121">Request headers</span></span>
| <span data-ttu-id="08ad7-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="08ad7-122">Header</span></span>       | <span data-ttu-id="08ad7-123">値</span><span class="sxs-lookup"><span data-stu-id="08ad7-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="08ad7-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="08ad7-124">Authorization</span></span>  | <span data-ttu-id="08ad7-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="08ad7-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="08ad7-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="08ad7-127">Request body</span></span>
<span data-ttu-id="08ad7-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="08ad7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="08ad7-129">応答</span><span class="sxs-lookup"><span data-stu-id="08ad7-129">Response</span></span>

<span data-ttu-id="08ad7-p105">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="08ad7-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="08ad7-132">例</span><span class="sxs-lookup"><span data-stu-id="08ad7-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="08ad7-133">要求</span><span class="sxs-lookup"><span data-stu-id="08ad7-133">Request</span></span>
<span data-ttu-id="08ad7-134">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="08ad7-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_channel"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```

#### <a name="response"></a><span data-ttu-id="08ad7-135">応答</span><span class="sxs-lookup"><span data-stu-id="08ad7-135">Response</span></span>

<span data-ttu-id="08ad7-136">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="08ad7-136">The following is an example of the response.</span></span> 
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
  "tocPath": ""
}-->
