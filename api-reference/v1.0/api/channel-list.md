---
title: チャネルのリスト
description: このチーム内のチャンネルのリストを取得します。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 9d6d149a0e38fb5e02a2c32f9ad218fb95f32911
ms.sourcegitcommit: 2c60e38bb1b71ba958659f66ad4736495e520851
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/15/2019
ms.locfileid: "28016647"
---
# <a name="list-channels"></a><span data-ttu-id="5bdfe-103">チャネルのリスト</span><span class="sxs-lookup"><span data-stu-id="5bdfe-103">List channels</span></span>



<span data-ttu-id="5bdfe-104">このチーム内[のチャネル](../resources/channel.md)のリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="5bdfe-104">Retrieve the list of [channels](../resources/channel.md) in this team.</span></span>

## <a name="permissions"></a><span data-ttu-id="5bdfe-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5bdfe-105">Permissions</span></span>
<span data-ttu-id="5bdfe-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5bdfe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5bdfe-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5bdfe-108">Permission type</span></span>      | <span data-ttu-id="5bdfe-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5bdfe-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5bdfe-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5bdfe-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5bdfe-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5bdfe-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5bdfe-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5bdfe-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5bdfe-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5bdfe-113">Not supported.</span></span>    |
|<span data-ttu-id="5bdfe-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5bdfe-114">Application</span></span> | <span data-ttu-id="5bdfe-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5bdfe-115">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="5bdfe-116">**注**: この API は、管理者のアクセス許可をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="5bdfe-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="5bdfe-117">グローバル管理者とサービス管理者のマイクロソフトのチームのメンバーではないことをチームにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="5bdfe-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="5bdfe-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5bdfe-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5bdfe-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="5bdfe-119">Optional query parameters</span></span>
<span data-ttu-id="5bdfe-120">このメソッドは、$filter、$select をサポートしていて、$ は、応答をカスタマイズするために[OData クエリ パラメーター](/graph/query-parameters)を展開します。</span><span class="sxs-lookup"><span data-stu-id="5bdfe-120">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5bdfe-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5bdfe-121">Request headers</span></span>
| <span data-ttu-id="5bdfe-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5bdfe-122">Header</span></span>       | <span data-ttu-id="5bdfe-123">値</span><span class="sxs-lookup"><span data-stu-id="5bdfe-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5bdfe-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5bdfe-124">Authorization</span></span>  | <span data-ttu-id="5bdfe-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5bdfe-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5bdfe-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="5bdfe-127">Request body</span></span>
<span data-ttu-id="5bdfe-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="5bdfe-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5bdfe-129">応答</span><span class="sxs-lookup"><span data-stu-id="5bdfe-129">Response</span></span>

<span data-ttu-id="5bdfe-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に、[チャネル](../resources/channel.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="5bdfe-130">If successful, this method returns a `200 OK` response code and collection of [Channel](../resources/channel.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5bdfe-131">例</span><span class="sxs-lookup"><span data-stu-id="5bdfe-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5bdfe-132">要求</span><span class="sxs-lookup"><span data-stu-id="5bdfe-132">Request</span></span>
<span data-ttu-id="5bdfe-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5bdfe-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channels"
}-->
```http
GET https://graph.microsoft.com/v1.0/teams/{id}/channels
```
##### <a name="response"></a><span data-ttu-id="5bdfe-134">応答</span><span class="sxs-lookup"><span data-stu-id="5bdfe-134">Response</span></span>
<span data-ttu-id="5bdfe-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5bdfe-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 262

{
  "value": [
    {
      "description": "description-value",
      "displayName": "display-name-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List channels",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
