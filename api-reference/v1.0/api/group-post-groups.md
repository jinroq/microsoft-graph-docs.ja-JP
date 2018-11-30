---
title: グループを作成する
description: この API を使用して、要求本文で指定した新しいグループを作成します。次に示す 3 種類のグループのうちの 1 つを作成できます。
ms.openlocfilehash: 63cb04ad1b7bd8bfbe0798b53f28b5b16e0b795f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021375"
---
# <a name="create-group"></a><span data-ttu-id="95e48-104">グループを作成する</span><span class="sxs-lookup"><span data-stu-id="95e48-104">Create group</span></span>
<span data-ttu-id="95e48-p102">この API を使用して、要求本文で指定した新しいグループを作成します。次に示す 3 種類のグループのうちの 1 つを作成できます。</span><span class="sxs-lookup"><span data-stu-id="95e48-p102">Use this API to create a new group as specified in the request body. You can create one of three types of groups:</span></span>

* <span data-ttu-id="95e48-107">Office 365 グループ (統合グループ)</span><span class="sxs-lookup"><span data-stu-id="95e48-107">Office 365 Group (unified group)</span></span>
* <span data-ttu-id="95e48-108">動的グループ</span><span class="sxs-lookup"><span data-stu-id="95e48-108">Dynamic group</span></span>
* <span data-ttu-id="95e48-109">セキュリティ グループ</span><span class="sxs-lookup"><span data-stu-id="95e48-109">Security group</span></span>

> <span data-ttu-id="95e48-p103">**注**:Microsoft Teams は Office 365 グループに基づいていますが、現在、この API を使用してチームを作成することはできません。Microsoft Teams UI で作成されたチームを管理するには、その他のグループ API を使用できます。</span><span class="sxs-lookup"><span data-stu-id="95e48-p103">**Note**: Although Microsoft Teams is built on Office 365 Groups, you can't currently create a team via this API. You can use the other group APIs to manage a team that has been created in the Microsoft Teams UI.</span></span>

## <a name="permissions"></a><span data-ttu-id="95e48-112">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="95e48-112">Permissions</span></span>
<span data-ttu-id="95e48-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="95e48-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95e48-115">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="95e48-115">Permission type</span></span>      | <span data-ttu-id="95e48-116">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="95e48-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="95e48-117">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="95e48-117">Delegated (work or school account)</span></span> | <span data-ttu-id="95e48-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95e48-118">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="95e48-119">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="95e48-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="95e48-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="95e48-120">Not supported.</span></span>    |
|<span data-ttu-id="95e48-121">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="95e48-121">Application</span></span> | <span data-ttu-id="95e48-122">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95e48-122">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="95e48-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="95e48-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="95e48-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="95e48-124">Request headers</span></span>
| <span data-ttu-id="95e48-125">名前</span><span class="sxs-lookup"><span data-stu-id="95e48-125">Name</span></span>       | <span data-ttu-id="95e48-126">型</span><span class="sxs-lookup"><span data-stu-id="95e48-126">Type</span></span> | <span data-ttu-id="95e48-127">説明</span><span class="sxs-lookup"><span data-stu-id="95e48-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="95e48-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="95e48-128">Authorization</span></span>  | <span data-ttu-id="95e48-129">string</span><span class="sxs-lookup"><span data-stu-id="95e48-129">string</span></span>  | <span data-ttu-id="95e48-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="95e48-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="95e48-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="95e48-132">Request body</span></span>
<span data-ttu-id="95e48-133">グループを作成するときに指定する[グループ](../resources/group.md)・ リソースのプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="95e48-133">The following table shows the properties of the [group](../resources/group.md) resource to specify when you create a group.</span></span> 

