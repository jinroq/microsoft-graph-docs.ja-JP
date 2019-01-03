---
title: チャネルを取得します。
description: プロパティとチャネルの関係を取得します。
author: nkramer
ms.openlocfilehash: e1c5a46b43fcb3245877fba9d8529e9396e62ba8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27322723"
---
# <a name="get-channel"></a><span data-ttu-id="fb552-103">チャネルを取得します。</span><span class="sxs-lookup"><span data-stu-id="fb552-103">Get channel</span></span>

> <span data-ttu-id="fb552-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fb552-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fb552-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fb552-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fb552-106">プロパティと[チャネル](../resources/channel.md)の関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="fb552-106">Retrieve the properties and relationships of a [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="fb552-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="fb552-107">Permissions</span></span>
<span data-ttu-id="fb552-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fb552-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb552-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fb552-110">Permission type</span></span>      | <span data-ttu-id="fb552-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="fb552-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fb552-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fb552-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fb552-113">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb552-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="fb552-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fb552-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fb552-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fb552-115">Not supported.</span></span>    |
|<span data-ttu-id="fb552-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fb552-116">Application</span></span> | <span data-ttu-id="fb552-117">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb552-117">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="fb552-118">**注**: この API は、管理者のアクセス許可をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="fb552-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="fb552-119">グローバル管理者とサービス管理者のマイクロソフトのチームのメンバーではないことをチームにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="fb552-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="fb552-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fb552-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}

```

## <a name="optional-query-parameters"></a><span data-ttu-id="fb552-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="fb552-121">Optional query parameters</span></span>

<span data-ttu-id="fb552-122">このメソッドは、$filter、$select をサポートしていて、$ は、応答をカスタマイズするために[OData クエリ パラメーター](/graph/query-parameters)を展開します。</span><span class="sxs-lookup"><span data-stu-id="fb552-122">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fb552-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fb552-123">Request headers</span></span>
| <span data-ttu-id="fb552-124">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fb552-124">Header</span></span>       | <span data-ttu-id="fb552-125">値</span><span class="sxs-lookup"><span data-stu-id="fb552-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fb552-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="fb552-126">Authorization</span></span>  | <span data-ttu-id="fb552-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="fb552-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fb552-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="fb552-129">Request body</span></span>
<span data-ttu-id="fb552-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="fb552-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fb552-131">応答</span><span class="sxs-lookup"><span data-stu-id="fb552-131">Response</span></span>

<span data-ttu-id="fb552-132">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文の[チャネル](../resources/channel.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="fb552-132">If successful, this method returns a `200 OK` response code and a [channel](../resources/channel.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fb552-133">例</span><span class="sxs-lookup"><span data-stu-id="fb552-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fb552-134">要求</span><span class="sxs-lookup"><span data-stu-id="fb552-134">Request</span></span>
<span data-ttu-id="fb552-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fb552-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channel"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```
##### <a name="response"></a><span data-ttu-id="fb552-136">応答</span><span class="sxs-lookup"><span data-stu-id="fb552-136">Response</span></span>
<span data-ttu-id="fb552-137">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="fb552-137">Here is an example of the response.</span></span> 

><span data-ttu-id="fb552-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="fb552-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->