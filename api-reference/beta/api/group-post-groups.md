---
title: グループを作成する
description: この API を使用して、要求本文で指定した新しいグループを作成します。次に示す 3 種類のグループのうちの 1 つを作成できます。
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: 1ec6e4768e979f30cb0cb34de7555e08bf25b41f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33324248"
---
# <a name="create-group"></a><span data-ttu-id="4c7ea-104">グループを作成する</span><span class="sxs-lookup"><span data-stu-id="4c7ea-104">Create group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c7ea-p102">この API を使用して、要求本文で指定した新しい[グループ](../resources/group.md)を作成します。次に示す 3 種類のグループのうちの 1 つを作成できます。</span><span class="sxs-lookup"><span data-stu-id="4c7ea-p102">Use this API to create a new group as specified in the request body. You can create one of three types of groups:</span></span>

* <span data-ttu-id="4c7ea-107">Office 365 グループ (統合グループ)</span><span class="sxs-lookup"><span data-stu-id="4c7ea-107">Office 365 Group (unified group)</span></span>
* <span data-ttu-id="4c7ea-108">動的グループ</span><span class="sxs-lookup"><span data-stu-id="4c7ea-108">Dynamic group</span></span>
* <span data-ttu-id="4c7ea-109">セキュリティ グループ</span><span class="sxs-lookup"><span data-stu-id="4c7ea-109">Security group</span></span>

