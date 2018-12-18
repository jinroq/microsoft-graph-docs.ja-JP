---
title: チャネルのリスト
description: このチーム内のチャンネルのリストを取得します。
author: nkramer
ms.openlocfilehash: a09a4a25fb2324726bd7d8a8ac62290cfc3c5f92
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27307400"
---
# <a name="list-channels"></a><span data-ttu-id="f21d4-103">チャネルのリスト</span><span class="sxs-lookup"><span data-stu-id="f21d4-103">List channels</span></span>



<span data-ttu-id="f21d4-104">このチーム内[のチャネル](../resources/channel.md)のリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="f21d4-104">Retrieve the list of [channels](../resources/channel.md) in this team.</span></span>

## <a name="permissions"></a><span data-ttu-id="f21d4-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f21d4-105">Permissions</span></span>
<span data-ttu-id="f21d4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f21d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f21d4-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f21d4-108">Permission type</span></span>      | <span data-ttu-id="f21d4-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f21d4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f21d4-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f21d4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f21d4-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f21d4-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f21d4-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f21d4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f21d4-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f21d4-113">Not supported.</span></span>    |
|<span data-ttu-id="f21d4-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f21d4-114">Application</span></span> | <span data-ttu-id="f21d4-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f21d4-115">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="f21d4-116">**注**: この API は、管理者のアクセス許可をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="f21d4-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="f21d4-117">グローバル管理者とサービス管理者のマイクロソフトのチームのメンバーではないことをチームにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="f21d4-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="f21d4-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f21d4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f21d4-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="f21d4-119">Optional query parameters</span></span>
<span data-ttu-id="f21d4-120">このメソッドは、$filter、$select をサポートしていて、$ は、応答をカスタマイズするために[OData クエリ パラメーター](/graph/query-parameters)を展開します。</span><span class="sxs-lookup"><span data-stu-id="f21d4-120">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f21d4-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f21d4-121">Request headers</span></span>
| <span data-ttu-id="f21d4-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f21d4-122">Header</span></span>       | <span data-ttu-id="f21d4-123">値</span><span class="sxs-lookup"><span data-stu-id="f21d4-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f21d4-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f21d4-124">Authorization</span></span>  | <span data-ttu-id="f21d4-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f21d4-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f21d4-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="f21d4-127">Request body</span></span>
<span data-ttu-id="f21d4-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f21d4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f21d4-129">応答</span><span class="sxs-lookup"><span data-stu-id="f21d4-129">Response</span></span>

<span data-ttu-id="f21d4-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に、[チャネル](../resources/channel.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="f21d4-130">If successful, this method returns a `200 OK` response code and collection of [Channel](../resources/channel.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f21d4-131">例</span><span class="sxs-lookup"><span data-stu-id="f21d4-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f21d4-132">要求</span><span class="sxs-lookup"><span data-stu-id="f21d4-132">Request</span></span>
<span data-ttu-id="f21d4-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f21d4-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channels"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels
```
##### <a name="response"></a><span data-ttu-id="f21d4-134">応答</span><span class="sxs-lookup"><span data-stu-id="f21d4-134">Response</span></span>
<span data-ttu-id="f21d4-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f21d4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