| <span data-ttu-id="95e48-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="95e48-134">Property</span></span> | <span data-ttu-id="95e48-135">型</span><span class="sxs-lookup"><span data-stu-id="95e48-135">Type</span></span> | <span data-ttu-id="95e48-136">説明</span><span class="sxs-lookup"><span data-stu-id="95e48-136">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="95e48-137">displayName</span><span class="sxs-lookup"><span data-stu-id="95e48-137">displayName</span></span> | <span data-ttu-id="95e48-138">string</span><span class="sxs-lookup"><span data-stu-id="95e48-138">string</span></span> | <span data-ttu-id="95e48-139">アドレス帳に表示するグループの名前。</span><span class="sxs-lookup"><span data-stu-id="95e48-139">The name to display in the address book for the group.</span></span> <span data-ttu-id="95e48-140">必須。</span><span class="sxs-lookup"><span data-stu-id="95e48-140">Required.</span></span> |
| <span data-ttu-id="95e48-141">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="95e48-141">mailEnabled</span></span> | <span data-ttu-id="95e48-142">ブール値</span><span class="sxs-lookup"><span data-stu-id="95e48-142">boolean</span></span> | <span data-ttu-id="95e48-143">メールが有効なグループの場合は、**true** に設定します。</span><span class="sxs-lookup"><span data-stu-id="95e48-143">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="95e48-144">Office 365 グループを作成する場合**は true**に設定します。</span><span class="sxs-lookup"><span data-stu-id="95e48-144">Set this to **true** if creating an Office 365 Group.</span></span> <span data-ttu-id="95e48-145">**False**場合は、動的に作成するグループまたはセキュリティ グループを設定します。</span><span class="sxs-lookup"><span data-stu-id="95e48-145">Set this to **false** if creating dynamic or security group.</span></span> <span data-ttu-id="95e48-146">必須。</span><span class="sxs-lookup"><span data-stu-id="95e48-146">Required.</span></span> |
| <span data-ttu-id="95e48-147">mailNickname</span><span class="sxs-lookup"><span data-stu-id="95e48-147">mailNickname</span></span> | <span data-ttu-id="95e48-148">文字列</span><span class="sxs-lookup"><span data-stu-id="95e48-148">string</span></span> | <span data-ttu-id="95e48-149">グループの電子メール エイリアス。</span><span class="sxs-lookup"><span data-stu-id="95e48-149">The mail alias for the group.</span></span> <span data-ttu-id="95e48-150">必須。</span><span class="sxs-lookup"><span data-stu-id="95e48-150">Required.</span></span> |
| <span data-ttu-id="95e48-151">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="95e48-151">securityEnabled</span></span> | <span data-ttu-id="95e48-152">ブール値</span><span class="sxs-lookup"><span data-stu-id="95e48-152">boolean</span></span> | <span data-ttu-id="95e48-153">**真**のセキュリティが有効なグループを設定します。</span><span class="sxs-lookup"><span data-stu-id="95e48-153">Set to **true** for security-enabled groups.</span></span> <span data-ttu-id="95e48-154">動的またはセキュリティ グループを作成する場合**は true**に設定します。</span><span class="sxs-lookup"><span data-stu-id="95e48-154">Set this to **true** if creating a dynamic or security group.</span></span> <span data-ttu-id="95e48-155">Office 365 グループを作成する場合**は false**に設定します。</span><span class="sxs-lookup"><span data-stu-id="95e48-155">Set this to **false** if creating an Office 365 group.</span></span> <span data-ttu-id="95e48-156">必須。</span><span class="sxs-lookup"><span data-stu-id="95e48-156">Required.</span></span> |
| <span data-ttu-id="95e48-157">owners</span><span class="sxs-lookup"><span data-stu-id="95e48-157">owners</span></span> | <span data-ttu-id="95e48-158">string collection</span><span class="sxs-lookup"><span data-stu-id="95e48-158">string collection</span></span> | <span data-ttu-id="95e48-159">このプロパティは、作成時に、グループの所有者を表します。</span><span class="sxs-lookup"><span data-stu-id="95e48-159">This property represents the owners for the group at creation time.</span></span> <span data-ttu-id="95e48-160">省略可能。</span><span class="sxs-lookup"><span data-stu-id="95e48-160">Optional.</span></span> |
| <span data-ttu-id="95e48-161">メンバー</span><span class="sxs-lookup"><span data-stu-id="95e48-161">members</span></span> | <span data-ttu-id="95e48-162">string collection</span><span class="sxs-lookup"><span data-stu-id="95e48-162">string collection</span></span> | <span data-ttu-id="95e48-163">このプロパティは、作成時にグループのメンバーを表します。</span><span class="sxs-lookup"><span data-stu-id="95e48-163">This property represents the members for the group at creation time.</span></span> <span data-ttu-id="95e48-164">省略可能。</span><span class="sxs-lookup"><span data-stu-id="95e48-164">Optional.</span></span> |


<span data-ttu-id="95e48-165">Office 365 グループまたは動的グループを作成している場合は、以下のように **groupTypes** プロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="95e48-165">Specify the **groupTypes** property if you're creating an Office 365 or dynamic group, as stated below.</span></span>

### <a name="grouptypes-options"></a><span data-ttu-id="95e48-166">groupTypes オプション</span><span class="sxs-lookup"><span data-stu-id="95e48-166">groupTypes options</span></span>

| <span data-ttu-id="95e48-167">グループの種類</span><span class="sxs-lookup"><span data-stu-id="95e48-167">Type of group</span></span> | <span data-ttu-id="95e48-168">**groupTypes** プロパティ</span><span class="sxs-lookup"><span data-stu-id="95e48-168">**groupTypes** property</span></span> |
|:--------------|:------------------------|
| <span data-ttu-id="95e48-169">Office 365 (統合グループともいいます)</span><span class="sxs-lookup"><span data-stu-id="95e48-169">Office 365 (aka unified group)</span></span>| <span data-ttu-id="95e48-170">"Unified"</span><span class="sxs-lookup"><span data-stu-id="95e48-170">"Unified"</span></span> |
| <span data-ttu-id="95e48-171">Dynamic</span><span class="sxs-lookup"><span data-stu-id="95e48-171">Dynamic</span></span> | <span data-ttu-id="95e48-172">"DynamicMembership"</span><span class="sxs-lookup"><span data-stu-id="95e48-172">"DynamicMembership"</span></span> |
| <span data-ttu-id="95e48-173">Security</span><span class="sxs-lookup"><span data-stu-id="95e48-173">Security</span></span> | <span data-ttu-id="95e48-174">設定しない。</span><span class="sxs-lookup"><span data-stu-id="95e48-174">Do not set.</span></span> |


