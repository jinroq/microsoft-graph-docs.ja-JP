---
title: チャネルを取得します。
description: プロパティとチャネルの関係を取得します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 51a1d565438deca2c7202b1be8f18b52f1c875f2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528887"
---
# <a name="get-channel"></a><span data-ttu-id="a2397-103">チャネルを取得します。</span><span class="sxs-lookup"><span data-stu-id="a2397-103">Get channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2397-104">プロパティと[チャネル](../resources/channel.md)の関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="a2397-104">Retrieve the properties and relationships of a [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a2397-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a2397-105">Permissions</span></span>
<span data-ttu-id="a2397-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a2397-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2397-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a2397-108">Permission type</span></span>      | <span data-ttu-id="a2397-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a2397-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a2397-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a2397-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a2397-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2397-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a2397-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a2397-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a2397-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a2397-113">Not supported.</span></span>    |
|<span data-ttu-id="a2397-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a2397-114">Application</span></span> | <span data-ttu-id="a2397-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2397-115">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="a2397-116">**注**: この API は、管理者のアクセス許可をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="a2397-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="a2397-117">グローバル管理者とサービス管理者のマイクロソフトのチームのメンバーではないことをチームにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="a2397-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="a2397-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a2397-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}

```

## <a name="optional-query-parameters"></a><span data-ttu-id="a2397-119">省略可能なクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="a2397-119">Optional query parameters</span></span>

<span data-ttu-id="a2397-120">このメソッドは、$filter、$select をサポートしていて、$ は、応答をカスタマイズするために[OData クエリ パラメーター](/graph/query-parameters)を展開します。</span><span class="sxs-lookup"><span data-stu-id="a2397-120">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a2397-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a2397-121">Request headers</span></span>
| <span data-ttu-id="a2397-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a2397-122">Header</span></span>       | <span data-ttu-id="a2397-123">値</span><span class="sxs-lookup"><span data-stu-id="a2397-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a2397-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2397-124">Authorization</span></span>  | <span data-ttu-id="a2397-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a2397-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a2397-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="a2397-127">Request body</span></span>
<span data-ttu-id="a2397-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a2397-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a2397-129">応答</span><span class="sxs-lookup"><span data-stu-id="a2397-129">Response</span></span>

<span data-ttu-id="a2397-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文の[チャネル](../resources/channel.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="a2397-130">If successful, this method returns a `200 OK` response code and a [channel](../resources/channel.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a2397-131">例</span><span class="sxs-lookup"><span data-stu-id="a2397-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a2397-132">要求</span><span class="sxs-lookup"><span data-stu-id="a2397-132">Request</span></span>
<span data-ttu-id="a2397-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a2397-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channel"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```
##### <a name="response"></a><span data-ttu-id="a2397-134">応答</span><span class="sxs-lookup"><span data-stu-id="a2397-134">Response</span></span>
<span data-ttu-id="a2397-135">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="a2397-135">Here is an example of the response.</span></span> 

><span data-ttu-id="a2397-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="a2397-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/channel-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
