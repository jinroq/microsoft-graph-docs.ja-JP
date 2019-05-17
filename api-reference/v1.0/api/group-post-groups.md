---
title: グループを作成する
description: '要求本文で指定した新しいグループを作成します。 '
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: baaf76455fefc6e44bf4995854d99baafb713005
ms.sourcegitcommit: 70ebcc469e2fdf2c31aeb6c5169f0101c3e698b0
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/15/2019
ms.locfileid: "34036375"
---
# <a name="create-group"></a><span data-ttu-id="fddff-103">グループを作成する</span><span class="sxs-lookup"><span data-stu-id="fddff-103">Create group</span></span>
<span data-ttu-id="fddff-104">要求本文で指定した新しいグループを作成します。</span><span class="sxs-lookup"><span data-stu-id="fddff-104">Use this API to create a new group as specified in the request body.</span></span> <span data-ttu-id="fddff-105">次に示す種類のグループを作成できます。</span><span class="sxs-lookup"><span data-stu-id="fddff-105">You can use the New-DistributionGroup cmdlet to create the following types of groups:</span></span>

* <span data-ttu-id="fddff-106">Office 365 グループ (統合グループ)</span><span class="sxs-lookup"><span data-stu-id="fddff-106">Office 365 Group (unified group)</span></span>
* <span data-ttu-id="fddff-107">セキュリティ グループ</span><span class="sxs-lookup"><span data-stu-id="fddff-107">Security group</span></span>

