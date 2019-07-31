---
title: チャネルを作成する
description: 要求の本文で指定されているように、Microsoft Team に新しいチャネルを作成します。
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: f119181375cfb97128ddcef619e5ea6730d34140
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35944206"
---
# <a name="create-channel"></a><span data-ttu-id="529b0-103">チャネルを作成する</span><span class="sxs-lookup"><span data-stu-id="529b0-103">Create Channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="529b0-104">要求の本文で指定されているように、Microsoft Team に新しい[チャネル](../resources/channel.md)を作成します。</span><span class="sxs-lookup"><span data-stu-id="529b0-104">Create a new [channel](../resources/channel.md) in a Microsoft Team, as specified in the request body.</span></span>

> <span data-ttu-id="529b0-105">**注**: アプリケーションのアクセス許可とこの API には既知の問題があります。</span><span class="sxs-lookup"><span data-stu-id="529b0-105">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="529b0-106">詳細については、「[既知の問題の一覧](/graph/known-issues#application-permissions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="529b0-106">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

## <a name="permissions"></a><span data-ttu-id="529b0-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="529b0-107">Permissions</span></span>
<span data-ttu-id="529b0-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="529b0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="529b0-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="529b0-110">Permission type</span></span>      | <span data-ttu-id="529b0-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="529b0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="529b0-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="529b0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="529b0-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="529b0-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="529b0-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="529b0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="529b0-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="529b0-115">Not supported.</span></span>    |
|<span data-ttu-id="529b0-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="529b0-116">Application</span></span> | <span data-ttu-id="529b0-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="529b0-117">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="529b0-118">**注**: この API は、管理者のアクセス許可をサポートします。</span><span class="sxs-lookup"><span data-stu-id="529b0-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="529b0-119">グローバル管理者と Microsoft Teams サービス管理者は、メンバーではないチームにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="529b0-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="529b0-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="529b0-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels
```
## <a name="request-headers"></a><span data-ttu-id="529b0-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="529b0-121">Request headers</span></span>
| <span data-ttu-id="529b0-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="529b0-122">Header</span></span>       | <span data-ttu-id="529b0-123">値</span><span class="sxs-lookup"><span data-stu-id="529b0-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="529b0-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="529b0-124">Authorization</span></span>  | <span data-ttu-id="529b0-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="529b0-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="529b0-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="529b0-127">Content-Type</span></span>  | <span data-ttu-id="529b0-128">application/json</span><span class="sxs-lookup"><span data-stu-id="529b0-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="529b0-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="529b0-129">Request body</span></span>
<span data-ttu-id="529b0-130">要求本文で、[チャンネル](../resources/channel.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="529b0-130">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="529b0-131">応答</span><span class="sxs-lookup"><span data-stu-id="529b0-131">Response</span></span>

<span data-ttu-id="529b0-132">成功した場合、このメソッドは `201 Created` 応答コードと [チャンネル](../resources/channel.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="529b0-132">If successful, this method returns `201 Created` response code and [channel](../resources/channel.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="529b0-133">例</span><span class="sxs-lookup"><span data-stu-id="529b0-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="529b0-134">要求</span><span class="sxs-lookup"><span data-stu-id="529b0-134">Request</span></span>
<span data-ttu-id="529b0-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="529b0-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="529b0-136">プロトコル</span><span class="sxs-lookup"><span data-stu-id="529b0-136">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="529b0-137">C#</span><span class="sxs-lookup"><span data-stu-id="529b0-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-channel-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="529b0-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="529b0-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-channel-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="529b0-139">目的-C</span><span class="sxs-lookup"><span data-stu-id="529b0-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-channel-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="529b0-140">Java</span><span class="sxs-lookup"><span data-stu-id="529b0-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-channel-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="529b0-141">応答</span><span class="sxs-lookup"><span data-stu-id="529b0-141">Response</span></span>
<span data-ttu-id="529b0-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="529b0-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create Channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