<span data-ttu-id="4c7ea-110">この操作は既定で各グループのプロパティのサブセットのみを返します。</span><span class="sxs-lookup"><span data-stu-id="4c7ea-110">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="4c7ea-111">これらの既定のプロパティは、「[プロパティ](../resources/group.md#properties)」セクションに記載されています。</span><span class="sxs-lookup"><span data-stu-id="4c7ea-111">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span>

<span data-ttu-id="4c7ea-112">既定で_返されない_プロパティを取得するには、GET 操作を実行し、`$select` OData クエリ オプションでプロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="4c7ea-112">To get properties that are _not_ returned by default, do a GET operation and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="4c7ea-113">[例](group-get.md#request-2)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4c7ea-113">See an [example](group-get.md#request-2).</span></span>

> <span data-ttu-id="4c7ea-114">**注:** [チーム](../resources/team.md)を作成するには、まずグループを作成し、それからそのグループにチームを追加します。[チームの作成](../api/team-put-teams.md)に関するページを参照してください。</span><span class="sxs-lookup"><span data-stu-id="4c7ea-114">**Note**: To create a [team](../resources/team.md), first create a group then add a team to it, see [create team](../api/team-put-teams.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4c7ea-115">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4c7ea-115">Permissions</span></span>
<span data-ttu-id="4c7ea-p105">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4c7ea-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c7ea-118">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4c7ea-118">Permission type</span></span>      | <span data-ttu-id="4c7ea-119">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4c7ea-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4c7ea-120">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4c7ea-120">Delegated (work or school account)</span></span> | <span data-ttu-id="4c7ea-121">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c7ea-121">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4c7ea-122">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4c7ea-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c7ea-123">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4c7ea-123">Not supported.</span></span>    |
|<span data-ttu-id="4c7ea-124">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4c7ea-124">Application</span></span> | <span data-ttu-id="4c7ea-125">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c7ea-125">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4c7ea-126">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4c7ea-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="4c7ea-127">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4c7ea-127">Request headers</span></span>
| <span data-ttu-id="4c7ea-128">名前</span><span class="sxs-lookup"><span data-stu-id="4c7ea-128">Name</span></span>       | <span data-ttu-id="4c7ea-129">型</span><span class="sxs-lookup"><span data-stu-id="4c7ea-129">Type</span></span> | <span data-ttu-id="4c7ea-130">説明</span><span class="sxs-lookup"><span data-stu-id="4c7ea-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4c7ea-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c7ea-131">Authorization</span></span>  | <span data-ttu-id="4c7ea-132">string</span><span class="sxs-lookup"><span data-stu-id="4c7ea-132">string</span></span>  | <span data-ttu-id="4c7ea-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4c7ea-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4c7ea-135">要求本文</span><span class="sxs-lookup"><span data-stu-id="4c7ea-135">Request body</span></span>
<span data-ttu-id="4c7ea-136">次の表は、グループを作成するときに指定する [group](../resources/group.md) リソースのプロパティを示しています。</span><span class="sxs-lookup"><span data-stu-id="4c7ea-136">The following table shows the properties of the [group](../resources/group.md) resource to specify when you create a group.</span></span> 

| <span data-ttu-id="4c7ea-137">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4c7ea-137">Property</span></span> | <span data-ttu-id="4c7ea-138">型</span><span class="sxs-lookup"><span data-stu-id="4c7ea-138">Type</span></span> | <span data-ttu-id="4c7ea-139">説明</span><span class="sxs-lookup"><span data-stu-id="4c7ea-139">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4c7ea-140">displayName</span><span class="sxs-lookup"><span data-stu-id="4c7ea-140">displayName</span></span> | <span data-ttu-id="4c7ea-141">string</span><span class="sxs-lookup"><span data-stu-id="4c7ea-141">string</span></span> | <span data-ttu-id="4c7ea-142">アドレス帳に表示するグループの名前。</span><span class="sxs-lookup"><span data-stu-id="4c7ea-142">The name to display in the address book for the group.</span></span> <span data-ttu-id="4c7ea-143">必須です。</span><span class="sxs-lookup"><span data-stu-id="4c7ea-143">Required.</span></span> |
| <span data-ttu-id="4c7ea-144">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="4c7ea-144">mailEnabled</span></span> | <span data-ttu-id="4c7ea-145">boolean</span><span class="sxs-lookup"><span data-stu-id="4c7ea-145">boolean</span></span> | <span data-ttu-id="4c7ea-146">メールが有効なグループの場合は、**true** に設定します。</span><span class="sxs-lookup"><span data-stu-id="4c7ea-146">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="4c7ea-147">Office 365 グループを作成する場合は、これを **true** に設定します。</span><span class="sxs-lookup"><span data-stu-id="4c7ea-147">Set this to **true** if creating an Office 365 Group.</span></span> <span data-ttu-id="4c7ea-148">動的グループまたはセキュリティ グループを作成する場合は、これを **false** に設定します。</span><span class="sxs-lookup"><span data-stu-id="4c7ea-148">Set this to **false** if creating dynamic or security group.</span></span> <span data-ttu-id="4c7ea-149">必須です。</span><span class="sxs-lookup"><span data-stu-id="4c7ea-149">Required.</span></span> |
| <span data-ttu-id="4c7ea-150">mailNickname</span><span class="sxs-lookup"><span data-stu-id="4c7ea-150">mailNickname</span></span> | <span data-ttu-id="4c7ea-151">string</span><span class="sxs-lookup"><span data-stu-id="4c7ea-151">string</span></span> | <span data-ttu-id="4c7ea-152">グループのメール エイリアス。</span><span class="sxs-lookup"><span data-stu-id="4c7ea-152">The mail alias for the group.</span></span> <span data-ttu-id="4c7ea-153">必須です。</span><span class="sxs-lookup"><span data-stu-id="4c7ea-153">Required.</span></span> |
| <span data-ttu-id="4c7ea-154">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="4c7ea-154">securityEnabled</span></span> | <span data-ttu-id="4c7ea-155">ブール値</span><span class="sxs-lookup"><span data-stu-id="4c7ea-155">boolean</span></span> | <span data-ttu-id="4c7ea-156">セキュリティが有効なグループの場合は、**true** に設定します。</span><span class="sxs-lookup"><span data-stu-id="4c7ea-156">Set to **true** for security-enabled groups.</span></span> <span data-ttu-id="4c7ea-157">動的グループまたはセキュリティ グループを作成する場合は、これを **true** に設定します。</span><span class="sxs-lookup"><span data-stu-id="4c7ea-157">Set this to **true** if creating a dynamic or security group.</span></span> <span data-ttu-id="4c7ea-158">Office 365 グループを作成する場合は、これを **false** に設定します。</span><span class="sxs-lookup"><span data-stu-id="4c7ea-158">Set this to **false** if creating an Office 365 Group.</span></span> <span data-ttu-id="4c7ea-159">必須です。</span><span class="sxs-lookup"><span data-stu-id="4c7ea-159">Required.</span></span> |
| <span data-ttu-id="4c7ea-160">owners</span><span class="sxs-lookup"><span data-stu-id="4c7ea-160">owners</span></span> | <span data-ttu-id="4c7ea-161">string collection</span><span class="sxs-lookup"><span data-stu-id="4c7ea-161">string collection</span></span> | <span data-ttu-id="4c7ea-162">このプロパティは、作成時のグループの所有者を表します。</span><span class="sxs-lookup"><span data-stu-id="4c7ea-162">This property represents the owners for the group at creation time.</span></span> <span data-ttu-id="4c7ea-163">省略可能。</span><span class="sxs-lookup"><span data-stu-id="4c7ea-163">Optional.</span></span> |
| <span data-ttu-id="4c7ea-164">members</span><span class="sxs-lookup"><span data-stu-id="4c7ea-164">members</span></span> | <span data-ttu-id="4c7ea-165">string collection</span><span class="sxs-lookup"><span data-stu-id="4c7ea-165">string collection</span></span> | <span data-ttu-id="4c7ea-166">このプロパティは、作成時のグループのメンバーを表します。</span><span class="sxs-lookup"><span data-stu-id="4c7ea-166">This property represents the members for the group at creation time.</span></span> <span data-ttu-id="4c7ea-167">省略可能。</span><span class="sxs-lookup"><span data-stu-id="4c7ea-167">Optional.</span></span> |

<span data-ttu-id="4c7ea-168">Office 365 グループまたは動的グループを作成している場合は、以下のように **groupTypes** プロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="4c7ea-168">Specify the **groupTypes** property if you're creating an Office 365 or dynamic group, as stated below.</span></span>

| <span data-ttu-id="4c7ea-169">グループの種類</span><span class="sxs-lookup"><span data-stu-id="4c7ea-169">Type of group</span></span> | <span data-ttu-id="4c7ea-170">**groupTypes** プロパティ</span><span class="sxs-lookup"><span data-stu-id="4c7ea-170">**groupTypes** property</span></span> |
|:--------------|:------------------------|
| <span data-ttu-id="4c7ea-171">Office 365 (統合グループともいいます)</span><span class="sxs-lookup"><span data-stu-id="4c7ea-171">Office 365 (aka unified group)</span></span>| <span data-ttu-id="4c7ea-172">"Unified"</span><span class="sxs-lookup"><span data-stu-id="4c7ea-172">"Unified"</span></span> |
| <span data-ttu-id="4c7ea-173">Dynamic</span><span class="sxs-lookup"><span data-stu-id="4c7ea-173">Dynamic</span></span> | <span data-ttu-id="4c7ea-174">"DynamicMembership"</span><span class="sxs-lookup"><span data-stu-id="4c7ea-174">"DynamicMembership"</span></span> |
| <span data-ttu-id="4c7ea-175">Security</span><span class="sxs-lookup"><span data-stu-id="4c7ea-175">Security</span></span> | <span data-ttu-id="4c7ea-176">設定しない。</span><span class="sxs-lookup"><span data-stu-id="4c7ea-176">Do not set.</span></span> |

<span data-ttu-id="4c7ea-177">**グループ** リソースは[拡張機能](/graph/extensibility-overview)をサポートしているため、`POST` 操作を使用して、リソースの作成時にカスタム プロパティを独自のデータとともにグループに追加することができます。</span><span class="sxs-lookup"><span data-stu-id="4c7ea-177">Since the **group** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the group while creating it.</span></span>

><span data-ttu-id="4c7ea-178">**注:** ユーザー コンテキストを使用せず、所有者を指定せずにプログラムで Office 365 グループを作成すると、そのグループは匿名で作成されます。</span><span class="sxs-lookup"><span data-stu-id="4c7ea-178">**Note:** Creating an Office 365 Group programmatically without a user context and  without specifying owners will create the group anonymously.</span></span>  <span data-ttu-id="4c7ea-179">この操作を行うと、さらに手動操作が行われるまで、関連付けられている SharePoint Online サイトが自動的に作成されない可能性があります。</span><span class="sxs-lookup"><span data-stu-id="4c7ea-179">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  

<span data-ttu-id="4c7ea-p114">グループの必要に応じて他の書き込み可能なプロパティを指定します。詳細については、[group](../resources/group.md) リソースのプロパティを参照してください。</span><span class="sxs-lookup"><span data-stu-id="4c7ea-p114">Specify other writable properties as necessary for your group. For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

## <a name="response"></a><span data-ttu-id="4c7ea-182">応答</span><span class="sxs-lookup"><span data-stu-id="4c7ea-182">Response</span></span>
<span data-ttu-id="4c7ea-183">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [group](../resources/group.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4c7ea-183">If successful, this method returns `201 Created` response code and [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="4c7ea-184">応答には、そのグループの既定のプロパティのみが含まれます。</span><span class="sxs-lookup"><span data-stu-id="4c7ea-184">The response includes only the default properties of the group.</span></span>

## <a name="example"></a><span data-ttu-id="4c7ea-185">例</span><span class="sxs-lookup"><span data-stu-id="4c7ea-185">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="4c7ea-186">要求 1</span><span class="sxs-lookup"><span data-stu-id="4c7ea-186">Request 1</span></span>
<span data-ttu-id="4c7ea-187">最初の要求例では、Office 365 グループを作成しています。</span><span class="sxs-lookup"><span data-stu-id="4c7ea-187">The first example request creates an Office 365 Group.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_group"
}-->
```http
POST https://graph.microsoft.com/beta/groups
Content-type: application/json
Content-length: 244

{
  "description": "Self help community for golf",
  "displayName": "Golf Assist",
  "groupTypes": [
    "Unified"
  ],
  "mailEnabled": true,
  "mailNickname": "golfassist",
  "securityEnabled": false
}
```

#### <a name="response"></a><span data-ttu-id="4c7ea-188">応答</span><span class="sxs-lookup"><span data-stu-id="4c7ea-188">Response</span></span>
<span data-ttu-id="4c7ea-189">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4c7ea-189">The following is an example of the response.</span></span>
><span data-ttu-id="4c7ea-190">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="4c7ea-190">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4c7ea-191">実際の呼び出しからは、すべての既定のプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="4c7ea-191">All the default properties are returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "create_group"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
     "id": "45b7d2e7-b882-4a80-ba97-10b7a63b8fa4",
     "deletedDateTime": null,
     "classification": null,
     "createdDateTime": "2018-12-22T02:21:05Z",
     "description": "Self help community for golf",
     "displayName": "Golf Assist",
     "expirationDateTime": null,
     "groupTypes": [
         "Unified"
     ],
     "mail": "golfassist@contoso.com",
     "mailEnabled": true,
     "mailNickname": "golfassist",
     "membershipRule": null,
     "membershipRuleProcessingState": null,
     "onPremisesLastSyncDateTime": null,
     "onPremisesSecurityIdentifier": null,
     "onPremisesSyncEnabled": null,
     "preferredDataLocation": "CAN",
     "preferredLanguage": null,
     "proxyAddresses": [
         "SMTP:golfassist@contoso.onmicrosoft.com"
     ],
     "renewedDateTime": "2018-12-22T02:21:05Z",
     "resourceBehaviorOptions": [],
     "resourceProvisioningOptions": [],
     "securityEnabled": false,
     "theme": null,
     "visibility": "Public",
     "onPremisesProvisioningErrors": []
}
```

#### <a name="request-2"></a><span data-ttu-id="4c7ea-192">要求 2</span><span class="sxs-lookup"><span data-stu-id="4c7ea-192">Request 2</span></span>
<span data-ttu-id="4c7ea-193">2 つ目の要求例では、所有者とメンバーを指定して Office 365 グループを作成しています。</span><span class="sxs-lookup"><span data-stu-id="4c7ea-193">The second example request creates an Office 365 group with an owner and members specified.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_prepopulated_group"
}-->
```http
POST https://graph.microsoft.com/beta/groups
Content-Type: application/json

{
  "description": "Group with designated owner and members",
  "displayName": "Operations group",
  "groupTypes": [
    "Unified"
  ],
  "mailEnabled": true,
  "mailNickname": "operations2019",
  "securityEnabled": false,
  "owners@odata.bind": [
    "https://graph.microsoft.com/beta/users/26be1845-4119-4801-a799-aea79d09f1a2"
  ],
  "members@odata.bind": [
    "https://graph.microsoft.com/beta/users/ff7cb387-6688-423c-8188-3da9532a73cc",
    "https://graph.microsoft.com/beta/users/69456242-0067-49d3-ba96-9de6f2728e14"
  ]
}
```

#### <a name="response-2"></a><span data-ttu-id="4c7ea-194">応答 2</span><span class="sxs-lookup"><span data-stu-id="4c7ea-194">Response 2</span></span>
<span data-ttu-id="4c7ea-195">成功応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4c7ea-195">The following is an example of a successful response.</span></span> <span data-ttu-id="4c7ea-196">既定のプロパティのみが含まれています。</span><span class="sxs-lookup"><span data-stu-id="4c7ea-196">It includes only default properties.</span></span> <span data-ttu-id="4c7ea-197">その後は、グループの **owners** ナビゲーション プロパティまたは **members** ナビゲーション プロパティを取得して所有者またはメンバーの詳細を確認できます。</span><span class="sxs-lookup"><span data-stu-id="4c7ea-197">You can subsequently get the **owners** or **members** navigation properties of the group to verify the owner or members.</span></span> 
><span data-ttu-id="4c7ea-198">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="4c7ea-198">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4c7ea-199">実際の呼び出しからは、すべての既定のプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="4c7ea-199">All the default properties are returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "create_prepopulated_group"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups/$entity",
    "id": "502df398-d59c-469d-944f-34a50e60db3f",
    "deletedDateTime": null,
    "classification": null,
    "createdDateTime": "2018-12-27T22:17:07Z",
    "creationOptions": [],
    "description": "Group with designated owner and members",
    "displayName": "Operations group",
    "groupTypes": [
        "Unified"
    ],
    "mail": "operations2019@contoso.com",
    "mailEnabled": true,
    "mailNickname": "operations2019",
    "onPremisesLastSyncDateTime": null,
    "onPremisesSecurityIdentifier": null,
    "onPremisesSyncEnabled": null,
    "preferredDataLocation": "CAN",
    "proxyAddresses": [
        "SMTP:operations2019@contoso.com"
    ],
    "renewedDateTime": "2018-12-27T22:17:07Z",
    "resourceBehaviorOptions": [],
    "resourceProvisioningOptions": [],
    "securityEnabled": false,
    "visibility": "Public",
    "onPremisesProvisioningErrors": []
}
```

## <a name="see-also"></a><span data-ttu-id="4c7ea-200">関連項目</span><span class="sxs-lookup"><span data-stu-id="4c7ea-200">See also</span></span>

- [<span data-ttu-id="4c7ea-201">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="4c7ea-201">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="4c7ea-202">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="4c7ea-202">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="4c7ea-203">スキーマ拡張機能を使用したグループへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="4c7ea-203">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