<span data-ttu-id="fddff-108">この操作は既定で各グループのプロパティのサブセットのみを返します。</span><span class="sxs-lookup"><span data-stu-id="fddff-108">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="fddff-109">これらの既定のプロパティは、「[プロパティ](../resources/group.md#properties)」セクションに記載されています。</span><span class="sxs-lookup"><span data-stu-id="fddff-109">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span>

<span data-ttu-id="fddff-110">既定で_返されない_プロパティを取得するには、GET 操作を実行し、`$select` OData クエリ オプションでプロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="fddff-110">To get properties that are _not_ returned by default, do a GET operation and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="fddff-111">[例](group-get.md#request-2)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fddff-111">See an [example](group-get.md#request-2).</span></span>

> <span data-ttu-id="fddff-p104">**注**:Microsoft Teams は Office 365 グループに基づいていますが、現在、この API を使用してチームを作成することはできません。Microsoft Teams UI で作成されたチームを管理するには、その他のグループ API を使用できます。</span><span class="sxs-lookup"><span data-stu-id="fddff-p104">**Note**: Although Microsoft Teams is built on Office 365 Groups, you can't currently create a team via this API. You can use the other group APIs to manage a team that has been created in the Microsoft Teams UI.</span></span>

## <a name="permissions"></a><span data-ttu-id="fddff-114">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="fddff-114">Permissions</span></span>
<span data-ttu-id="fddff-p105">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fddff-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fddff-117">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fddff-117">Permission type</span></span>      | <span data-ttu-id="fddff-118">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="fddff-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fddff-119">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fddff-119">Delegated (work or school account)</span></span> | <span data-ttu-id="fddff-120">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fddff-120">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="fddff-121">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fddff-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fddff-122">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fddff-122">Not supported.</span></span>    |
|<span data-ttu-id="fddff-123">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fddff-123">Application</span></span> | <span data-ttu-id="fddff-124">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fddff-124">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fddff-125">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fddff-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="fddff-126">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fddff-126">Request headers</span></span>
| <span data-ttu-id="fddff-127">名前</span><span class="sxs-lookup"><span data-stu-id="fddff-127">Name</span></span>       | <span data-ttu-id="fddff-128">型</span><span class="sxs-lookup"><span data-stu-id="fddff-128">Type</span></span> | <span data-ttu-id="fddff-129">説明</span><span class="sxs-lookup"><span data-stu-id="fddff-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fddff-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="fddff-130">Authorization</span></span>  | <span data-ttu-id="fddff-131">string</span><span class="sxs-lookup"><span data-stu-id="fddff-131">string</span></span>  | <span data-ttu-id="fddff-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="fddff-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fddff-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fddff-134">Content-Type</span></span>  | <span data-ttu-id="fddff-135">application/json</span><span class="sxs-lookup"><span data-stu-id="fddff-135">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fddff-136">要求本文</span><span class="sxs-lookup"><span data-stu-id="fddff-136">Request body</span></span>
<span data-ttu-id="fddff-137">次の表は、グループを作成するときに指定する [group](../resources/group.md) リソースのプロパティを示しています。</span><span class="sxs-lookup"><span data-stu-id="fddff-137">The following table shows the properties of the [group](../resources/group.md) resource to specify when you create a group.</span></span> 

| <span data-ttu-id="fddff-138">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fddff-138">Property</span></span> | <span data-ttu-id="fddff-139">型</span><span class="sxs-lookup"><span data-stu-id="fddff-139">Type</span></span> | <span data-ttu-id="fddff-140">説明</span><span class="sxs-lookup"><span data-stu-id="fddff-140">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fddff-141">displayName</span><span class="sxs-lookup"><span data-stu-id="fddff-141">displayName</span></span> | <span data-ttu-id="fddff-142">string</span><span class="sxs-lookup"><span data-stu-id="fddff-142">string</span></span> | <span data-ttu-id="fddff-143">アドレス帳に表示するグループの名前。</span><span class="sxs-lookup"><span data-stu-id="fddff-143">The name to display in the address book for the group.</span></span> <span data-ttu-id="fddff-144">必須です。</span><span class="sxs-lookup"><span data-stu-id="fddff-144">Required.</span></span> |
| <span data-ttu-id="fddff-145">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="fddff-145">mailEnabled</span></span> | <span data-ttu-id="fddff-146">boolean</span><span class="sxs-lookup"><span data-stu-id="fddff-146">boolean</span></span> | <span data-ttu-id="fddff-147">メールが有効なグループの場合は、**true** に設定します。</span><span class="sxs-lookup"><span data-stu-id="fddff-147">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="fddff-148">必須。</span><span class="sxs-lookup"><span data-stu-id="fddff-148">Required.</span></span> |
| <span data-ttu-id="fddff-149">mailNickname</span><span class="sxs-lookup"><span data-stu-id="fddff-149">mailNickname</span></span> | <span data-ttu-id="fddff-150">string</span><span class="sxs-lookup"><span data-stu-id="fddff-150">string</span></span> | <span data-ttu-id="fddff-151">グループのメール エイリアス。</span><span class="sxs-lookup"><span data-stu-id="fddff-151">The mail alias for the group.</span></span> <span data-ttu-id="fddff-152">必須です。</span><span class="sxs-lookup"><span data-stu-id="fddff-152">Required.</span></span> |
| <span data-ttu-id="fddff-153">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="fddff-153">securityEnabled</span></span> | <span data-ttu-id="fddff-154">ブール値</span><span class="sxs-lookup"><span data-stu-id="fddff-154">boolean</span></span> | <span data-ttu-id="fddff-155">Office 365 グループを含む、セキュリティが有効なグループに **true** を設定します。</span><span class="sxs-lookup"><span data-stu-id="fddff-155">Set to **true** for security-enabled groups, including Office 365 groups.</span></span> <span data-ttu-id="fddff-156">必須。</span><span class="sxs-lookup"><span data-stu-id="fddff-156">Required.</span></span> |
| <span data-ttu-id="fddff-157">owners</span><span class="sxs-lookup"><span data-stu-id="fddff-157">owners</span></span> | <span data-ttu-id="fddff-158">string collection</span><span class="sxs-lookup"><span data-stu-id="fddff-158">string collection</span></span> | <span data-ttu-id="fddff-159">このプロパティは、作成時のグループの所有者を表します。</span><span class="sxs-lookup"><span data-stu-id="fddff-159">This property represents the owners for the group at creation time.</span></span> <span data-ttu-id="fddff-160">省略可能。</span><span class="sxs-lookup"><span data-stu-id="fddff-160">Optional.</span></span> |
| <span data-ttu-id="fddff-161">members</span><span class="sxs-lookup"><span data-stu-id="fddff-161">members</span></span> | <span data-ttu-id="fddff-162">string collection</span><span class="sxs-lookup"><span data-stu-id="fddff-162">string collection</span></span> | <span data-ttu-id="fddff-163">このプロパティは、作成時のグループのメンバーを表します。</span><span class="sxs-lookup"><span data-stu-id="fddff-163">This property represents the members for the group at creation time.</span></span> <span data-ttu-id="fddff-164">省略可能。</span><span class="sxs-lookup"><span data-stu-id="fddff-164">Optional.</span></span> |

> <span data-ttu-id="fddff-165">注: Microsoft Azure portal を使用して作成されるグループでは、**securityEnabled** と **mailEnabled** は最初は常に `true` に設定されます。</span><span class="sxs-lookup"><span data-stu-id="fddff-165">Note: Groups created using the Microsoft Azure portal always have **securityEnabled** and **mailEnabled** initially set to `true`.</span></span>

<span data-ttu-id="fddff-166">グループの必要に応じて他の書き込み可能なプロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="fddff-166">Specify other writable properties as necessary for your group.</span></span> <span data-ttu-id="fddff-167">詳細については、[group](../resources/group.md) リソースのプロパティをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="fddff-167">For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

><span data-ttu-id="fddff-168">**注:**  ユーザー コンテキストを使用せず、所有者を指定せずにプログラムで Office 365 グループを作成すると、そのグループは匿名で作成されます。</span><span class="sxs-lookup"><span data-stu-id="fddff-168">**Note:** Creating an Office 365 Group programmatically without a user context and  without specifying owners will create the group anonymously.</span></span>  <span data-ttu-id="fddff-169">この操作を行うと、さらに手動操作が行われるまで、関連付けられている SharePoint Online サイトが自動的に作成されない可能性があります。</span><span class="sxs-lookup"><span data-stu-id="fddff-169">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  

### <a name="grouptypes-options"></a><span data-ttu-id="fddff-170">groupTypes オプション</span><span class="sxs-lookup"><span data-stu-id="fddff-170">groupTypes options</span></span>

<span data-ttu-id="fddff-171">以下に示すように、**groupTypes** プロパティを使用し、グループの種類とグループのメンバーシップを管理します:</span><span class="sxs-lookup"><span data-stu-id="fddff-171">Use the **groupTypes** property to control the type of group and its membership, as shown below:</span></span>

| <span data-ttu-id="fddff-172">グループの種類</span><span class="sxs-lookup"><span data-stu-id="fddff-172">Type of group</span></span> | <span data-ttu-id="fddff-173">割り当て済みのメンバーシップ</span><span class="sxs-lookup"><span data-stu-id="fddff-173">Assigned membership</span></span> | <span data-ttu-id="fddff-174">動的メンバーシップ</span><span class="sxs-lookup"><span data-stu-id="fddff-174">Dynamic membership</span></span> |
|:--------------|:------------------------|:---------------|
| <span data-ttu-id="fddff-175">Office 365 (統合グループともいいます)</span><span class="sxs-lookup"><span data-stu-id="fddff-175">Office 365 (aka unified group)</span></span>| `["Unified"]` | `["Unified","DynamicMembership"]`
| <span data-ttu-id="fddff-176">Dynamic</span><span class="sxs-lookup"><span data-stu-id="fddff-176">Dynamic</span></span> | <span data-ttu-id="fddff-177">`[]` (_null_)</span><span class="sxs-lookup"><span data-stu-id="fddff-177">Null</span></span> | `["DynamicMembership"]`|

## <a name="response"></a><span data-ttu-id="fddff-178">応答</span><span class="sxs-lookup"><span data-stu-id="fddff-178">Response</span></span>
<span data-ttu-id="fddff-179">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [group](../resources/group.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="fddff-179">If successful, this method returns `201 Created` response code and [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="fddff-180">応答には、そのグループの既定のプロパティのみが含まれます。</span><span class="sxs-lookup"><span data-stu-id="fddff-180">The response includes only the default properties of the group.</span></span>

## <a name="examples"></a><span data-ttu-id="fddff-181">例</span><span class="sxs-lookup"><span data-stu-id="fddff-181">Examples</span></span>

### <a name="example-1-create-an-office-365-group"></a><span data-ttu-id="fddff-182">例 1: Office 365 グループを作成する</span><span class="sxs-lookup"><span data-stu-id="fddff-182">Create an Office 365 group</span></span>

<span data-ttu-id="fddff-183">次の例では、Office 365 グループを作成します。</span><span class="sxs-lookup"><span data-stu-id="fddff-183">The following example creates an Office 365 group.</span></span>

#### <a name="request"></a><span data-ttu-id="fddff-184">要求</span><span class="sxs-lookup"><span data-stu-id="fddff-184">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_group"
}-->
``` http
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

#### <a name="response"></a><span data-ttu-id="fddff-185">応答</span><span class="sxs-lookup"><span data-stu-id="fddff-185">Response</span></span>

<span data-ttu-id="fddff-186">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fddff-186">The following is an example of the response.</span></span>

><span data-ttu-id="fddff-187">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="fddff-187">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="fddff-188">実際の呼び出しからは、すべての既定のプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="fddff-188">All the default properties are returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "create_group"
} -->
``` http
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="fddff-189">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="fddff-189">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="fddff-190">C#</span><span class="sxs-lookup"><span data-stu-id="fddff-190">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fddff-191">Javascript</span><span class="sxs-lookup"><span data-stu-id="fddff-191">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_group-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="example-2-create-a-group-with-owners-and-members"></a><span data-ttu-id="fddff-192">例 2: 所有者とメンバーを指定してグループを作成する</span><span class="sxs-lookup"><span data-stu-id="fddff-192">Example 2: Create a group with owners and members</span></span>

<span data-ttu-id="fddff-193">次の例では、所有者とメンバーを指定して Office 365 グループを作成します。</span><span class="sxs-lookup"><span data-stu-id="fddff-193">The second example request creates an Office 365 group with an owner and members specified.</span></span>

#### <a name="request"></a><span data-ttu-id="fddff-194">要求</span><span class="sxs-lookup"><span data-stu-id="fddff-194">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_prepopulated_group"
}-->
``` http
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

#### <a name="response"></a><span data-ttu-id="fddff-195">応答</span><span class="sxs-lookup"><span data-stu-id="fddff-195">Response</span></span>

<span data-ttu-id="fddff-196">成功応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fddff-196">The following is an example of a successful response.</span></span> <span data-ttu-id="fddff-197">既定のプロパティのみが含まれています。</span><span class="sxs-lookup"><span data-stu-id="fddff-197">It includes only default properties.</span></span> <span data-ttu-id="fddff-198">その後は、グループの **owners** ナビゲーション プロパティまたは **members** ナビゲーション プロパティを取得して所有者またはメンバーの詳細を確認できます。</span><span class="sxs-lookup"><span data-stu-id="fddff-198">You can subsequently get the **owners** or **members** navigation properties of the group to verify the owner or members.</span></span> 

><span data-ttu-id="fddff-199">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="fddff-199">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="fddff-200">実際の呼び出しからは、すべての既定のプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="fddff-200">All the default properties are returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "create_prepopulated_group"
} -->
``` http
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="fddff-201">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="fddff-201">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="fddff-202">C#</span><span class="sxs-lookup"><span data-stu-id="fddff-202">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_prepopulated_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fddff-203">Javascript</span><span class="sxs-lookup"><span data-stu-id="fddff-203">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_prepopulated_group-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-post-groups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-post-groups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/group-post-groups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-post-groups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
