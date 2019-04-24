---
title: チャネルを取得する
description: チャネルのプロパティとリレーションシップを取得します。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 51a1d565438deca2c7202b1be8f18b52f1c875f2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32456620"
---
# <a name="get-channel"></a><span data-ttu-id="a0d2e-103">チャネルを取得する</span><span class="sxs-lookup"><span data-stu-id="a0d2e-103">Get channel</span></span>



<span data-ttu-id="a0d2e-104">[チャネル](../resources/channel.md)のプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="a0d2e-104">Retrieve the properties and relationships of a [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a0d2e-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a0d2e-105">Permissions</span></span>
<span data-ttu-id="a0d2e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a0d2e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0d2e-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a0d2e-108">Permission type</span></span>      | <span data-ttu-id="a0d2e-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a0d2e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a0d2e-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a0d2e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a0d2e-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0d2e-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a0d2e-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a0d2e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a0d2e-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a0d2e-113">Not supported.</span></span>    |
|<span data-ttu-id="a0d2e-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a0d2e-114">Application</span></span> | <span data-ttu-id="a0d2e-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0d2e-115">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="a0d2e-116">**注**: この API は、管理者のアクセス許可をサポートします。</span><span class="sxs-lookup"><span data-stu-id="a0d2e-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="a0d2e-117">グローバル管理者と Microsoft Teams サービス管理者は、メンバーではないチームにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="a0d2e-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="a0d2e-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a0d2e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}

```

## <a name="optional-query-parameters"></a><span data-ttu-id="a0d2e-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="a0d2e-119">Optional query parameters</span></span>

<span data-ttu-id="a0d2e-120">このメソッドは、応答をカスタマイズするための $filter、$select、および $expand [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="a0d2e-120">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a0d2e-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a0d2e-121">Request headers</span></span>
| <span data-ttu-id="a0d2e-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a0d2e-122">Header</span></span>       | <span data-ttu-id="a0d2e-123">値</span><span class="sxs-lookup"><span data-stu-id="a0d2e-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a0d2e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a0d2e-124">Authorization</span></span>  | <span data-ttu-id="a0d2e-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a0d2e-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a0d2e-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="a0d2e-127">Request body</span></span>
<span data-ttu-id="a0d2e-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a0d2e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a0d2e-129">応答</span><span class="sxs-lookup"><span data-stu-id="a0d2e-129">Response</span></span>

<span data-ttu-id="a0d2e-130">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[channel](../resources/channel.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a0d2e-130">If successful, this method returns a `200 OK` response code and a [channel](../resources/channel.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a0d2e-131">例</span><span class="sxs-lookup"><span data-stu-id="a0d2e-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a0d2e-132">要求</span><span class="sxs-lookup"><span data-stu-id="a0d2e-132">Request</span></span>
<span data-ttu-id="a0d2e-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a0d2e-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channel"
}-->
```http
GET https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}
```
##### <a name="response"></a><span data-ttu-id="a0d2e-134">応答</span><span class="sxs-lookup"><span data-stu-id="a0d2e-134">Response</span></span>
<span data-ttu-id="a0d2e-135">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="a0d2e-135">Here is an example of the response.</span></span> 

><span data-ttu-id="a0d2e-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="a0d2e-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
