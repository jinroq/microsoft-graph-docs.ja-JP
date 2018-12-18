---
title: グループを作成する
description: この API を使用して、要求本文で指定した新しいグループを作成します。次に示す 3 種類のグループのうちの 1 つを作成できます。
author: dkershaw10
ms.openlocfilehash: 1c77b3a33b19e9f0254642ef89e3d7fddc224b9a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320770"
---
# <a name="create-group"></a><span data-ttu-id="f8442-104">グループを作成する</span><span class="sxs-lookup"><span data-stu-id="f8442-104">Create group</span></span>

> <span data-ttu-id="f8442-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f8442-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f8442-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f8442-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f8442-107">要求の本体に指定されている新しい[グループ](../resources/group.md)を作成するのにには、この API を使用します。</span><span class="sxs-lookup"><span data-stu-id="f8442-107">Use this API to create a new [group](../resources/group.md) as specified in the request body.</span></span> <span data-ttu-id="f8442-108">3 つの種類のグループのいずれかを作成できます。</span><span class="sxs-lookup"><span data-stu-id="f8442-108">You can create one of three types of groups:</span></span>

* <span data-ttu-id="f8442-109">Office 365 グループ (統合グループ)</span><span class="sxs-lookup"><span data-stu-id="f8442-109">Office 365 Group (unified group)</span></span>
* <span data-ttu-id="f8442-110">動的グループ</span><span class="sxs-lookup"><span data-stu-id="f8442-110">Dynamic group</span></span>
* <span data-ttu-id="f8442-111">セキュリティ グループ</span><span class="sxs-lookup"><span data-stu-id="f8442-111">Security group</span></span>

