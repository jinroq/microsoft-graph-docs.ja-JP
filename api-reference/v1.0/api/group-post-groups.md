---
title: グループを作成する
description: '要求本文で指定した新しいグループを作成します。 '
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: b1fca0941b04099be02e2f9929c0683655dfeaa1
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35456408"
---
# <a name="create-group"></a><span data-ttu-id="8d1eb-103">グループを作成する</span><span class="sxs-lookup"><span data-stu-id="8d1eb-103">Create group</span></span>
<span data-ttu-id="8d1eb-104">要求本文で指定した新しいグループを作成します。</span><span class="sxs-lookup"><span data-stu-id="8d1eb-104">Use this API to create a new group as specified in the request body.</span></span> <span data-ttu-id="8d1eb-105">次に示す種類のグループを作成できます。</span><span class="sxs-lookup"><span data-stu-id="8d1eb-105">You can use the New-DistributionGroup cmdlet to create the following types of groups:</span></span>

* <span data-ttu-id="8d1eb-106">Office 365 グループ (統合グループ)</span><span class="sxs-lookup"><span data-stu-id="8d1eb-106">Office 365 Group (unified group)</span></span>
* <span data-ttu-id="8d1eb-107">セキュリティ グループ</span><span class="sxs-lookup"><span data-stu-id="8d1eb-107">Security group</span></span>

