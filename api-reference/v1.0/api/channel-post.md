---
title: チャネルを作成します。
description: 要求の本体に指定されている、マイクロソフトのチームでは、新しいチャネルを作成します。
localization_priority: Priority
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 9021ed45cb187b8db64ec2a3270b6a7f840134ba
ms.sourcegitcommit: 2c60e38bb1b71ba958659f66ad4736495e520851
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/15/2019
ms.locfileid: "28016689"
---
# <a name="create-channel"></a><span data-ttu-id="8472f-103">チャネルを作成します。</span><span class="sxs-lookup"><span data-stu-id="8472f-103">Create Channel</span></span>



<span data-ttu-id="8472f-104">要求の本体に指定されている、マイクロソフトのチームでは、新しい[チャネル](../resources/channel.md)を作成します。</span><span class="sxs-lookup"><span data-stu-id="8472f-104">Create a new [channel](../resources/channel.md) in a Microsoft Team, as specified in the request body.</span></span>

> <span data-ttu-id="8472f-105">**注**: アプリケーションのアクセス許可とこの API に関する既知の問題があります。</span><span class="sxs-lookup"><span data-stu-id="8472f-105">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="8472f-106">詳細についてはの[既知の問題点のリスト](/graph/known-issues#application-permissions)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8472f-106">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

## <a name="permissions"></a><span data-ttu-id="8472f-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8472f-107">Permissions</span></span>
<span data-ttu-id="8472f-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8472f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="8472f-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8472f-110">Permission type</span></span>      | <span data-ttu-id="8472f-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8472f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8472f-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8472f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8472f-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8472f-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8472f-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8472f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8472f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8472f-115">Not supported.</span></span>    |
|<span data-ttu-id="8472f-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8472f-116">Application</span></span> | <span data-ttu-id="8472f-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8472f-117">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="8472f-118">**注**: この API は、管理者のアクセス許可をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="8472f-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="8472f-119">グローバル管理者とサービス管理者のマイクロソフトのチームのメンバーではないことをチームにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="8472f-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="8472f-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8472f-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels
```
## <a name="request-headers"></a><span data-ttu-id="8472f-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8472f-121">Request headers</span></span>
| <span data-ttu-id="8472f-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8472f-122">Header</span></span>       | <span data-ttu-id="8472f-123">値</span><span class="sxs-lookup"><span data-stu-id="8472f-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8472f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="8472f-124">Authorization</span></span>  | <span data-ttu-id="8472f-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8472f-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8472f-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8472f-127">Content-Type</span></span>  | <span data-ttu-id="8472f-128">application/json</span><span class="sxs-lookup"><span data-stu-id="8472f-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8472f-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="8472f-129">Request body</span></span>
<span data-ttu-id="8472f-130">要求の本文には、[チャネル](../resources/channel.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="8472f-130">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="8472f-131">応答</span><span class="sxs-lookup"><span data-stu-id="8472f-131">Response</span></span>

<span data-ttu-id="8472f-132">かどうかは成功すると、このメソッドを返します`201 Created`、応答の本体での応答コードおよび[チャネル](../resources/channel.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="8472f-132">If successful, this method returns `201 Created` response code and [channel](../resources/channel.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8472f-133">例</span><span class="sxs-lookup"><span data-stu-id="8472f-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8472f-134">要求</span><span class="sxs-lookup"><span data-stu-id="8472f-134">Request</span></span>
<span data-ttu-id="8472f-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8472f-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_channel_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/{id}/channels
Content-type: application/json

{
  "displayName": "Architecture Discussion",
  "description": "This channel is where we debate all future architecture plans"
}
```
##### <a name="response"></a><span data-ttu-id="8472f-136">応答</span><span class="sxs-lookup"><span data-stu-id="8472f-136">Response</span></span>
<span data-ttu-id="8472f-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8472f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
