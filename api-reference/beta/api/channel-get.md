---
title: チャネルを取得する
description: チャネルのプロパティと関係を取得します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: a217f83cc9ab039e990af2cada53919d00b296dc
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33635478"
---
# <a name="get-channel"></a><span data-ttu-id="1c99c-103">チャネルを取得する</span><span class="sxs-lookup"><span data-stu-id="1c99c-103">Get channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c99c-104">[チャネル](../resources/channel.md)のプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="1c99c-104">Retrieve the properties and relationships of a [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1c99c-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1c99c-105">Permissions</span></span>
<span data-ttu-id="1c99c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1c99c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c99c-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1c99c-108">Permission type</span></span>      | <span data-ttu-id="1c99c-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1c99c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1c99c-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1c99c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1c99c-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c99c-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1c99c-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1c99c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c99c-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1c99c-113">Not supported.</span></span>    |
|<span data-ttu-id="1c99c-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1c99c-114">Application</span></span> | <span data-ttu-id="1c99c-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c99c-115">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="1c99c-116">**注**: この API は、管理者のアクセス許可をサポートします。</span><span class="sxs-lookup"><span data-stu-id="1c99c-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="1c99c-117">グローバル管理者と Microsoft Teams サービス管理者は、メンバーではないチームにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="1c99c-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="1c99c-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1c99c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}

```

## <a name="optional-query-parameters"></a><span data-ttu-id="1c99c-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="1c99c-119">Optional query parameters</span></span>

<span data-ttu-id="1c99c-120">このメソッドは、応答をカスタマイズするための $filter、$select、および $expand [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="1c99c-120">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1c99c-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1c99c-121">Request headers</span></span>
| <span data-ttu-id="1c99c-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1c99c-122">Header</span></span>       | <span data-ttu-id="1c99c-123">値</span><span class="sxs-lookup"><span data-stu-id="1c99c-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1c99c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1c99c-124">Authorization</span></span>  | <span data-ttu-id="1c99c-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1c99c-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1c99c-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="1c99c-127">Request body</span></span>
<span data-ttu-id="1c99c-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1c99c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c99c-129">応答</span><span class="sxs-lookup"><span data-stu-id="1c99c-129">Response</span></span>

<span data-ttu-id="1c99c-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [channel](../resources/channel.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1c99c-130">If successful, this method returns a `200 OK` response code and a [channel](../resources/channel.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1c99c-131">例</span><span class="sxs-lookup"><span data-stu-id="1c99c-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1c99c-132">要求</span><span class="sxs-lookup"><span data-stu-id="1c99c-132">Request</span></span>
<span data-ttu-id="1c99c-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1c99c-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channel"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```
##### <a name="response"></a><span data-ttu-id="1c99c-134">応答</span><span class="sxs-lookup"><span data-stu-id="1c99c-134">Response</span></span>
<span data-ttu-id="1c99c-135">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="1c99c-135">Here is an example of the response.</span></span> 

><span data-ttu-id="1c99c-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="1c99c-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "id": "id-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="1c99c-138">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="1c99c-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1c99c-139">Visual</span><span class="sxs-lookup"><span data-stu-id="1c99c-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_channel-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1c99c-140">Java</span><span class="sxs-lookup"><span data-stu-id="1c99c-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_channel-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/channel-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/channel-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