> <span data-ttu-id="f8442-112">**注**:[チーム](../resources/team.md)を作成して、最初にグループを作成し、チームを追加するのには、[チームの作成](../api/team-put-teams.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f8442-112">**Note**: To create a [team](../resources/team.md), first create a group then add a team to it, see [create team](../api/team-put-teams.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f8442-113">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f8442-113">Permissions</span></span>
<span data-ttu-id="f8442-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f8442-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8442-116">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f8442-116">Permission type</span></span>      | <span data-ttu-id="f8442-117">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f8442-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f8442-118">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f8442-118">Delegated (work or school account)</span></span> | <span data-ttu-id="f8442-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8442-119">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f8442-120">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f8442-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8442-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f8442-121">Not supported.</span></span>    |
|<span data-ttu-id="f8442-122">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f8442-122">Application</span></span> | <span data-ttu-id="f8442-123">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8442-123">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f8442-124">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f8442-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="f8442-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f8442-125">Request headers</span></span>
| <span data-ttu-id="f8442-126">名前</span><span class="sxs-lookup"><span data-stu-id="f8442-126">Name</span></span>       | <span data-ttu-id="f8442-127">種類</span><span class="sxs-lookup"><span data-stu-id="f8442-127">Type</span></span> | <span data-ttu-id="f8442-128">説明</span><span class="sxs-lookup"><span data-stu-id="f8442-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f8442-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8442-129">Authorization</span></span>  | <span data-ttu-id="f8442-130">string</span><span class="sxs-lookup"><span data-stu-id="f8442-130">string</span></span>  | <span data-ttu-id="f8442-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f8442-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f8442-133">要求本文</span><span class="sxs-lookup"><span data-stu-id="f8442-133">Request body</span></span>
<span data-ttu-id="f8442-134">グループを作成するときに指定する[グループ](../resources/group.md)・ リソースのプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="f8442-134">The following table shows the properties of the [group](../resources/group.md) resource to specify when you create a group.</span></span> 

| <span data-ttu-id="f8442-135">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f8442-135">Property</span></span> | <span data-ttu-id="f8442-136">種類</span><span class="sxs-lookup"><span data-stu-id="f8442-136">Type</span></span> | <span data-ttu-id="f8442-137">説明</span><span class="sxs-lookup"><span data-stu-id="f8442-137">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f8442-138">displayName</span><span class="sxs-lookup"><span data-stu-id="f8442-138">displayName</span></span> | <span data-ttu-id="f8442-139">string</span><span class="sxs-lookup"><span data-stu-id="f8442-139">string</span></span> | <span data-ttu-id="f8442-140">アドレス帳に表示するグループの名前。</span><span class="sxs-lookup"><span data-stu-id="f8442-140">The name to display in the address book for the group.</span></span> <span data-ttu-id="f8442-141">必須です。</span><span class="sxs-lookup"><span data-stu-id="f8442-141">Required.</span></span> |
| <span data-ttu-id="f8442-142">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="f8442-142">mailEnabled</span></span> | <span data-ttu-id="f8442-143">ブール値</span><span class="sxs-lookup"><span data-stu-id="f8442-143">boolean</span></span> | <span data-ttu-id="f8442-144">メールが有効なグループの場合は、**true** に設定します。</span><span class="sxs-lookup"><span data-stu-id="f8442-144">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="f8442-145">Office 365 グループを作成する場合**は true**に設定します。</span><span class="sxs-lookup"><span data-stu-id="f8442-145">Set this to **true** if creating an Office 365 Group.</span></span> <span data-ttu-id="f8442-146">**False**場合は、動的に作成するグループまたはセキュリティ グループを設定します。</span><span class="sxs-lookup"><span data-stu-id="f8442-146">Set this to **false** if creating dynamic or security group.</span></span> <span data-ttu-id="f8442-147">必須です。</span><span class="sxs-lookup"><span data-stu-id="f8442-147">Required.</span></span> |
| <span data-ttu-id="f8442-148">mailNickname</span><span class="sxs-lookup"><span data-stu-id="f8442-148">mailNickname</span></span> | <span data-ttu-id="f8442-149">string</span><span class="sxs-lookup"><span data-stu-id="f8442-149">string</span></span> | <span data-ttu-id="f8442-150">グループの電子メール エイリアス。</span><span class="sxs-lookup"><span data-stu-id="f8442-150">The mail alias for the group.</span></span> <span data-ttu-id="f8442-151">必須です。</span><span class="sxs-lookup"><span data-stu-id="f8442-151">Required.</span></span> |
| <span data-ttu-id="f8442-152">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="f8442-152">securityEnabled</span></span> | <span data-ttu-id="f8442-153">ブール値</span><span class="sxs-lookup"><span data-stu-id="f8442-153">boolean</span></span> | <span data-ttu-id="f8442-154">**真**のセキュリティが有効なグループを設定します。</span><span class="sxs-lookup"><span data-stu-id="f8442-154">Set to **true** for security-enabled groups.</span></span> <span data-ttu-id="f8442-155">動的またはセキュリティ グループを作成する場合**は true**に設定します。</span><span class="sxs-lookup"><span data-stu-id="f8442-155">Set this to **true** if creating a dynamic or security group.</span></span> <span data-ttu-id="f8442-156">Office 365 グループを作成する場合**は false**に設定します。</span><span class="sxs-lookup"><span data-stu-id="f8442-156">Set this to **false** if creating an Office 365 Group.</span></span> <span data-ttu-id="f8442-157">必須です。</span><span class="sxs-lookup"><span data-stu-id="f8442-157">Required.</span></span> |
| <span data-ttu-id="f8442-158">owners</span><span class="sxs-lookup"><span data-stu-id="f8442-158">owners</span></span> | <span data-ttu-id="f8442-159">string collection</span><span class="sxs-lookup"><span data-stu-id="f8442-159">string collection</span></span> | <span data-ttu-id="f8442-160">このプロパティは、作成時に、グループの所有者を表します。</span><span class="sxs-lookup"><span data-stu-id="f8442-160">This property represents the owners for the group at creation time.</span></span> <span data-ttu-id="f8442-161">省略可能。</span><span class="sxs-lookup"><span data-stu-id="f8442-161">Optional.</span></span> |
| <span data-ttu-id="f8442-162">メンバー</span><span class="sxs-lookup"><span data-stu-id="f8442-162">members</span></span> | <span data-ttu-id="f8442-163">string collection</span><span class="sxs-lookup"><span data-stu-id="f8442-163">string collection</span></span> | <span data-ttu-id="f8442-164">このプロパティは、作成時にグループのメンバーを表します。</span><span class="sxs-lookup"><span data-stu-id="f8442-164">This property represents the members for the group at creation time.</span></span> <span data-ttu-id="f8442-165">省略可能。</span><span class="sxs-lookup"><span data-stu-id="f8442-165">Optional.</span></span> |

<span data-ttu-id="f8442-166">Office 365 グループまたは動的グループを作成している場合は、以下のように **groupTypes** プロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="f8442-166">Specify the **groupTypes** property if you're creating an Office 365 or dynamic group, as stated below.</span></span>

| <span data-ttu-id="f8442-167">グループの種類</span><span class="sxs-lookup"><span data-stu-id="f8442-167">Type of group</span></span> | <span data-ttu-id="f8442-168">**groupTypes** プロパティ</span><span class="sxs-lookup"><span data-stu-id="f8442-168">**groupTypes** property</span></span> |
|:--------------|:------------------------|
| <span data-ttu-id="f8442-169">Office 365 (統合グループともいいます)</span><span class="sxs-lookup"><span data-stu-id="f8442-169">Office 365 (aka unified group)</span></span>| <span data-ttu-id="f8442-170">"Unified"</span><span class="sxs-lookup"><span data-stu-id="f8442-170">"Unified"</span></span> |
| <span data-ttu-id="f8442-171">Dynamic</span><span class="sxs-lookup"><span data-stu-id="f8442-171">Dynamic</span></span> | <span data-ttu-id="f8442-172">"DynamicMembership"</span><span class="sxs-lookup"><span data-stu-id="f8442-172">"DynamicMembership"</span></span> |
| <span data-ttu-id="f8442-173">Security</span><span class="sxs-lookup"><span data-stu-id="f8442-173">Security</span></span> | <span data-ttu-id="f8442-174">設定しない。</span><span class="sxs-lookup"><span data-stu-id="f8442-174">Do not set.</span></span> |

<span data-ttu-id="f8442-175">**グループ**・ リソースは、[拡張機能](/graph/extensibility-overview)をサポートするため使用すること、`POST`操作し、作成時に実際のデータにカスタム プロパティをグループに追加します。</span><span class="sxs-lookup"><span data-stu-id="f8442-175">Since the **group** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the group while creating it.</span></span>

><span data-ttu-id="f8442-176">**注:** ユーザー コンテキストおよび所有者を指定することがなくプログラムでは、Office 365 のグループを作成すると、匿名で、グループが作成されます。</span><span class="sxs-lookup"><span data-stu-id="f8442-176">**Note:** Creating an Office 365 Group programmatically without a user context and  without specifying owners will create the group anonymously.</span></span>  <span data-ttu-id="f8442-177">これを行うと、関連付けられた SharePoint Online サイトで作成されていない自動的にさらに手動で操作が実行されるまでがあります。</span><span class="sxs-lookup"><span data-stu-id="f8442-177">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  

<span data-ttu-id="f8442-p113">グループの必要に応じて他の書き込み可能なプロパティを指定します。詳細については、[group](../resources/group.md) リソースのプロパティをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="f8442-p113">Specify other writable properties as necessary for your group. For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

## <a name="response"></a><span data-ttu-id="f8442-180">応答</span><span class="sxs-lookup"><span data-stu-id="f8442-180">Response</span></span>
<span data-ttu-id="f8442-181">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で[グループ](../resources/group.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f8442-181">If successful, this method returns `201 Created` response code and [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8442-182">例</span><span class="sxs-lookup"><span data-stu-id="f8442-182">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="f8442-183">要求 1</span><span class="sxs-lookup"><span data-stu-id="f8442-183">Request 1</span></span>
<span data-ttu-id="f8442-184">例の最初の要求では、Office 365 グループを作成します。</span><span class="sxs-lookup"><span data-stu-id="f8442-184">The first example request creates an Office 365 Group.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_group"
}-->
```http
POST https://graph.microsoft.com/beta/groups
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

#### <a name="response"></a><span data-ttu-id="f8442-185">応答</span><span class="sxs-lookup"><span data-stu-id="f8442-185">Response</span></span>
<span data-ttu-id="f8442-186">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f8442-186">The following is an example of the response.</span></span>
><span data-ttu-id="f8442-187">**注:** ここに示す応答オブジェクトは、読みやすさの短縮される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="f8442-187">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f8442-188">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="f8442-188">All the properties will be returned from an actual call.</span></span>
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

#### <a name="request-2"></a><span data-ttu-id="f8442-189">要求 2</span><span class="sxs-lookup"><span data-stu-id="f8442-189">Request 2</span></span>
<span data-ttu-id="f8442-190">2 番目の例の要求では、所有者が指定されている、Office 365 のグループを作成します。</span><span class="sxs-lookup"><span data-stu-id="f8442-190">The second example request creates an Office 365 Group with owners specified.</span></span>
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

 #### <a name="response-2"></a><span data-ttu-id="f8442-191">応答 2</span><span class="sxs-lookup"><span data-stu-id="f8442-191">Response 2</span></span>
<span data-ttu-id="f8442-192">次は、正常な応答の例です。</span><span class="sxs-lookup"><span data-stu-id="f8442-192">The following is an example of the successful response.</span></span>
><span data-ttu-id="f8442-p115">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="f8442-p115">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="f8442-195">関連項目</span><span class="sxs-lookup"><span data-stu-id="f8442-195">See also</span></span>

- [<span data-ttu-id="f8442-196">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="f8442-196">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="f8442-197">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="f8442-197">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="f8442-198">スキーマ拡張機能を使用したグループへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="f8442-198">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
