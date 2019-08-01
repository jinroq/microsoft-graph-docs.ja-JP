---
title: チームを作成する
description: グループの下に新しいチームを作成します。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 53651a230a6ab6a9d45fb37ec1b587d43aa07e4d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36021173"
---
# <a name="create-team"></a><span data-ttu-id="0631f-103">チームを作成する</span><span class="sxs-lookup"><span data-stu-id="0631f-103">Create team</span></span>



<span data-ttu-id="0631f-104">[グループ](../resources/group.md)の下に新しい[チーム](../resources/team.md)を作成します。</span><span class="sxs-lookup"><span data-stu-id="0631f-104">Create a new [team](../resources/team.md) under a [group](../resources/group.md).</span></span>

<span data-ttu-id="0631f-105">チームを作成するために、グループには少なくとも 1 人の所有者が必要です。</span><span class="sxs-lookup"><span data-stu-id="0631f-105">In order to create a team, the group must have a least one owner.</span></span>

<span data-ttu-id="0631f-106">グループが作成されて 15 分以上経っていない場合は、レプリケーションの遅延のためにチーム作成の呼び出しが失敗し、404 エラー コードが表示される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="0631f-106">If the group was created less than 15 minutes ago, it's possible for the Create team call to fail with a 404 error code due to replication delays.</span></span> <span data-ttu-id="0631f-107">呼び出しと呼び出しの間に 10 秒の遅延を設けて、チーム作成の呼び出しを 3 回再試行するパターンをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="0631f-107">The recommended pattern is to retry the Create team call three times, with a 10 second delay between calls.</span></span>

## <a name="permissions"></a><span data-ttu-id="0631f-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0631f-108">Permissions</span></span>

<span data-ttu-id="0631f-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0631f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0631f-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0631f-111">Permission type</span></span>      | <span data-ttu-id="0631f-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0631f-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0631f-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0631f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="0631f-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0631f-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="0631f-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0631f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0631f-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0631f-116">Not supported.</span></span>    |
|<span data-ttu-id="0631f-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0631f-117">Application</span></span> | <span data-ttu-id="0631f-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0631f-118">Group.ReadWrite.All</span></span> |

> <span data-ttu-id="0631f-119">**注**: この API は、管理者のアクセス許可をサポートします。</span><span class="sxs-lookup"><span data-stu-id="0631f-119">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="0631f-120">グローバル管理者と Microsoft Teams サービス管理者は、メンバーではないグループにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="0631f-120">Global admins and Microsoft Teams service admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="0631f-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0631f-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /groups/{id}/team
```

## <a name="request-headers"></a><span data-ttu-id="0631f-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0631f-122">Request headers</span></span>

| <span data-ttu-id="0631f-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0631f-123">Header</span></span>       | <span data-ttu-id="0631f-124">値</span><span class="sxs-lookup"><span data-stu-id="0631f-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0631f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="0631f-125">Authorization</span></span>  | <span data-ttu-id="0631f-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0631f-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0631f-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0631f-128">Content-Type</span></span>  | <span data-ttu-id="0631f-129">application/json</span><span class="sxs-lookup"><span data-stu-id="0631f-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0631f-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="0631f-130">Request body</span></span>

<span data-ttu-id="0631f-131">要求本文で、[team](../resources/team.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="0631f-131">In the request body, supply a JSON representation of a [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="0631f-132">応答</span><span class="sxs-lookup"><span data-stu-id="0631f-132">Response</span></span>

<span data-ttu-id="0631f-133">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [team](../resources/team.md) オブジェクトを返す必要があります。</span><span class="sxs-lookup"><span data-stu-id="0631f-133">If successful, this method should return a `201 Created` response code and a [team](../resources/team.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0631f-134">例</span><span class="sxs-lookup"><span data-stu-id="0631f-134">Example</span></span>

#### <a name="request"></a><span data-ttu-id="0631f-135">要求</span><span class="sxs-lookup"><span data-stu-id="0631f-135">Request</span></span>

<span data-ttu-id="0631f-136">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0631f-136">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0631f-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="0631f-137">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="0631f-138">C#</span><span class="sxs-lookup"><span data-stu-id="0631f-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0631f-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="0631f-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0631f-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0631f-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0631f-141">Java</span><span class="sxs-lookup"><span data-stu-id="0631f-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0631f-142">応答</span><span class="sxs-lookup"><span data-stu-id="0631f-142">Response</span></span>

<span data-ttu-id="0631f-143">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0631f-143">The following is an example of the response.</span></span> 

><span data-ttu-id="0631f-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="0631f-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
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

## <a name="see-also"></a><span data-ttu-id="0631f-146">関連項目</span><span class="sxs-lookup"><span data-stu-id="0631f-146">See also</span></span>

- [<span data-ttu-id="0631f-147">チームを使用してグループを作成する</span><span class="sxs-lookup"><span data-stu-id="0631f-147">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)
