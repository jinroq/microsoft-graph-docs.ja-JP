# <a name="create-team"></a><span data-ttu-id="ee26b-101">チームを作成します。</span><span class="sxs-lookup"><span data-stu-id="ee26b-101">Create team</span></span>



<span data-ttu-id="ee26b-102">[グループ](../resources/group.md)の下に新しい[チーム](../resources/team.md)を作成します。</span><span class="sxs-lookup"><span data-stu-id="ee26b-102">Create a new [team](../resources/team.md) under a [group](../resources/group.md).</span></span>

<span data-ttu-id="ee26b-103">グループには、チームを作成するために少なくとも 1 人の所有者が必要です。</span><span class="sxs-lookup"><span data-stu-id="ee26b-103">In order to create a team, the group must have a least one owner.</span></span>

<span data-ttu-id="ee26b-104">グループは 15 分未満で作成されている場合は、作成チームの呼び出しが失敗し、レプリケーションの遅延のための 404 エラー コード可能性があります。</span><span class="sxs-lookup"><span data-stu-id="ee26b-104">If the group was created less than 15 minutes ago, it's possible for the Create team call to fail with a 404 error code due to replication delays.</span></span> <span data-ttu-id="ee26b-105">推奨のパターンでは、呼び出しの間で 10 秒の遅延で 3 回を作成するチームの呼び出しを再試行します。</span><span class="sxs-lookup"><span data-stu-id="ee26b-105">The recommended pattern is to retry the Create team call three times, with a 10 second delay between calls.</span></span>

## <a name="permissions"></a><span data-ttu-id="ee26b-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ee26b-106">Permissions</span></span>

<span data-ttu-id="ee26b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ee26b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ee26b-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ee26b-109">Permission type</span></span>      | <span data-ttu-id="ee26b-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ee26b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ee26b-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ee26b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ee26b-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee26b-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ee26b-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ee26b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee26b-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ee26b-114">Not supported.</span></span>    |
|<span data-ttu-id="ee26b-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ee26b-115">Application</span></span> | <span data-ttu-id="ee26b-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee26b-116">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ee26b-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ee26b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /groups/{id}/team
```

## <a name="request-headers"></a><span data-ttu-id="ee26b-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ee26b-118">Request headers</span></span>

| <span data-ttu-id="ee26b-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ee26b-119">Header</span></span>       | <span data-ttu-id="ee26b-120">値</span><span class="sxs-lookup"><span data-stu-id="ee26b-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ee26b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ee26b-121">Authorization</span></span>  | <span data-ttu-id="ee26b-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ee26b-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ee26b-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ee26b-124">Content-Type</span></span>  | <span data-ttu-id="ee26b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ee26b-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ee26b-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="ee26b-126">Request body</span></span>

<span data-ttu-id="ee26b-127">要求の本体で、[チーム](../resources/team.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="ee26b-127">In the request body, supply a JSON representation of a [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ee26b-128">応答</span><span class="sxs-lookup"><span data-stu-id="ee26b-128">Response</span></span>

<span data-ttu-id="ee26b-129">成功すると、このメソッドを返します、`201 Created`応答コードおよび応答の本文の[チーム](../resources/team.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="ee26b-129">If successful, this method should return a `201 Created` response code and a [team](../resources/team.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee26b-130">例</span><span class="sxs-lookup"><span data-stu-id="ee26b-130">Example</span></span>

#### <a name="request"></a><span data-ttu-id="ee26b-131">要求</span><span class="sxs-lookup"><span data-stu-id="ee26b-131">Request</span></span>

<span data-ttu-id="ee26b-132">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ee26b-132">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="ee26b-133">応答</span><span class="sxs-lookup"><span data-stu-id="ee26b-133">Response</span></span>

<span data-ttu-id="ee26b-134">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ee26b-134">The following is an example of the response.</span></span> 

><span data-ttu-id="ee26b-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="ee26b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="ee26b-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="ee26b-137">See also</span></span>

- [<span data-ttu-id="ee26b-138">チームのグループを作成</span><span class="sxs-lookup"><span data-stu-id="ee26b-138">Creating a group with a team</span></span>](../../../concepts/teams-create-group-and-team.md)
