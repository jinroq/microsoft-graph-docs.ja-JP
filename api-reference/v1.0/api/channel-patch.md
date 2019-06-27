---
title: パッチチャネル
description: 指定したチャネルのプロパティを更新します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: b101b964d166ffd2a757a2c461f019c107d5db7b
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35273704"
---
# <a name="patch-channel"></a><span data-ttu-id="e3375-103">パッチチャネル</span><span class="sxs-lookup"><span data-stu-id="e3375-103">Patch channel</span></span>



<span data-ttu-id="e3375-104">指定した[チャネル](../resources/channel.md)のプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e3375-104">Update the properties of the specified [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="e3375-105">**注**: アプリケーションのアクセス許可とこの API には既知の問題があります。</span><span class="sxs-lookup"><span data-stu-id="e3375-105">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="e3375-106">詳細については、「[既知の問題の一覧](/graph/known-issues#application-permissions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e3375-106">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

## <a name="permissions"></a><span data-ttu-id="e3375-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e3375-107">Permissions</span></span>
<span data-ttu-id="e3375-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e3375-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3375-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e3375-110">Permission type</span></span>      | <span data-ttu-id="e3375-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e3375-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e3375-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e3375-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e3375-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3375-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e3375-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e3375-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3375-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e3375-115">Not supported.</span></span>    |
|<span data-ttu-id="e3375-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e3375-116">Application</span></span> | <span data-ttu-id="e3375-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3375-117">Group.ReadWrite.All</span></span> |

> <span data-ttu-id="e3375-118">**注**: この API は、管理者のアクセス許可をサポートします。</span><span class="sxs-lookup"><span data-stu-id="e3375-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="e3375-119">グローバル管理者と Microsoft Teams サービス管理者は、メンバーではないチームにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="e3375-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="e3375-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e3375-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}/channels/{id}
```
## <a name="request-headers"></a><span data-ttu-id="e3375-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e3375-121">Request headers</span></span>
| <span data-ttu-id="e3375-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e3375-122">Header</span></span>       | <span data-ttu-id="e3375-123">値</span><span class="sxs-lookup"><span data-stu-id="e3375-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e3375-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3375-124">Authorization</span></span>  | <span data-ttu-id="e3375-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e3375-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e3375-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e3375-127">Content-Type</span></span>  | <span data-ttu-id="e3375-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e3375-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e3375-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="e3375-129">Request body</span></span>
<span data-ttu-id="e3375-130">要求本文で、[チャンネル](../resources/channel.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e3375-130">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e3375-131">応答</span><span class="sxs-lookup"><span data-stu-id="e3375-131">Response</span></span>

<span data-ttu-id="e3375-132">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="e3375-132">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e3375-133">例</span><span class="sxs-lookup"><span data-stu-id="e3375-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e3375-134">要求</span><span class="sxs-lookup"><span data-stu-id="e3375-134">Request</span></span>
<span data-ttu-id="e3375-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e3375-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "patch_channel"
}-->
```http
PATCH https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```
##### <a name="response"></a><span data-ttu-id="e3375-136">応答</span><span class="sxs-lookup"><span data-stu-id="e3375-136">Response</span></span>
<span data-ttu-id="e3375-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e3375-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="e3375-140">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="e3375-140">SDK sample code</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="e3375-141">目的-C</span><span class="sxs-lookup"><span data-stu-id="e3375-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/patch_channel-Objective-C-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Patch channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/channel-patch.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)"
  ]
}-->
