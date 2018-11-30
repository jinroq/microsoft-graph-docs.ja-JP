---
title: パッチ チャネル
description: 指定されたチャネルのプロパティを更新します。
ms.openlocfilehash: 833b5cf4999f43e9de799691a9f6d7a98318d4fe
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066651"
---
# <a name="patch-channel"></a><span data-ttu-id="49804-103">パッチ チャネル</span><span class="sxs-lookup"><span data-stu-id="49804-103">Patch channel</span></span>

> <span data-ttu-id="49804-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="49804-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="49804-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="49804-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="49804-106">指定された[チャネル](../resources/channel.md)のプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="49804-106">Update the properties of the specified [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="49804-107">**注**: アプリケーションのアクセス許可とこの API に関する既知の問題があります。</span><span class="sxs-lookup"><span data-stu-id="49804-107">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="49804-108">詳細についてはの[既知の問題点のリスト](/graph/known-issues#application-permissions)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="49804-108">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

## <a name="permissions"></a><span data-ttu-id="49804-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="49804-109">Permissions</span></span>
<span data-ttu-id="49804-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="49804-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49804-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="49804-112">Permission type</span></span>      | <span data-ttu-id="49804-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="49804-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="49804-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="49804-114">Delegated (work or school account)</span></span> | <span data-ttu-id="49804-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49804-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="49804-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="49804-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49804-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="49804-117">Not supported.</span></span>    |
|<span data-ttu-id="49804-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="49804-118">Application</span></span> | <span data-ttu-id="49804-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49804-119">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="49804-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="49804-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}/channels/{id}
```
## <a name="request-headers"></a><span data-ttu-id="49804-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="49804-121">Request headers</span></span>
| <span data-ttu-id="49804-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="49804-122">Header</span></span>       | <span data-ttu-id="49804-123">値</span><span class="sxs-lookup"><span data-stu-id="49804-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="49804-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="49804-124">Authorization</span></span>  | <span data-ttu-id="49804-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="49804-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="49804-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="49804-127">Content-Type</span></span>  | <span data-ttu-id="49804-128">application/json</span><span class="sxs-lookup"><span data-stu-id="49804-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="49804-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="49804-129">Request body</span></span>
<span data-ttu-id="49804-130">要求の本文には、[チャネル](../resources/channel.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="49804-130">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="49804-131">応答</span><span class="sxs-lookup"><span data-stu-id="49804-131">Response</span></span>

<span data-ttu-id="49804-132">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="49804-132">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="49804-133">例</span><span class="sxs-lookup"><span data-stu-id="49804-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="49804-134">要求</span><span class="sxs-lookup"><span data-stu-id="49804-134">Request</span></span>
<span data-ttu-id="49804-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="49804-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "patch_channel"
}-->
```http
PATCH https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```
##### <a name="response"></a><span data-ttu-id="49804-136">応答</span><span class="sxs-lookup"><span data-stu-id="49804-136">Response</span></span>
<span data-ttu-id="49804-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="49804-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
    "description": "description-value",
    "displayName": "display-name-value",
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Patch channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