<span data-ttu-id="8d1eb-108">この操作は既定で各グループのプロパティのサブセットのみを返します。</span><span class="sxs-lookup"><span data-stu-id="8d1eb-108">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="8d1eb-109">これらの既定のプロパティは、「[プロパティ](../resources/group.md#properties)」セクションに記載されています。</span><span class="sxs-lookup"><span data-stu-id="8d1eb-109">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span>

<span data-ttu-id="8d1eb-110">既定で_返されない_プロパティを取得するには、[GET 操作](group-get.md)を実行し、`$select` OData クエリ オプションでプロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="8d1eb-110">To get properties that are _not_ returned by default, do a GET operation and specify the properties in a `$select` OData query option.</span></span>

> <span data-ttu-id="8d1eb-p103">**注**:Microsoft Teams は Office 365 グループに基づいていますが、現在、この API を使用してチームを作成することはできません。Microsoft Teams UI で作成されたチームを管理するには、その他のグループ API を使用できます。</span><span class="sxs-lookup"><span data-stu-id="8d1eb-p103">**Note**: Although Microsoft Teams is built on Office 365 Groups, you can't currently create a team via this API. You can use the other group APIs to manage a team that has been created in the Microsoft Teams UI.</span></span>

## <a name="permissions"></a><span data-ttu-id="8d1eb-113">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8d1eb-113">Permissions</span></span>
<span data-ttu-id="8d1eb-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8d1eb-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d1eb-116">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8d1eb-116">Permission type</span></span>      | <span data-ttu-id="8d1eb-117">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8d1eb-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8d1eb-118">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8d1eb-118">Delegated (work or school account)</span></span> | <span data-ttu-id="8d1eb-119">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8d1eb-119">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="8d1eb-120">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8d1eb-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d1eb-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8d1eb-121">Not supported.</span></span>    |
|<span data-ttu-id="8d1eb-122">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8d1eb-122">Application</span></span> | <span data-ttu-id="8d1eb-123">Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d1eb-123">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8d1eb-124">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8d1eb-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="8d1eb-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8d1eb-125">Request headers</span></span>
| <span data-ttu-id="8d1eb-126">名前</span><span class="sxs-lookup"><span data-stu-id="8d1eb-126">Name</span></span>       | <span data-ttu-id="8d1eb-127">型</span><span class="sxs-lookup"><span data-stu-id="8d1eb-127">Type</span></span> | <span data-ttu-id="8d1eb-128">説明</span><span class="sxs-lookup"><span data-stu-id="8d1eb-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8d1eb-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d1eb-129">Authorization</span></span>  | <span data-ttu-id="8d1eb-130">string</span><span class="sxs-lookup"><span data-stu-id="8d1eb-130">string</span></span>  | <span data-ttu-id="8d1eb-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8d1eb-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8d1eb-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8d1eb-133">Content-Type</span></span>  | <span data-ttu-id="8d1eb-134">application/json</span><span class="sxs-lookup"><span data-stu-id="8d1eb-134">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8d1eb-135">要求本文</span><span class="sxs-lookup"><span data-stu-id="8d1eb-135">Request body</span></span>
<span data-ttu-id="8d1eb-136">次の表は、グループを作成するときに指定する [group](../resources/group.md) リソースのプロパティを示しています。</span><span class="sxs-lookup"><span data-stu-id="8d1eb-136">The following table shows the properties of the [group](../resources/group.md) resource to specify when you create a group.</span></span> 

| <span data-ttu-id="8d1eb-137">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8d1eb-137">Property</span></span> | <span data-ttu-id="8d1eb-138">型</span><span class="sxs-lookup"><span data-stu-id="8d1eb-138">Type</span></span> | <span data-ttu-id="8d1eb-139">説明</span><span class="sxs-lookup"><span data-stu-id="8d1eb-139">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8d1eb-140">displayName</span><span class="sxs-lookup"><span data-stu-id="8d1eb-140">displayName</span></span> | <span data-ttu-id="8d1eb-141">string</span><span class="sxs-lookup"><span data-stu-id="8d1eb-141">string</span></span> | <span data-ttu-id="8d1eb-142">アドレス帳に表示するグループの名前。</span><span class="sxs-lookup"><span data-stu-id="8d1eb-142">The name to display in the address book for the group.</span></span> <span data-ttu-id="8d1eb-143">必須です。</span><span class="sxs-lookup"><span data-stu-id="8d1eb-143">Required.</span></span> |
| <span data-ttu-id="8d1eb-144">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="8d1eb-144">mailEnabled</span></span> | <span data-ttu-id="8d1eb-145">boolean</span><span class="sxs-lookup"><span data-stu-id="8d1eb-145">boolean</span></span> | <span data-ttu-id="8d1eb-146">メールが有効なグループの場合は、**true** に設定します。</span><span class="sxs-lookup"><span data-stu-id="8d1eb-146">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="8d1eb-147">必須。</span><span class="sxs-lookup"><span data-stu-id="8d1eb-147">Required.</span></span> |
| <span data-ttu-id="8d1eb-148">mailNickname</span><span class="sxs-lookup"><span data-stu-id="8d1eb-148">mailNickname</span></span> | <span data-ttu-id="8d1eb-149">string</span><span class="sxs-lookup"><span data-stu-id="8d1eb-149">string</span></span> | <span data-ttu-id="8d1eb-150">グループのメール エイリアス。</span><span class="sxs-lookup"><span data-stu-id="8d1eb-150">The mail alias for the group.</span></span> <span data-ttu-id="8d1eb-151">必須です。</span><span class="sxs-lookup"><span data-stu-id="8d1eb-151">Required.</span></span> |
| <span data-ttu-id="8d1eb-152">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="8d1eb-152">securityEnabled</span></span> | <span data-ttu-id="8d1eb-153">ブール値</span><span class="sxs-lookup"><span data-stu-id="8d1eb-153">boolean</span></span> | <span data-ttu-id="8d1eb-154">Office 365 グループを含む、セキュリティが有効なグループに **true** を設定します。</span><span class="sxs-lookup"><span data-stu-id="8d1eb-154">Set to **true** for security-enabled groups, including Office 365 groups.</span></span> <span data-ttu-id="8d1eb-155">必須。</span><span class="sxs-lookup"><span data-stu-id="8d1eb-155">Required.</span></span> |
| <span data-ttu-id="8d1eb-156">owners</span><span class="sxs-lookup"><span data-stu-id="8d1eb-156">owners</span></span> | <span data-ttu-id="8d1eb-157">string collection</span><span class="sxs-lookup"><span data-stu-id="8d1eb-157">string collection</span></span> | <span data-ttu-id="8d1eb-158">このプロパティは、作成時のグループの所有者を表します。</span><span class="sxs-lookup"><span data-stu-id="8d1eb-158">This property represents the owners for the group at creation time.</span></span> <span data-ttu-id="8d1eb-159">省略可能。</span><span class="sxs-lookup"><span data-stu-id="8d1eb-159">Optional.</span></span> |
| <span data-ttu-id="8d1eb-160">members</span><span class="sxs-lookup"><span data-stu-id="8d1eb-160">members</span></span> | <span data-ttu-id="8d1eb-161">string collection</span><span class="sxs-lookup"><span data-stu-id="8d1eb-161">string collection</span></span> | <span data-ttu-id="8d1eb-162">このプロパティは、作成時のグループのメンバーを表します。</span><span class="sxs-lookup"><span data-stu-id="8d1eb-162">This property represents the members for the group at creation time.</span></span> <span data-ttu-id="8d1eb-163">省略可能。</span><span class="sxs-lookup"><span data-stu-id="8d1eb-163">Optional.</span></span> |

> <span data-ttu-id="8d1eb-164">**注**: Microsoft Azure portal を使用して作成されるグループでは、**securityEnabled** は最初は常に `true` に設定されます。</span><span class="sxs-lookup"><span data-stu-id="8d1eb-164">**Note:** Groups created using the Microsoft Azure portal always have **securityEnabled** initially set to `true`.</span></span>

<span data-ttu-id="8d1eb-165">グループの必要に応じて他の書き込み可能なプロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="8d1eb-165">Specify other writable properties as necessary for your group.</span></span> <span data-ttu-id="8d1eb-166">詳細については、[group](../resources/group.md) リソースのプロパティをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="8d1eb-166">For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

><span data-ttu-id="8d1eb-167">**注:**  ユーザー コンテキストを使用せず、所有者を指定せずにプログラムで Office 365 グループを作成すると、そのグループは匿名で作成されます。</span><span class="sxs-lookup"><span data-stu-id="8d1eb-167">**Note:** Creating an Office 365 Group programmatically without a user context and  without specifying owners will create the group anonymously.</span></span>  <span data-ttu-id="8d1eb-168">この操作を行うと、さらに手動操作が行われるまで、関連付けられている SharePoint Online サイトが自動的に作成されない可能性があります。</span><span class="sxs-lookup"><span data-stu-id="8d1eb-168">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  

### <a name="grouptypes-options"></a><span data-ttu-id="8d1eb-169">groupTypes オプション</span><span class="sxs-lookup"><span data-stu-id="8d1eb-169">groupTypes options</span></span>

<span data-ttu-id="8d1eb-170">以下に示すように、**groupTypes** プロパティを使用し、グループの種類とグループのメンバーシップを管理します:</span><span class="sxs-lookup"><span data-stu-id="8d1eb-170">Use the **groupTypes** property to control the type of group and its membership, as shown below:</span></span>

| <span data-ttu-id="8d1eb-171">グループの種類</span><span class="sxs-lookup"><span data-stu-id="8d1eb-171">Type of group</span></span> | <span data-ttu-id="8d1eb-172">割り当て済みのメンバーシップ</span><span class="sxs-lookup"><span data-stu-id="8d1eb-172">Assigned membership</span></span> | <span data-ttu-id="8d1eb-173">動的メンバーシップ</span><span class="sxs-lookup"><span data-stu-id="8d1eb-173">Dynamic membership</span></span> |
|:--------------|:------------------------|:---------------|
| <span data-ttu-id="8d1eb-174">Office 365 (統合グループともいいます)</span><span class="sxs-lookup"><span data-stu-id="8d1eb-174">Office 365 (aka unified group)</span></span>| `["Unified"]` | `["Unified","DynamicMembership"]`
| <span data-ttu-id="8d1eb-175">Dynamic</span><span class="sxs-lookup"><span data-stu-id="8d1eb-175">Dynamic</span></span> | <span data-ttu-id="8d1eb-176">`[]` (_null_)</span><span class="sxs-lookup"><span data-stu-id="8d1eb-176">Null</span></span> | `["DynamicMembership"]`|

## <a name="response"></a><span data-ttu-id="8d1eb-177">応答</span><span class="sxs-lookup"><span data-stu-id="8d1eb-177">Response</span></span>
<span data-ttu-id="8d1eb-178">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [group](../resources/group.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8d1eb-178">If successful, this method returns `201 Created` response code and [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="8d1eb-179">応答には、そのグループの既定のプロパティのみが含まれます。</span><span class="sxs-lookup"><span data-stu-id="8d1eb-179">The response includes only the default properties of the group.</span></span>

## <a name="examples"></a><span data-ttu-id="8d1eb-180">例</span><span class="sxs-lookup"><span data-stu-id="8d1eb-180">Examples</span></span>

### <a name="example-1-create-an-office-365-group"></a><span data-ttu-id="8d1eb-181">例 1: Office 365 グループを作成する</span><span class="sxs-lookup"><span data-stu-id="8d1eb-181">Create an Office 365 group</span></span>

<span data-ttu-id="8d1eb-182">次の例では、Office 365 グループを作成します。</span><span class="sxs-lookup"><span data-stu-id="8d1eb-182">The following example creates an Office 365 group.</span></span>

#### <a name="request"></a><span data-ttu-id="8d1eb-183">要求</span><span class="sxs-lookup"><span data-stu-id="8d1eb-183">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="8d1eb-184">HTTP</span><span class="sxs-lookup"><span data-stu-id="8d1eb-184">--Http</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="8d1eb-185">C#</span><span class="sxs-lookup"><span data-stu-id="8d1eb-185">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8d1eb-186">Javascript</span><span class="sxs-lookup"><span data-stu-id="8d1eb-186">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8d1eb-187">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8d1eb-187">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8d1eb-188">応答</span><span class="sxs-lookup"><span data-stu-id="8d1eb-188">Response</span></span>

<span data-ttu-id="8d1eb-189">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8d1eb-189">The following is an example of the response.</span></span>

><span data-ttu-id="8d1eb-190">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="8d1eb-190">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="8d1eb-191">実際の呼び出しからは、すべての既定のプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="8d1eb-191">All the default properties are returned from an actual call.</span></span>
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

### <a name="example-2-create-a-group-with-owners-and-members"></a><span data-ttu-id="8d1eb-192">例 2: 所有者とメンバーを指定してグループを作成する</span><span class="sxs-lookup"><span data-stu-id="8d1eb-192">Example 2: Create a group with owners and members</span></span>

<span data-ttu-id="8d1eb-193">次の例では、所有者とメンバーを指定して Office 365 グループを作成します。</span><span class="sxs-lookup"><span data-stu-id="8d1eb-193">The second example request creates an Office 365 group with an owner and members specified.</span></span>

#### <a name="request"></a><span data-ttu-id="8d1eb-194">要求</span><span class="sxs-lookup"><span data-stu-id="8d1eb-194">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="8d1eb-195">HTTP</span><span class="sxs-lookup"><span data-stu-id="8d1eb-195">--Http</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="8d1eb-196">C#</span><span class="sxs-lookup"><span data-stu-id="8d1eb-196">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-prepopulated-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8d1eb-197">Javascript</span><span class="sxs-lookup"><span data-stu-id="8d1eb-197">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-prepopulated-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8d1eb-198">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8d1eb-198">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-prepopulated-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8d1eb-199">応答</span><span class="sxs-lookup"><span data-stu-id="8d1eb-199">Response</span></span>

<span data-ttu-id="8d1eb-200">成功応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8d1eb-200">The following is an example of a successful response.</span></span> <span data-ttu-id="8d1eb-201">既定のプロパティのみが含まれています。</span><span class="sxs-lookup"><span data-stu-id="8d1eb-201">It includes only default properties.</span></span> <span data-ttu-id="8d1eb-202">その後は、グループの **owners** ナビゲーション プロパティまたは **members** ナビゲーション プロパティを取得して所有者またはメンバーの詳細を確認できます。</span><span class="sxs-lookup"><span data-stu-id="8d1eb-202">You can subsequently get the **owners** or **members** navigation properties of the group to verify the owner or members.</span></span> 

><span data-ttu-id="8d1eb-203">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="8d1eb-203">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="8d1eb-204">実際の呼び出しからは、すべての既定のプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="8d1eb-204">All the default properties are returned from an actual call.</span></span>

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
