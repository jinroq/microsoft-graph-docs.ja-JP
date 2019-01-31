---
title: グループを作成する
description: この API を使用して、要求本文で指定した新しいグループを作成します。次に示す 3 種類のグループのうちの 1 つを作成できます。
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: 8bf432d30ba000641654d8c5d457096f5bfcb70e
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574867"
---
# <a name="create-group"></a><span data-ttu-id="2605e-104">グループを作成する</span><span class="sxs-lookup"><span data-stu-id="2605e-104">Create group</span></span>
<span data-ttu-id="2605e-p102">この API を使用して、要求本文で指定した新しいグループを作成します。次に示す 3 種類のグループのうちの 1 つを作成できます。</span><span class="sxs-lookup"><span data-stu-id="2605e-p102">Use this API to create a new group as specified in the request body. You can create one of three types of groups:</span></span>

* <span data-ttu-id="2605e-107">Office 365 グループ (統合グループ)</span><span class="sxs-lookup"><span data-stu-id="2605e-107">Office 365 Group (unified group)</span></span>
* <span data-ttu-id="2605e-108">動的グループ</span><span class="sxs-lookup"><span data-stu-id="2605e-108">Dynamic group</span></span>
* <span data-ttu-id="2605e-109">セキュリティ グループ</span><span class="sxs-lookup"><span data-stu-id="2605e-109">Security group</span></span>

