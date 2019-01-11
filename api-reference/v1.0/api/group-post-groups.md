---
title: グループを作成する
description: この API を使用して、要求本文で指定した新しいグループを作成します。次に示す 3 種類のグループのうちの 1 つを作成できます。
author: dkershaw10
localization_priority: Priority
ms.openlocfilehash: 3f6a73b6fd2dcf76bb1ebd0fab4c02a673a1be8e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849421"
---
# <a name="create-group"></a><span data-ttu-id="2372e-104">グループを作成する</span><span class="sxs-lookup"><span data-stu-id="2372e-104">Create group</span></span>
<span data-ttu-id="2372e-p102">この API を使用して、要求本文で指定した新しいグループを作成します。次に示す 3 種類のグループのうちの 1 つを作成できます。</span><span class="sxs-lookup"><span data-stu-id="2372e-p102">Use this API to create a new group as specified in the request body. You can create one of three types of groups:</span></span>

* <span data-ttu-id="2372e-107">Office 365 グループ (統合グループ)</span><span class="sxs-lookup"><span data-stu-id="2372e-107">Office 365 Group (unified group)</span></span>
* <span data-ttu-id="2372e-108">動的グループ</span><span class="sxs-lookup"><span data-stu-id="2372e-108">Dynamic group</span></span>
* <span data-ttu-id="2372e-109">セキュリティ グループ</span><span class="sxs-lookup"><span data-stu-id="2372e-109">Security group</span></span>

> <span data-ttu-id="2372e-p103">**注**:Microsoft Teams は Office 365 グループに基づいていますが、現在、この API を使用してチームを作成することはできません。Microsoft Teams UI で作成されたチームを管理するには、その他のグループ API を使用できます。</span><span class="sxs-lookup"><span data-stu-id="2372e-p103">**Note**: Although Microsoft Teams is built on Office 365 Groups, you can't currently create a team via this API. You can use the other group APIs to manage a team that has been created in the Microsoft Teams UI.</span></span>

## <a name="permissions"></a><span data-ttu-id="2372e-112">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2372e-112">Permissions</span></span>
<span data-ttu-id="2372e-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2372e-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2372e-115">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2372e-115">Permission type</span></span>      | <span data-ttu-id="2372e-116">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2372e-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2372e-117">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2372e-117">Delegated (work or school account)</span></span> | <span data-ttu-id="2372e-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2372e-118">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="2372e-119">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2372e-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2372e-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2372e-120">Not supported.</span></span>    |
|<span data-ttu-id="2372e-121">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2372e-121">Application</span></span> | <span data-ttu-id="2372e-122">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2372e-122">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2372e-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2372e-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="2372e-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2372e-124">Request headers</span></span>
| <span data-ttu-id="2372e-125">名前</span><span class="sxs-lookup"><span data-stu-id="2372e-125">Name</span></span>       | <span data-ttu-id="2372e-126">種類</span><span class="sxs-lookup"><span data-stu-id="2372e-126">Type</span></span> | <span data-ttu-id="2372e-127">説明</span><span class="sxs-lookup"><span data-stu-id="2372e-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2372e-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="2372e-128">Authorization</span></span>  | <span data-ttu-id="2372e-129">string</span><span class="sxs-lookup"><span data-stu-id="2372e-129">string</span></span>  | <span data-ttu-id="2372e-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2372e-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2372e-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="2372e-132">Request body</span></span>
<span data-ttu-id="2372e-133">グループを作成するときに指定する[グループ](../resources/group.md)・ リソースのプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="2372e-133">The following table shows the properties of the [group](../resources/group.md) resource to specify when you create a group.</span></span> 