><span data-ttu-id="95e48-175">**注:** ユーザー コンテキストおよび所有者を指定することがなくプログラムでは、Office 365 のグループを作成するグループを作成し、匿名で。</span><span class="sxs-lookup"><span data-stu-id="95e48-175">**Note:** Creating an Office 365 Group programmatically without a user context and  without specifying owners will create the group anonymously.</span></span>  <span data-ttu-id="95e48-176">これを行うと、関連付けられた SharePoint Online サイトで作成されていない自動的にさらに手動で操作が実行されるまでがあります。</span><span class="sxs-lookup"><span data-stu-id="95e48-176">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  

<span data-ttu-id="95e48-p113">グループの必要に応じて他の書き込み可能なプロパティを指定します。詳細については、[group](../resources/group.md) リソースのプロパティをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="95e48-p113">Specify other writable properties as necessary for your group. For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

## <a name="response"></a><span data-ttu-id="95e48-179">応答</span><span class="sxs-lookup"><span data-stu-id="95e48-179">Response</span></span>
<span data-ttu-id="95e48-180">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で[グループ](../resources/group.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="95e48-180">If successful, this method returns `201 Created` response code and [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95e48-181">例</span><span class="sxs-lookup"><span data-stu-id="95e48-181">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="95e48-182">要求 1</span><span class="sxs-lookup"><span data-stu-id="95e48-182">Request 1</span></span>
<span data-ttu-id="95e48-183">例の最初の要求では、Office 365 グループを作成します。</span><span class="sxs-lookup"><span data-stu-id="95e48-183">The first example request creates an Office 365 Group.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups
Content-type: application/json
Content-length: 244

{
  "description": "Self help community for library",
  "displayName": "Library Assist",
  "groupTypes": [
    "Unified"
  ],
  "mailEnabled": true,
  "mailNickname": "library",
  "securityEnabled": false
}
```

#### <a name="response-1"></a><span data-ttu-id="95e48-184">応答 1</span><span class="sxs-lookup"><span data-stu-id="95e48-184">Response 1</span></span>
<span data-ttu-id="95e48-185">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="95e48-185">The following is an example of the response.</span></span>
><span data-ttu-id="95e48-186">**注:** ここに示す応答オブジェクトは、読みやすさの短縮される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="95e48-186">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="95e48-187">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="95e48-187">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 244

{
  "description": "Self help community for library",
  "displayName": "Library Assist",
  "groupTypes": [
    "Unified"
  ],
  "mail": "library@contoso.onmicrosoft.com",
  "mailEnabled": true,
  "mailNickname": "library",
  "securityEnabled": false
}
```

#### <a name="request-2"></a><span data-ttu-id="95e48-188">要求 2</span><span class="sxs-lookup"><span data-stu-id="95e48-188">Request 2</span></span>
<span data-ttu-id="95e48-189">2 番目の例の要求では、所有者が指定されている、Office 365 のグループを作成します。</span><span class="sxs-lookup"><span data-stu-id="95e48-189">The second example request creates an Office 365 Group with owners specified.</span></span>
<!-- {
  "blockType": "request"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups
Content-Type: application/json

{
  "description": "Group with owners",
  "displayName": "Group1",
  "groupTypes": [
    "Unified"
  ],
  "mailEnabled": true,
  "mailNickname": "group1",
  "securityEnabled": false,
  "owners@odata.bind": [
    "https://graph.microsoft.com/v1.0/users/26be1845-4119-4801-a799-aea79d09f1a2"
  ]
}
```

#### <a name="response-2"></a><span data-ttu-id="95e48-190">応答 2</span><span class="sxs-lookup"><span data-stu-id="95e48-190">Response 2</span></span>
<span data-ttu-id="95e48-191">次は、正常な応答の例です。</span><span class="sxs-lookup"><span data-stu-id="95e48-191">The following is an example of the successful response.</span></span>
><span data-ttu-id="95e48-192">**注:** ここに示す応答オブジェクトは、読みやすさの短縮される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="95e48-192">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="95e48-193">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="95e48-193">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "description": "Group with owners",
    "displayName": "Group1",
    "groupTypes": [
        "Unified"
    ],
    "mail": "group1@contoso.onmicrosoft.com",
    "mailEnabled": true,
    "mailNickname": "group1",
    "securityEnabled": false
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
