---
title: チャネルを作成します。
description: 要求の本体に指定されている、マイクロソフトのチームでは、新しいチャネルを作成します。
ms.openlocfilehash: 7f561c13b688d76ec4d45f03c2fd7f73192fe8a8
ms.sourcegitcommit: 72d4da2a6bfaf99fa4edaf6ce3b97b1a6d96d874
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/11/2018
ms.locfileid: "27222528"
---
# <a name="create-channel"></a><span data-ttu-id="f11db-103">チャネルを作成します。</span><span class="sxs-lookup"><span data-stu-id="f11db-103">Create Channel</span></span>

> <span data-ttu-id="f11db-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f11db-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f11db-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f11db-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f11db-106">要求の本体に指定されている、マイクロソフトのチームでは、新しい[チャネル](../resources/channel.md)を作成します。</span><span class="sxs-lookup"><span data-stu-id="f11db-106">Create a new [channel](../resources/channel.md) in a Microsoft Team, as specified in the request body.</span></span>

> <span data-ttu-id="f11db-107">**注**: アプリケーションのアクセス許可とこの API に関する既知の問題があります。</span><span class="sxs-lookup"><span data-stu-id="f11db-107">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="f11db-108">詳細についてはの[既知の問題点のリスト](/graph/known-issues#application-permissions)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f11db-108">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

## <a name="permissions"></a><span data-ttu-id="f11db-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f11db-109">Permissions</span></span>
<span data-ttu-id="f11db-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f11db-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f11db-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f11db-112">Permission type</span></span>      | <span data-ttu-id="f11db-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f11db-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f11db-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f11db-114">Delegated (work or school account)</span></span> | <span data-ttu-id="f11db-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f11db-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f11db-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f11db-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f11db-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f11db-117">Not supported.</span></span>    |
|<span data-ttu-id="f11db-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f11db-118">Application</span></span> | <span data-ttu-id="f11db-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f11db-119">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="f11db-120">**注**: この API は、管理者のアクセス許可をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="f11db-120">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="f11db-121">グローバル管理者とサービス管理者のマイクロソフトのチームのメンバーではないことをチームにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="f11db-121">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="f11db-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f11db-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels
```
## <a name="request-headers"></a><span data-ttu-id="f11db-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f11db-123">Request headers</span></span>
| <span data-ttu-id="f11db-124">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f11db-124">Header</span></span>       | <span data-ttu-id="f11db-125">値</span><span class="sxs-lookup"><span data-stu-id="f11db-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f11db-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="f11db-126">Authorization</span></span>  | <span data-ttu-id="f11db-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f11db-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f11db-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f11db-129">Content-Type</span></span>  | <span data-ttu-id="f11db-130">application/json</span><span class="sxs-lookup"><span data-stu-id="f11db-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f11db-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="f11db-131">Request body</span></span>
<span data-ttu-id="f11db-132">要求の本文には、[チャネル](../resources/channel.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="f11db-132">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f11db-133">応答</span><span class="sxs-lookup"><span data-stu-id="f11db-133">Response</span></span>

<span data-ttu-id="f11db-134">かどうかは成功すると、このメソッドを返します`201 Created`、応答の本体での応答コードおよび[チャネル](../resources/channel.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="f11db-134">If successful, this method returns `201 Created` response code and [channel](../resources/channel.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f11db-135">例</span><span class="sxs-lookup"><span data-stu-id="f11db-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f11db-136">要求</span><span class="sxs-lookup"><span data-stu-id="f11db-136">Request</span></span>
<span data-ttu-id="f11db-137">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f11db-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_channel_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels
Content-type: application/json

{
  "displayName": "Architecture Discussion",
  "description": "This channel is where we debate all future architecture plans"
}
```
##### <a name="response"></a><span data-ttu-id="f11db-138">応答</span><span class="sxs-lookup"><span data-stu-id="f11db-138">Response</span></span>
<span data-ttu-id="f11db-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f11db-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "id": "id-value",
  "displayName": "Architecture Discussion",
  "description": "This channel is where we debate all future architecture plans"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->