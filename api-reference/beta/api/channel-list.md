---
title: チャネルのリスト
description: このチーム内のチャンネルのリストを取得します。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 6900b0a64721556b5020baee197e4c7f78d90278
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27936166"
---
# <a name="list-channels"></a><span data-ttu-id="18a16-103">チャネルのリスト</span><span class="sxs-lookup"><span data-stu-id="18a16-103">List channels</span></span>

> <span data-ttu-id="18a16-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="18a16-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="18a16-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="18a16-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="18a16-106">このチーム内[のチャネル](../resources/channel.md)のリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="18a16-106">Retrieve the list of [channels](../resources/channel.md) in this team.</span></span>

## <a name="permissions"></a><span data-ttu-id="18a16-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="18a16-107">Permissions</span></span>
<span data-ttu-id="18a16-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="18a16-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="18a16-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="18a16-110">Permission type</span></span>      | <span data-ttu-id="18a16-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="18a16-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18a16-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="18a16-112">Delegated (work or school account)</span></span> | <span data-ttu-id="18a16-113">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18a16-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="18a16-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="18a16-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18a16-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="18a16-115">Not supported.</span></span>    |
|<span data-ttu-id="18a16-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="18a16-116">Application</span></span> | <span data-ttu-id="18a16-117">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18a16-117">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="18a16-118">**注**: この API は、管理者のアクセス許可をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="18a16-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="18a16-119">グローバル管理者とサービス管理者のマイクロソフトのチームのメンバーではないことをチームにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="18a16-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="18a16-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="18a16-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels
```

## <a name="optional-query-parameters"></a><span data-ttu-id="18a16-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="18a16-121">Optional query parameters</span></span>
<span data-ttu-id="18a16-122">このメソッドは、$filter、$select をサポートしていて、$ は、応答をカスタマイズするために[OData クエリ パラメーター](/graph/query-parameters)を展開します。</span><span class="sxs-lookup"><span data-stu-id="18a16-122">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="18a16-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="18a16-123">Request headers</span></span>
| <span data-ttu-id="18a16-124">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="18a16-124">Header</span></span>       | <span data-ttu-id="18a16-125">値</span><span class="sxs-lookup"><span data-stu-id="18a16-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="18a16-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="18a16-126">Authorization</span></span>  | <span data-ttu-id="18a16-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="18a16-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="18a16-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="18a16-129">Request body</span></span>
<span data-ttu-id="18a16-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="18a16-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="18a16-131">応答</span><span class="sxs-lookup"><span data-stu-id="18a16-131">Response</span></span>

<span data-ttu-id="18a16-132">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に、[チャネル](../resources/channel.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="18a16-132">If successful, this method returns a `200 OK` response code and collection of [Channel](../resources/channel.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18a16-133">例</span><span class="sxs-lookup"><span data-stu-id="18a16-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="18a16-134">要求</span><span class="sxs-lookup"><span data-stu-id="18a16-134">Request</span></span>
<span data-ttu-id="18a16-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="18a16-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channels"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels
```
##### <a name="response"></a><span data-ttu-id="18a16-136">応答</span><span class="sxs-lookup"><span data-stu-id="18a16-136">Response</span></span>
<span data-ttu-id="18a16-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="18a16-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
