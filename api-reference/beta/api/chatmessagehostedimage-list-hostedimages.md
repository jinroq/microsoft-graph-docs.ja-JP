---
title: chatmessage に chatMessageHostedImages を一覧表示する
description: chatMessage にホストされているすべての画像を一覧表示します。
localization_priority: Priority
author: clearab
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 351e473e0d97ec23c1a4b859d637c40a3e49b7ab
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35943555"
---
# <a name="list-chatmessagehostedimages-in-a-chatmessage"></a><span data-ttu-id="7aed6-103">chatMessage に chatMessageHostedImages を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="7aed6-103">List chatMessageHostedImages in a chatMessage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7aed6-104">[chatMessage](../resources/chatmessage.md) に[ホストされているすべての画像](../resources/chatmessagehostedimage.md)を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="7aed6-104">List all [hosted images](../resources/chatmessagehostedimage.md) in a [chatMessage](../resources/chatmessage.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7aed6-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7aed6-105">Permissions</span></span>

<span data-ttu-id="7aed6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7aed6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7aed6-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7aed6-108">Permission Type</span></span>|<span data-ttu-id="7aed6-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7aed6-109">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="7aed6-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7aed6-110">Delegated (work or school account)</span></span>|<span data-ttu-id="7aed6-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7aed6-111">Group.Read.All, Group.ReadWrite.All</span></span>|
|<span data-ttu-id="7aed6-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7aed6-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7aed6-113">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="7aed6-113">Not supported</span></span>|
|<span data-ttu-id="7aed6-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7aed6-114">Application</span></span>| <span data-ttu-id="7aed6-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7aed6-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7aed6-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7aed6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/{id}/hostedImages
GET /teams/{id}/channels/{id}/messages/{id}/replies/{id}/hostedImages
GET /chats/{id}/messages/{id}/hostedImages
GET /users/{id}/chats/{id}/messages/{id}/hostedImages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7aed6-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="7aed6-117">Optional query parameters</span></span>

<span data-ttu-id="7aed6-118">この操作は、応答をカスタマイズする [OData クエリ パラメーター](/graph/query-parameters)をサポートしていません。</span><span class="sxs-lookup"><span data-stu-id="7aed6-118">This operation does not currently support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7aed6-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7aed6-119">Request headers</span></span>

| <span data-ttu-id="7aed6-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7aed6-120">Header</span></span>       | <span data-ttu-id="7aed6-121">値</span><span class="sxs-lookup"><span data-stu-id="7aed6-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7aed6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7aed6-122">Authorization</span></span>  | <span data-ttu-id="7aed6-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7aed6-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7aed6-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="7aed6-125">Request body</span></span>

<span data-ttu-id="7aed6-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7aed6-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7aed6-127">応答</span><span class="sxs-lookup"><span data-stu-id="7aed6-127">Response</span></span>

<span data-ttu-id="7aed6-128">このメソッドは、成功すると `200 OK` 応答コードと [hostedImage](../resources/chatmessagehostedimage.md) オブジェクトのコレクションを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="7aed6-128">If successful, this method returns a `200 OK` response code and collection of [Message](../resources/chatmessagehostedimage.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7aed6-129">例</span><span class="sxs-lookup"><span data-stu-id="7aed6-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7aed6-130">要求</span><span class="sxs-lookup"><span data-stu-id="7aed6-130">Request</span></span>

<span data-ttu-id="7aed6-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7aed6-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channel_messages"
}-->

```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages/{id}/hostedImages
```

##### <a name="response"></a><span data-ttu-id="7aed6-132">応答</span><span class="sxs-lookup"><span data-stu-id="7aed6-132">Response</span></span>

<span data-ttu-id="7aed6-133">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="7aed6-133">Here is an example of the response.</span></span> 

><span data-ttu-id="7aed6-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="7aed6-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
  "value": [
    {
        "id": "id-value",
        "url": "url-value"
    },
    {
        "id": "id-value",
        "url": "url-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List hosted images in a chatmessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chatmessagehostedimage-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