| <span data-ttu-id="2372e-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2372e-134">Property</span></span> | <span data-ttu-id="2372e-135">種類</span><span class="sxs-lookup"><span data-stu-id="2372e-135">Type</span></span> | <span data-ttu-id="2372e-136">説明</span><span class="sxs-lookup"><span data-stu-id="2372e-136">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2372e-137">displayName</span><span class="sxs-lookup"><span data-stu-id="2372e-137">displayName</span></span> | <span data-ttu-id="2372e-138">string</span><span class="sxs-lookup"><span data-stu-id="2372e-138">string</span></span> | <span data-ttu-id="2372e-139">アドレス帳に表示するグループの名前。</span><span class="sxs-lookup"><span data-stu-id="2372e-139">The name to display in the address book for the group.</span></span> <span data-ttu-id="2372e-140">必須。</span><span class="sxs-lookup"><span data-stu-id="2372e-140">Required.</span></span> |
| <span data-ttu-id="2372e-141">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="2372e-141">mailEnabled</span></span> | <span data-ttu-id="2372e-142">ブール値</span><span class="sxs-lookup"><span data-stu-id="2372e-142">boolean</span></span> | <span data-ttu-id="2372e-143">メールが有効なグループの場合は、**true** に設定します。</span><span class="sxs-lookup"><span data-stu-id="2372e-143">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="2372e-144">Office 365 グループを作成する場合**は true**に設定します。</span><span class="sxs-lookup"><span data-stu-id="2372e-144">Set this to **true** if creating an Office 365 Group.</span></span> <span data-ttu-id="2372e-145">**False**場合は、動的に作成するグループまたはセキュリティ グループを設定します。</span><span class="sxs-lookup"><span data-stu-id="2372e-145">Set this to **false** if creating dynamic or security group.</span></span> <span data-ttu-id="2372e-146">必須。</span><span class="sxs-lookup"><span data-stu-id="2372e-146">Required.</span></span> |
| <span data-ttu-id="2372e-147">mailNickname</span><span class="sxs-lookup"><span data-stu-id="2372e-147">mailNickname</span></span> | <span data-ttu-id="2372e-148">文字列</span><span class="sxs-lookup"><span data-stu-id="2372e-148">string</span></span> | <span data-ttu-id="2372e-149">グループの電子メール エイリアス。</span><span class="sxs-lookup"><span data-stu-id="2372e-149">The mail alias for the group.</span></span> <span data-ttu-id="2372e-150">必須。</span><span class="sxs-lookup"><span data-stu-id="2372e-150">Required.</span></span> |
| <span data-ttu-id="2372e-151">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="2372e-151">securityEnabled</span></span> | <span data-ttu-id="2372e-152">ブール値</span><span class="sxs-lookup"><span data-stu-id="2372e-152">boolean</span></span> | <span data-ttu-id="2372e-153">**真**のセキュリティが有効なグループを設定します。</span><span class="sxs-lookup"><span data-stu-id="2372e-153">Set to **true** for security-enabled groups.</span></span> <span data-ttu-id="2372e-154">動的またはセキュリティ グループを作成する場合**は true**に設定します。</span><span class="sxs-lookup"><span data-stu-id="2372e-154">Set this to **true** if creating a dynamic or security group.</span></span> <span data-ttu-id="2372e-155">Office 365 グループを作成する場合**は false**に設定します。</span><span class="sxs-lookup"><span data-stu-id="2372e-155">Set this to **false** if creating an Office 365 group.</span></span> <span data-ttu-id="2372e-156">必須。</span><span class="sxs-lookup"><span data-stu-id="2372e-156">Required.</span></span> |
| <span data-ttu-id="2372e-157">owners</span><span class="sxs-lookup"><span data-stu-id="2372e-157">owners</span></span> | <span data-ttu-id="2372e-158">string collection</span><span class="sxs-lookup"><span data-stu-id="2372e-158">string collection</span></span> | <span data-ttu-id="2372e-159">このプロパティは、作成時に、グループの所有者を表します。</span><span class="sxs-lookup"><span data-stu-id="2372e-159">This property represents the owners for the group at creation time.</span></span> <span data-ttu-id="2372e-160">省略可能。</span><span class="sxs-lookup"><span data-stu-id="2372e-160">Optional.</span></span> |
| <span data-ttu-id="2372e-161">メンバー</span><span class="sxs-lookup"><span data-stu-id="2372e-161">members</span></span> | <span data-ttu-id="2372e-162">string collection</span><span class="sxs-lookup"><span data-stu-id="2372e-162">string collection</span></span> | <span data-ttu-id="2372e-163">このプロパティは、作成時にグループのメンバーを表します。</span><span class="sxs-lookup"><span data-stu-id="2372e-163">This property represents the members for the group at creation time.</span></span> <span data-ttu-id="2372e-164">省略可能。</span><span class="sxs-lookup"><span data-stu-id="2372e-164">Optional.</span></span> |


<span data-ttu-id="2372e-165">Office 365 グループまたは動的グループを作成している場合は、以下のように **groupTypes** プロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="2372e-165">Specify the **groupTypes** property if you're creating an Office 365 or dynamic group, as stated below.</span></span>

### <a name="grouptypes-options"></a><span data-ttu-id="2372e-166">groupTypes オプション</span><span class="sxs-lookup"><span data-stu-id="2372e-166">groupTypes options</span></span>

