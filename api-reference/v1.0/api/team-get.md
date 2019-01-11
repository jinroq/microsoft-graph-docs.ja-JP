---
title: チームを取得します。
description: プロパティと指定されたチームの関係を取得します。
author: nkramer
localization_priority: Priority
ms.openlocfilehash: 3efec6e9b767d026d0a7626c2da257feaa20fde3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27887081"
---
# <a name="get-team"></a><span data-ttu-id="96e6a-103">チームを取得します。</span><span class="sxs-lookup"><span data-stu-id="96e6a-103">Get team</span></span>



<span data-ttu-id="96e6a-104">プロパティと指定した[チーム](../resources/team.md)の関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="96e6a-104">Retrieve the properties and relationships of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="96e6a-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="96e6a-105">Permissions</span></span>
<span data-ttu-id="96e6a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="96e6a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96e6a-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="96e6a-108">Permission type</span></span>      | <span data-ttu-id="96e6a-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="96e6a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="96e6a-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="96e6a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="96e6a-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96e6a-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="96e6a-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="96e6a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96e6a-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="96e6a-113">Not supported.</span></span>    |
|<span data-ttu-id="96e6a-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="96e6a-114">Application</span></span> | <span data-ttu-id="96e6a-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96e6a-115">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="96e6a-116">**注**: この API は、管理者のアクセス許可をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="96e6a-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="96e6a-117">グローバル管理者とサービス管理者のマイクロソフトのチームのメンバーではないことをチームにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="96e6a-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="96e6a-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="96e6a-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="96e6a-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="96e6a-119">Optional query parameters</span></span>
<span data-ttu-id="96e6a-120">このメソッドは、$select をサポートし、$ は、応答をカスタマイズするために[OData クエリ パラメーター](/graph/query-parameters)を展開します。</span><span class="sxs-lookup"><span data-stu-id="96e6a-120">This method supports the $select and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="96e6a-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="96e6a-121">Request headers</span></span>
| <span data-ttu-id="96e6a-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="96e6a-122">Header</span></span>       | <span data-ttu-id="96e6a-123">値</span><span class="sxs-lookup"><span data-stu-id="96e6a-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="96e6a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="96e6a-124">Authorization</span></span>  | <span data-ttu-id="96e6a-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="96e6a-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="96e6a-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="96e6a-127">Request body</span></span>
<span data-ttu-id="96e6a-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="96e6a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96e6a-129">応答</span><span class="sxs-lookup"><span data-stu-id="96e6a-129">Response</span></span>

<span data-ttu-id="96e6a-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文の[チーム](../resources/team.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="96e6a-130">If successful, this method returns a `200 OK` response code and a [team](../resources/team.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="96e6a-131">例</span><span class="sxs-lookup"><span data-stu-id="96e6a-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="96e6a-132">要求</span><span class="sxs-lookup"><span data-stu-id="96e6a-132">Request</span></span>
<span data-ttu-id="96e6a-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="96e6a-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}
```
#### <a name="response"></a><span data-ttu-id="96e6a-134">応答</span><span class="sxs-lookup"><span data-stu-id="96e6a-134">Response</span></span>
<span data-ttu-id="96e6a-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="96e6a-135">The following is an example of the response.</span></span> 

><span data-ttu-id="96e6a-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="96e6a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