<span data-ttu-id="2605e-110">この操作は既定で各グループのプロパティのサブセットのみを返します。</span><span class="sxs-lookup"><span data-stu-id="2605e-110">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="2605e-111">これらの既定のプロパティは、「[プロパティ](../resources/group.md#properties)」セクションに記載されています。</span><span class="sxs-lookup"><span data-stu-id="2605e-111">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span>

<span data-ttu-id="2605e-112">既定で_返されない_プロパティを取得するには、GET 操作を実行し、`$select` OData クエリ オプションでプロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="2605e-112">To get properties that are _not_ returned by default, do a GET operation for the group and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="2605e-113">[例](group-get.md#request-2)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2605e-113">See an [example](group-get.md#request-2).</span></span>

> <span data-ttu-id="2605e-p105">**注**:Microsoft Teams は Office 365 グループに基づいていますが、現在、この API を使用してチームを作成することはできません。Microsoft Teams UI で作成されたチームを管理するには、その他のグループ API を使用できます。</span><span class="sxs-lookup"><span data-stu-id="2605e-p105">**Note**: Although Microsoft Teams is built on Office 365 Groups, you can't currently create a team via this API. You can use the other group APIs to manage a team that has been created in the Microsoft Teams UI.</span></span>

## <a name="permissions"></a><span data-ttu-id="2605e-116">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2605e-116">Permissions</span></span>
<span data-ttu-id="2605e-p106">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2605e-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2605e-119">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2605e-119">Permission type</span></span>      | <span data-ttu-id="2605e-120">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2605e-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2605e-121">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2605e-121">Delegated (work or school account)</span></span> | <span data-ttu-id="2605e-122">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2605e-122">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="2605e-123">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2605e-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2605e-124">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2605e-124">Not supported.</span></span>    |
|<span data-ttu-id="2605e-125">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2605e-125">Application</span></span> | <span data-ttu-id="2605e-126">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2605e-126">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2605e-127">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2605e-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="2605e-128">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2605e-128">Request headers</span></span>
| <span data-ttu-id="2605e-129">名前</span><span class="sxs-lookup"><span data-stu-id="2605e-129">Name</span></span>       | <span data-ttu-id="2605e-130">型</span><span class="sxs-lookup"><span data-stu-id="2605e-130">Type</span></span> | <span data-ttu-id="2605e-131">説明</span><span class="sxs-lookup"><span data-stu-id="2605e-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2605e-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="2605e-132">Authorization</span></span>  | <span data-ttu-id="2605e-133">string</span><span class="sxs-lookup"><span data-stu-id="2605e-133">string</span></span>  | <span data-ttu-id="2605e-p107">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2605e-p107">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2605e-136">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2605e-136">Content-Type</span></span>  | <span data-ttu-id="2605e-137">application/json</span><span class="sxs-lookup"><span data-stu-id="2605e-137">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2605e-138">要求本文</span><span class="sxs-lookup"><span data-stu-id="2605e-138">Request body</span></span>
<span data-ttu-id="2605e-139">次の表は、グループを作成するときに指定する [group](../resources/group.md) リソースのプロパティを示しています。</span><span class="sxs-lookup"><span data-stu-id="2605e-139">The following table shows the properties of the [group](../resources/group.md) resource that you must specify at a minimum when you create a group.</span></span> 

| <span data-ttu-id="2605e-140">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2605e-140">Property</span></span> | <span data-ttu-id="2605e-141">型</span><span class="sxs-lookup"><span data-stu-id="2605e-141">Type</span></span> | <span data-ttu-id="2605e-142">説明</span><span class="sxs-lookup"><span data-stu-id="2605e-142">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2605e-143">displayName</span><span class="sxs-lookup"><span data-stu-id="2605e-143">displayName</span></span> | <span data-ttu-id="2605e-144">string</span><span class="sxs-lookup"><span data-stu-id="2605e-144">string</span></span> | <span data-ttu-id="2605e-145">アドレス帳に表示するグループの名前。</span><span class="sxs-lookup"><span data-stu-id="2605e-145">The name to display in the address book for the group.</span></span> <span data-ttu-id="2605e-146">必須です。</span><span class="sxs-lookup"><span data-stu-id="2605e-146">Required.</span></span> |
| <span data-ttu-id="2605e-147">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="2605e-147">mailEnabled</span></span> | <span data-ttu-id="2605e-148">boolean</span><span class="sxs-lookup"><span data-stu-id="2605e-148">boolean</span></span> | <span data-ttu-id="2605e-149">メールが有効なグループの場合は、**true** に設定します。</span><span class="sxs-lookup"><span data-stu-id="2605e-149">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="2605e-150">Office 365 グループを作成する場合は、これを **true** に設定します。</span><span class="sxs-lookup"><span data-stu-id="2605e-150">Set this to **true** if creating an Office 365 Group.</span></span> <span data-ttu-id="2605e-151">動的グループまたはセキュリティ グループを作成する場合は、これを **false** に設定します。</span><span class="sxs-lookup"><span data-stu-id="2605e-151">Set this to **false** if creating dynamic or security group.</span></span> <span data-ttu-id="2605e-152">必須です。</span><span class="sxs-lookup"><span data-stu-id="2605e-152">Required.</span></span> |
| <span data-ttu-id="2605e-153">mailNickname</span><span class="sxs-lookup"><span data-stu-id="2605e-153">mailNickname</span></span> | <span data-ttu-id="2605e-154">string</span><span class="sxs-lookup"><span data-stu-id="2605e-154">string</span></span> | <span data-ttu-id="2605e-155">グループのメール エイリアス。</span><span class="sxs-lookup"><span data-stu-id="2605e-155">The mail alias for the group.</span></span> <span data-ttu-id="2605e-156">必須です。</span><span class="sxs-lookup"><span data-stu-id="2605e-156">Required.</span></span> |
| <span data-ttu-id="2605e-157">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="2605e-157">securityEnabled</span></span> | <span data-ttu-id="2605e-158">ブール値</span><span class="sxs-lookup"><span data-stu-id="2605e-158">boolean</span></span> | <span data-ttu-id="2605e-159">セキュリティが有効なグループの場合は、**true** に設定します。</span><span class="sxs-lookup"><span data-stu-id="2605e-159">Set to **true** for security-enabled groups.</span></span> <span data-ttu-id="2605e-160">動的グループまたはセキュリティ グループを作成する場合は、これを **true** に設定します。</span><span class="sxs-lookup"><span data-stu-id="2605e-160">Set this to **true** if creating a dynamic or security group.</span></span> <span data-ttu-id="2605e-161">Office 365 グループを作成する場合は、これを **false** に設定します。</span><span class="sxs-lookup"><span data-stu-id="2605e-161">Set this to **false** if creating an Office 365 group.</span></span> <span data-ttu-id="2605e-162">必須です。</span><span class="sxs-lookup"><span data-stu-id="2605e-162">Required.</span></span> |
| <span data-ttu-id="2605e-163">owners</span><span class="sxs-lookup"><span data-stu-id="2605e-163">owners</span></span> | <span data-ttu-id="2605e-164">string collection</span><span class="sxs-lookup"><span data-stu-id="2605e-164">string collection</span></span> | <span data-ttu-id="2605e-165">このプロパティは、作成時のグループの所有者を表します。</span><span class="sxs-lookup"><span data-stu-id="2605e-165">This property represents the owners for the group at creation time.</span></span> <span data-ttu-id="2605e-166">省略可能。</span><span class="sxs-lookup"><span data-stu-id="2605e-166">Optional.</span></span> |
| <span data-ttu-id="2605e-167">members</span><span class="sxs-lookup"><span data-stu-id="2605e-167">members</span></span> | <span data-ttu-id="2605e-168">string collection</span><span class="sxs-lookup"><span data-stu-id="2605e-168">string collection</span></span> | <span data-ttu-id="2605e-169">このプロパティは、作成時のグループのメンバーを表します。</span><span class="sxs-lookup"><span data-stu-id="2605e-169">This property represents the members for the group at creation time.</span></span> <span data-ttu-id="2605e-170">省略可能。</span><span class="sxs-lookup"><span data-stu-id="2605e-170">Optional.</span></span> |


<span data-ttu-id="2605e-171">Office 365 グループまたは動的グループを作成している場合は、以下のように **groupTypes** プロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="2605e-171">Specify the **groupTypes** property if you're creating an Office 365 or dynamic group, as stated below.</span></span>

### <a name="grouptypes-options"></a><span data-ttu-id="2605e-172">groupTypes オプション</span><span class="sxs-lookup"><span data-stu-id="2605e-172">groupTypes options</span></span>

| <span data-ttu-id="2605e-173">グループの種類</span><span class="sxs-lookup"><span data-stu-id="2605e-173">Type of group</span></span> | <span data-ttu-id="2605e-174">**groupTypes** プロパティ</span><span class="sxs-lookup"><span data-stu-id="2605e-174">**groupTypes** property</span></span> |
|:--------------|:------------------------|
| <span data-ttu-id="2605e-175">Office 365 (統合グループともいいます)</span><span class="sxs-lookup"><span data-stu-id="2605e-175">Office 365 (aka unified group)</span></span>| <span data-ttu-id="2605e-176">"Unified"</span><span class="sxs-lookup"><span data-stu-id="2605e-176">"Unified"</span></span> |
| <span data-ttu-id="2605e-177">Dynamic</span><span class="sxs-lookup"><span data-stu-id="2605e-177">Dynamic</span></span> | <span data-ttu-id="2605e-178">"DynamicMembership"</span><span class="sxs-lookup"><span data-stu-id="2605e-178">"DynamicMembership"</span></span> |
| <span data-ttu-id="2605e-179">Security</span><span class="sxs-lookup"><span data-stu-id="2605e-179">Security</span></span> | <span data-ttu-id="2605e-180">設定しない。</span><span class="sxs-lookup"><span data-stu-id="2605e-180">Do not set.</span></span> |


><span data-ttu-id="2605e-181">**注:** ユーザー コンテキストを使用せず、所有者を指定せずにプログラムで Office 365 グループを作成すると、そのグループは匿名で作成されます。</span><span class="sxs-lookup"><span data-stu-id="2605e-181">**Note:** Creating an Office 365 Group programmatically without a user context and  without specifying owners will create the group anonymously.</span></span>  <span data-ttu-id="2605e-182">この操作を行うと、さらに手動操作が行われるまで、関連付けられている SharePoint Online サイトが自動的に作成されない可能性があります。</span><span class="sxs-lookup"><span data-stu-id="2605e-182">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  

<span data-ttu-id="2605e-p115">グループの必要に応じて他の書き込み可能なプロパティを指定します。詳細については、[group](../resources/group.md) リソースのプロパティを参照してください。</span><span class="sxs-lookup"><span data-stu-id="2605e-p115">Specify other writable properties as necessary for your group. For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

## <a name="response"></a><span data-ttu-id="2605e-185">応答</span><span class="sxs-lookup"><span data-stu-id="2605e-185">Response</span></span>
<span data-ttu-id="2605e-186">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [group](../resources/group.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2605e-186">If successful, this method returns `201 Created` response code and [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="2605e-187">応答には、そのグループの既定のプロパティのみが含まれます。</span><span class="sxs-lookup"><span data-stu-id="2605e-187">The response includes only the default properties of each group.</span></span>

## <a name="example"></a><span data-ttu-id="2605e-188">例</span><span class="sxs-lookup"><span data-stu-id="2605e-188">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="2605e-189">要求 1</span><span class="sxs-lookup"><span data-stu-id="2605e-189">Request 1</span></span>
<span data-ttu-id="2605e-190">最初の要求例では、Office 365 グループを作成しています。</span><span class="sxs-lookup"><span data-stu-id="2605e-190">The following is an example of a request that creates an Office 365 Group.</span></span>
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

#### <a name="response-1"></a><span data-ttu-id="2605e-191">応答 1</span><span class="sxs-lookup"><span data-stu-id="2605e-191">Response 1</span></span>
<span data-ttu-id="2605e-192">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2605e-192">The following is an example of the response.</span></span>
><span data-ttu-id="2605e-193">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="2605e-193">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="2605e-194">実際の呼び出しからは、すべての既定のプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="2605e-194">All the default properties are returned in an actual call.</span></span>
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
    "id": "b320ee12-b1cd-4cca-b648-a437be61c5cd",
      "deletedDateTime": null,
      "classification": null,
      "createdDateTime": "2018-12-22T00:51:37Z",
      "creationOptions": [],
      "description": "Self help community for library",
      "displayName": "Library Assist",
      "groupTypes": [
          "Unified"
      ],
      "mail": "library7423@contoso.com",
      "mailEnabled": true,
      "mailNickname": "library",
      "onPremisesLastSyncDateTime": null,
      "onPremisesSecurityIdentifier": null,
      "onPremisesSyncEnabled": null,
      "preferredDataLocation": "CAN",
      "proxyAddresses": [
          "SMTP:library7423@contoso.com"
      ],
      "renewedDateTime": "2018-12-22T00:51:37Z",
      "resourceBehaviorOptions": [],
      "resourceProvisioningOptions": [],
      "securityEnabled": false,
      "visibility": "Public",
      "onPremisesProvisioningErrors": []
}
```

#### <a name="request-2"></a><span data-ttu-id="2605e-195">要求 2</span><span class="sxs-lookup"><span data-stu-id="2605e-195">Request 2</span></span>
<span data-ttu-id="2605e-196">2 つ目の要求例では、所有者とメンバーを指定して Office 365 グループを作成しています。</span><span class="sxs-lookup"><span data-stu-id="2605e-196">The second example request creates an Office 365 group with an owner and members specified.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_prepopulated_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups
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
    "https://graph.microsoft.com/v1.0/users/26be1845-4119-4801-a799-aea79d09f1a2"
  ],
  "members@odata.bind": [
    "https://graph.microsoft.com/v1.0/users/ff7cb387-6688-423c-8188-3da9532a73cc",
    "https://graph.microsoft.com/v1.0/users/69456242-0067-49d3-ba96-9de6f2728e14"
  ]
}
```

#### <a name="response-2"></a><span data-ttu-id="2605e-197">応答 2</span><span class="sxs-lookup"><span data-stu-id="2605e-197">Response 2</span></span>
<span data-ttu-id="2605e-198">成功応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2605e-198">The following is an example of a response.</span></span> <span data-ttu-id="2605e-199">既定のプロパティのみが含まれています。</span><span class="sxs-lookup"><span data-stu-id="2605e-199">It includes only the default properties.</span></span> <span data-ttu-id="2605e-200">その後は、グループの **owners** ナビゲーション プロパティまたは **members** ナビゲーション プロパティを取得して所有者またはメンバーの詳細を確認できます。</span><span class="sxs-lookup"><span data-stu-id="2605e-200">You can subsequently get the **owners** or **members** navigation properties of the group to verify the owner or members.</span></span> 
><span data-ttu-id="2605e-201">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="2605e-201">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="2605e-202">実際の呼び出しからは、すべての既定のプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="2605e-202">All the default properties are returned in an actual call.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups/$entity",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