| <span data-ttu-id="2372e-167">グループの種類</span><span class="sxs-lookup"><span data-stu-id="2372e-167">Type of group</span></span> | <span data-ttu-id="2372e-168">**groupTypes** プロパティ</span><span class="sxs-lookup"><span data-stu-id="2372e-168">**groupTypes** property</span></span> |
|:--------------|:------------------------|
| <span data-ttu-id="2372e-169">Office 365 (統合グループともいいます)</span><span class="sxs-lookup"><span data-stu-id="2372e-169">Office 365 (aka unified group)</span></span>| <span data-ttu-id="2372e-170">"Unified"</span><span class="sxs-lookup"><span data-stu-id="2372e-170">"Unified"</span></span> |
| <span data-ttu-id="2372e-171">Dynamic</span><span class="sxs-lookup"><span data-stu-id="2372e-171">Dynamic</span></span> | <span data-ttu-id="2372e-172">"DynamicMembership"</span><span class="sxs-lookup"><span data-stu-id="2372e-172">"DynamicMembership"</span></span> |
| <span data-ttu-id="2372e-173">Security</span><span class="sxs-lookup"><span data-stu-id="2372e-173">Security</span></span> | <span data-ttu-id="2372e-174">設定しない。</span><span class="sxs-lookup"><span data-stu-id="2372e-174">Do not set.</span></span> |


><span data-ttu-id="2372e-175">**注:** ユーザー コンテキストおよび所有者を指定することがなくプログラムでは、Office 365 のグループを作成するグループを作成し、匿名で。</span><span class="sxs-lookup"><span data-stu-id="2372e-175">**Note:** Creating an Office 365 Group programmatically without a user context and  without specifying owners will create the group anonymously.</span></span>  <span data-ttu-id="2372e-176">これを行うと、関連付けられた SharePoint Online サイトで作成されていない自動的にさらに手動で操作が実行されるまでがあります。</span><span class="sxs-lookup"><span data-stu-id="2372e-176">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  

<span data-ttu-id="2372e-p113">グループの必要に応じて他の書き込み可能なプロパティを指定します。詳細については、[group](../resources/group.md) リソースのプロパティをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="2372e-p113">Specify other writable properties as necessary for your group. For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

## <a name="response"></a><span data-ttu-id="2372e-179">応答</span><span class="sxs-lookup"><span data-stu-id="2372e-179">Response</span></span>
<span data-ttu-id="2372e-180">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で[グループ](../resources/group.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2372e-180">If successful, this method returns `201 Created` response code and [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2372e-181">例</span><span class="sxs-lookup"><span data-stu-id="2372e-181">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="2372e-182">要求 1</span><span class="sxs-lookup"><span data-stu-id="2372e-182">Request 1</span></span>
<span data-ttu-id="2372e-183">例の最初の要求では、Office 365 グループを作成します。</span><span class="sxs-lookup"><span data-stu-id="2372e-183">The first example request creates an Office 365 Group.</span></span>
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

#### <a name="response-1"></a><span data-ttu-id="2372e-184">応答 1</span><span class="sxs-lookup"><span data-stu-id="2372e-184">Response 1</span></span>
<span data-ttu-id="2372e-185">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2372e-185">The following is an example of the response.</span></span>
><span data-ttu-id="2372e-186">**注:** ここに示す応答オブジェクトは、読みやすさの短縮される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="2372e-186">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="2372e-187">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="2372e-187">All the properties will be returned from an actual call.</span></span>
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

#### <a name="request-2"></a><span data-ttu-id="2372e-188">要求 2</span><span class="sxs-lookup"><span data-stu-id="2372e-188">Request 2</span></span>
<span data-ttu-id="2372e-189">2 番目の例の要求では、所有者が指定されている、Office 365 のグループを作成します。</span><span class="sxs-lookup"><span data-stu-id="2372e-189">The second example request creates an Office 365 Group with owners specified.</span></span>
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

#### <a name="response-2"></a><span data-ttu-id="2372e-190">応答 2</span><span class="sxs-lookup"><span data-stu-id="2372e-190">Response 2</span></span>
<span data-ttu-id="2372e-191">次は、正常な応答の例です。</span><span class="sxs-lookup"><span data-stu-id="2372e-191">The following is an example of the successful response.</span></span>
><span data-ttu-id="2372e-192">**注:** ここに示す応答オブジェクトは、読みやすさの短縮される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="2372e-192">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="2372e-193">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="2372e-193">All the properties will be returned from an actual call.</span></span>
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
