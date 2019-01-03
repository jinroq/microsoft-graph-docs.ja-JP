---
title: チームを取得します。
description: プロパティと指定されたチームの関係を取得します。
author: nkramer
ms.openlocfilehash: dfa59948a9bffce77c98a3462f919e75fe18042e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27329233"
---
# <a name="get-team"></a><span data-ttu-id="f9f9c-103">チームを取得します。</span><span class="sxs-lookup"><span data-stu-id="f9f9c-103">Get team</span></span>

> <span data-ttu-id="f9f9c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f9f9c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f9f9c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f9f9c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f9f9c-106">プロパティと指定した[チーム](../resources/team.md)の関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="f9f9c-106">Retrieve the properties and relationships of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f9f9c-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f9f9c-107">Permissions</span></span>
<span data-ttu-id="f9f9c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f9f9c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9f9c-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f9f9c-110">Permission type</span></span>      | <span data-ttu-id="f9f9c-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f9f9c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f9f9c-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f9f9c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f9f9c-113">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9f9c-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f9f9c-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f9f9c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9f9c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f9f9c-115">Not supported.</span></span>    |
|<span data-ttu-id="f9f9c-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f9f9c-116">Application</span></span> | <span data-ttu-id="f9f9c-117">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9f9c-117">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="f9f9c-118">**注**: この API は、管理者のアクセス許可をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="f9f9c-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="f9f9c-119">グローバル管理者とサービス管理者のマイクロソフトのチームのメンバーではないことをチームにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="f9f9c-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="f9f9c-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f9f9c-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f9f9c-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="f9f9c-121">Optional query parameters</span></span>
<span data-ttu-id="f9f9c-122">このメソッドは、$select をサポートし、$ は、応答をカスタマイズするために[OData クエリ パラメーター](/graph/query-parameters)を展開します。</span><span class="sxs-lookup"><span data-stu-id="f9f9c-122">This method supports the $select and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f9f9c-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f9f9c-123">Request headers</span></span>
| <span data-ttu-id="f9f9c-124">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f9f9c-124">Header</span></span>       | <span data-ttu-id="f9f9c-125">値</span><span class="sxs-lookup"><span data-stu-id="f9f9c-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f9f9c-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="f9f9c-126">Authorization</span></span>  | <span data-ttu-id="f9f9c-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f9f9c-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f9f9c-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="f9f9c-129">Request body</span></span>
<span data-ttu-id="f9f9c-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f9f9c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f9f9c-131">応答</span><span class="sxs-lookup"><span data-stu-id="f9f9c-131">Response</span></span>

<span data-ttu-id="f9f9c-132">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文の[チーム](../resources/team.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="f9f9c-132">If successful, this method returns a `200 OK` response code and a [team](../resources/team.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f9f9c-133">例</span><span class="sxs-lookup"><span data-stu-id="f9f9c-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="f9f9c-134">要求</span><span class="sxs-lookup"><span data-stu-id="f9f9c-134">Request</span></span>
<span data-ttu-id="f9f9c-135">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f9f9c-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}
```
#### <a name="response"></a><span data-ttu-id="f9f9c-136">応答</span><span class="sxs-lookup"><span data-stu-id="f9f9c-136">Response</span></span>
<span data-ttu-id="f9f9c-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f9f9c-137">The following is an example of the response.</span></span> 

><span data-ttu-id="f9f9c-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="f9f9c-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "isArchived" : false,
  "memberSettings": {
    "allowCreateUpdateChannels": true,
    "allowDeleteChannels": true,
    "allowAddRemoveApps": true,
    "allowCreateUpdateRemoveTabs": true,
    "allowCreateUpdateRemoveConnectors": true    
  },
  "guestSettings": {
    "allowCreateUpdateChannels": true,
    "allowDeleteChannels": true 
  },
  "messagingSettings": {
    "allowUserEditMessages": true,
    "allowUserDeleteMessages": true,
    "allowOwnerDeleteMessages": true,
    "allowTeamMentions": true,
    "allowChannelMentions": true    
  },
  "funSettings": {
    "allowGiphy": true,
    "giphyContentRating": "strict",
    "allowStickersAndMemes": true,
    "allowCustomMemes": true
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->