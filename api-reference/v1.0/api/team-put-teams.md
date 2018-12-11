---
title: チームを作成します。
description: グループの下の新しいチームを作成します。
ms.openlocfilehash: d7afffb331bf4a1714083ebb5f95147ec48a65d0
ms.sourcegitcommit: 72d4da2a6bfaf99fa4edaf6ce3b97b1a6d96d874
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/11/2018
ms.locfileid: "27222549"
---
# <a name="create-team"></a><span data-ttu-id="6d0ec-103">チームを作成します。</span><span class="sxs-lookup"><span data-stu-id="6d0ec-103">Create team</span></span>



<span data-ttu-id="6d0ec-104">[グループ](../resources/group.md)の下に新しい[チーム](../resources/team.md)を作成します。</span><span class="sxs-lookup"><span data-stu-id="6d0ec-104">Create a new [team](../resources/team.md) under a [group](../resources/group.md).</span></span>

<span data-ttu-id="6d0ec-105">グループには、チームを作成するために少なくとも 1 人の所有者が必要です。</span><span class="sxs-lookup"><span data-stu-id="6d0ec-105">In order to create a team, the group must have a least one owner.</span></span>

<span data-ttu-id="6d0ec-106">グループは 15 分未満で作成されている場合は、作成チームの呼び出しが失敗し、レプリケーションの遅延のための 404 エラー コード可能性があります。</span><span class="sxs-lookup"><span data-stu-id="6d0ec-106">If the group was created less than 15 minutes ago, it's possible for the Create team call to fail with a 404 error code due to replication delays.</span></span> <span data-ttu-id="6d0ec-107">推奨のパターンでは、呼び出しの間で 10 秒の遅延で 3 回を作成するチームの呼び出しを再試行します。</span><span class="sxs-lookup"><span data-stu-id="6d0ec-107">The recommended pattern is to retry the Create team call three times, with a 10 second delay between calls.</span></span>

## <a name="permissions"></a><span data-ttu-id="6d0ec-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6d0ec-108">Permissions</span></span>

<span data-ttu-id="6d0ec-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6d0ec-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d0ec-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6d0ec-111">Permission type</span></span>      | <span data-ttu-id="6d0ec-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6d0ec-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6d0ec-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6d0ec-113">Delegated (work or school account)</span></span> | <span data-ttu-id="6d0ec-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d0ec-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="6d0ec-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6d0ec-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6d0ec-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6d0ec-116">Not supported.</span></span>    |
|<span data-ttu-id="6d0ec-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6d0ec-117">Application</span></span> | <span data-ttu-id="6d0ec-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d0ec-118">Group.ReadWrite.All</span></span> |

> <span data-ttu-id="6d0ec-119">**注**: この API は、管理者のアクセス許可をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="6d0ec-119">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="6d0ec-120">グローバル管理者およびマイクロソフトのチームのサービス管理者グループのメンバーではないことにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="6d0ec-120">Global admins and Microsoft Teams service admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="6d0ec-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6d0ec-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /groups/{id}/team
```

## <a name="request-headers"></a><span data-ttu-id="6d0ec-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6d0ec-122">Request headers</span></span>

| <span data-ttu-id="6d0ec-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6d0ec-123">Header</span></span>       | <span data-ttu-id="6d0ec-124">値</span><span class="sxs-lookup"><span data-stu-id="6d0ec-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6d0ec-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="6d0ec-125">Authorization</span></span>  | <span data-ttu-id="6d0ec-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6d0ec-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6d0ec-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6d0ec-128">Content-Type</span></span>  | <span data-ttu-id="6d0ec-129">application/json</span><span class="sxs-lookup"><span data-stu-id="6d0ec-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6d0ec-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="6d0ec-130">Request body</span></span>

<span data-ttu-id="6d0ec-131">要求の本体で、[チーム](../resources/team.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="6d0ec-131">In the request body, supply a JSON representation of a [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="6d0ec-132">応答</span><span class="sxs-lookup"><span data-stu-id="6d0ec-132">Response</span></span>

<span data-ttu-id="6d0ec-133">成功すると、このメソッドを返します、`201 Created`応答コードおよび応答の本文の[チーム](../resources/team.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="6d0ec-133">If successful, this method should return a `201 Created` response code and a [team](../resources/team.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d0ec-134">例</span><span class="sxs-lookup"><span data-stu-id="6d0ec-134">Example</span></span>

#### <a name="request"></a><span data-ttu-id="6d0ec-135">要求</span><span class="sxs-lookup"><span data-stu-id="6d0ec-135">Request</span></span>

<span data-ttu-id="6d0ec-136">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6d0ec-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "create_team"
}-->
```http
PUT https://graph.microsoft.com/v1.0/groups/{id}/team
Content-type: application/json

{  
  "memberSettings": {
    "allowCreateUpdateChannels": true
  },
  "messagingSettings": {
    "allowUserEditMessages": true,
    "allowUserDeleteMessages": true
  },
  "funSettings": {
    "allowGiphy": true,
    "giphyContentRating": "strict"
  }
}
```

#### <a name="response"></a><span data-ttu-id="6d0ec-137">応答</span><span class="sxs-lookup"><span data-stu-id="6d0ec-137">Response</span></span>

<span data-ttu-id="6d0ec-138">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6d0ec-138">The following is an example of the response.</span></span> 

><span data-ttu-id="6d0ec-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="6d0ec-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 401

{
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
  "description": "Create Team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

## <a name="see-also"></a><span data-ttu-id="6d0ec-141">関連項目</span><span class="sxs-lookup"><span data-stu-id="6d0ec-141">See also</span></span>

- [<span data-ttu-id="6d0ec-142">チームのグループを作成</span><span class="sxs-lookup"><span data-stu-id="6d0ec-142">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)
