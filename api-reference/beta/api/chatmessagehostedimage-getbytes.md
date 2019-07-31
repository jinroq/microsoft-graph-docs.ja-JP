---
title: 'chatMessageHostedImage: getBytes'
description: チャネルまたはチャットメッセージ内のホストされた画像のバイナリ表現を取得します。
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 4830e3f845d657e5b073c27e228976bfe9926630
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35943569"
---
# <a name="chatmessagehostedimage-getbytes"></a><span data-ttu-id="3072e-103">chatMessageHostedImage: getBytes</span><span class="sxs-lookup"><span data-stu-id="3072e-103">chatMessageHostedImage: getBytes</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3072e-104">[メッセージ](../resources/chatmessage.md)内のホストされている[イメージ](../resources/chatmessagehostedimage.md)のバイナリ表現を取得します。</span><span class="sxs-lookup"><span data-stu-id="3072e-104">Get the binary representation of a [hosted image](../resources/chatmessagehostedimage.md) in a [message](../resources/chatmessage.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3072e-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3072e-105">Permissions</span></span>

<span data-ttu-id="3072e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3072e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3072e-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3072e-108">Permission Type</span></span>|<span data-ttu-id="3072e-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3072e-109">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="3072e-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3072e-110">Delegated (work or school account)</span></span>|<span data-ttu-id="3072e-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3072e-111">Group.Read.All, Group.ReadWrite.All</span></span>|
|<span data-ttu-id="3072e-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3072e-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3072e-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3072e-113">Not supported.</span></span>|
|<span data-ttu-id="3072e-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3072e-114">Application</span></span>| <span data-ttu-id="3072e-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3072e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3072e-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3072e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/{id}/hostedImages/{id}/$value
GET /teams/{id}/channels/{id}/messages/{id}/replies/{id}/hostedImages/{id}/$value
GET /chats/{id}/messages/{id}/hostedImages/{id}/$value
GET /users/{id}/chats/{id}/messages/{id}/hostedImages/{id}/$value
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3072e-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="3072e-117">Optional query parameters</span></span>

<span data-ttu-id="3072e-118">このメソッドは、応答をカスタマイズするための[OData クエリパラメーター](/graph/query-parameters)をサポートしていません。</span><span class="sxs-lookup"><span data-stu-id="3072e-118">This method does not support the [OData Query Parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3072e-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3072e-119">Request headers</span></span>

| <span data-ttu-id="3072e-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3072e-120">Header</span></span>       | <span data-ttu-id="3072e-121">値</span><span class="sxs-lookup"><span data-stu-id="3072e-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3072e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3072e-122">Authorization</span></span>  | <span data-ttu-id="3072e-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3072e-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3072e-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="3072e-125">Request body</span></span>

<span data-ttu-id="3072e-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="3072e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3072e-127">応答</span><span class="sxs-lookup"><span data-stu-id="3072e-127">Response</span></span>

<span data-ttu-id="3072e-128">成功した場合、このメソッド`200 OK`は応答コードと、要求されたイメージのバイナリデータを返します。</span><span class="sxs-lookup"><span data-stu-id="3072e-128">If successful, this method returns a `200 OK` response code and binary data of the requested image.</span></span>

## <a name="example"></a><span data-ttu-id="3072e-129">例</span><span class="sxs-lookup"><span data-stu-id="3072e-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3072e-130">要求</span><span class="sxs-lookup"><span data-stu-id="3072e-130">Request</span></span>

<span data-ttu-id="3072e-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3072e-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channel_message"
}-->

```http
GET /teams/{id}/channels/{id}/messages/{id}/hostedImages/{id}/$value
```

##### <a name="response"></a><span data-ttu-id="3072e-132">応答</span><span class="sxs-lookup"><span data-stu-id="3072e-132">Response</span></span>

<span data-ttu-id="3072e-133">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="3072e-133">Here is an example of the response.</span></span>

><span data-ttu-id="3072e-134">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="3072e-134">**Note:** The response object shown here is shortened for readability.</span></span> <span data-ttu-id="3072e-135">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="3072e-135">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: image/jpeg
Content-length: 201
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get bytes of a hosted image",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chatmessagehostedimage-getbytes.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
