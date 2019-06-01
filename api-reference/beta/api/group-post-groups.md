---
title: グループを作成する
description: 新しい Office 365 グループまたはセキュリティ グループを作成してください。
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: c91c43c0156aa4edda9eef71232001fdede38887
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536198"
---
# <a name="create-group"></a><span data-ttu-id="2fafa-103">グループを作成する</span><span class="sxs-lookup"><span data-stu-id="2fafa-103">Create group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2fafa-104">要求本文で指定した新しい[グループ](../resources/group.md)を作成します。</span><span class="sxs-lookup"><span data-stu-id="2fafa-104">Use this API to create a new [group](../resources/group.md) as specified in the request body.</span></span> <span data-ttu-id="2fafa-105">以下のいずれかのグループを作成できます:</span><span class="sxs-lookup"><span data-stu-id="2fafa-105">You can create one of the following groups:</span></span>

* <span data-ttu-id="2fafa-106">Office 365 グループ (統合グループ)</span><span class="sxs-lookup"><span data-stu-id="2fafa-106">Office 365 Group (unified group)</span></span>
* <span data-ttu-id="2fafa-107">セキュリティ グループ</span><span class="sxs-lookup"><span data-stu-id="2fafa-107">Security group</span></span>

<span data-ttu-id="2fafa-108">この操作は既定で各グループのプロパティのサブセットのみを返します。</span><span class="sxs-lookup"><span data-stu-id="2fafa-108">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="2fafa-109">これらの既定のプロパティは、「[プロパティ](../resources/group.md#properties)」セクションに記載されています。</span><span class="sxs-lookup"><span data-stu-id="2fafa-109">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span>

<span data-ttu-id="2fafa-110">既定で_返されない_プロパティを取得するには、GET 操作を実行し、`$select` OData クエリ オプションでプロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="2fafa-110">To get properties that are _not_ returned by default, do a GET operation and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="2fafa-111">[例](group-get.md#request-2)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2fafa-111">See an [example](group-get.md#request-2).</span></span>

><span data-ttu-id="2fafa-112">**注:** [チーム](../resources/team.md)を作成するには、まずグループを作成し、それからそのグループにチームを追加します。[チームの作成](../api/team-put-teams.md)に関するページを参照してください。</span><span class="sxs-lookup"><span data-stu-id="2fafa-112">**Note**: To create a [team](../resources/team.md), first create a group then add a team to it, see [create team](../api/team-put-teams.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2fafa-113">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2fafa-113">Permissions</span></span>
<span data-ttu-id="2fafa-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2fafa-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2fafa-116">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2fafa-116">Permission type</span></span>      | <span data-ttu-id="2fafa-117">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2fafa-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2fafa-118">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2fafa-118">Delegated (work or school account)</span></span> | <span data-ttu-id="2fafa-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2fafa-119">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="2fafa-120">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2fafa-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2fafa-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2fafa-121">Not supported.</span></span>    |
|<span data-ttu-id="2fafa-122">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2fafa-122">Application</span></span> | <span data-ttu-id="2fafa-123">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2fafa-123">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2fafa-124">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2fafa-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="2fafa-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2fafa-125">Request headers</span></span>

| <span data-ttu-id="2fafa-126">名前</span><span class="sxs-lookup"><span data-stu-id="2fafa-126">Name</span></span>       | <span data-ttu-id="2fafa-127">型</span><span class="sxs-lookup"><span data-stu-id="2fafa-127">Type</span></span> | <span data-ttu-id="2fafa-128">説明</span><span class="sxs-lookup"><span data-stu-id="2fafa-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2fafa-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="2fafa-129">Authorization</span></span>  | <span data-ttu-id="2fafa-130">string</span><span class="sxs-lookup"><span data-stu-id="2fafa-130">string</span></span>  | <span data-ttu-id="2fafa-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2fafa-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2fafa-133">要求本文</span><span class="sxs-lookup"><span data-stu-id="2fafa-133">Request body</span></span>

<span data-ttu-id="2fafa-134">次の表は、グループを作成するときに指定する [group](../resources/group.md) リソースのプロパティを示しています。</span><span class="sxs-lookup"><span data-stu-id="2fafa-134">The following table shows the properties of the [group](../resources/group.md) resource to specify when you create a group.</span></span> 

| <span data-ttu-id="2fafa-135">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2fafa-135">Property</span></span> | <span data-ttu-id="2fafa-136">型</span><span class="sxs-lookup"><span data-stu-id="2fafa-136">Type</span></span> | <span data-ttu-id="2fafa-137">説明</span><span class="sxs-lookup"><span data-stu-id="2fafa-137">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2fafa-138">displayName</span><span class="sxs-lookup"><span data-stu-id="2fafa-138">displayName</span></span> | <span data-ttu-id="2fafa-139">string</span><span class="sxs-lookup"><span data-stu-id="2fafa-139">string</span></span> | <span data-ttu-id="2fafa-140">アドレス帳に表示するグループの名前。</span><span class="sxs-lookup"><span data-stu-id="2fafa-140">The name to display in the address book for the group.</span></span> <span data-ttu-id="2fafa-141">必須です。</span><span class="sxs-lookup"><span data-stu-id="2fafa-141">Required.</span></span> |
| <span data-ttu-id="2fafa-142">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="2fafa-142">mailEnabled</span></span> | <span data-ttu-id="2fafa-143">boolean</span><span class="sxs-lookup"><span data-stu-id="2fafa-143">boolean</span></span> | <span data-ttu-id="2fafa-144">メールが有効なグループの場合は、**true** に設定します。</span><span class="sxs-lookup"><span data-stu-id="2fafa-144">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="2fafa-145">必須。</span><span class="sxs-lookup"><span data-stu-id="2fafa-145">Required.</span></span> |
| <span data-ttu-id="2fafa-146">mailNickname</span><span class="sxs-lookup"><span data-stu-id="2fafa-146">mailNickname</span></span> | <span data-ttu-id="2fafa-147">string</span><span class="sxs-lookup"><span data-stu-id="2fafa-147">string</span></span> | <span data-ttu-id="2fafa-148">グループのメール エイリアス。</span><span class="sxs-lookup"><span data-stu-id="2fafa-148">The mail alias for the group.</span></span> <span data-ttu-id="2fafa-149">必須です。</span><span class="sxs-lookup"><span data-stu-id="2fafa-149">Required.</span></span> |
| <span data-ttu-id="2fafa-150">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="2fafa-150">securityEnabled</span></span> | <span data-ttu-id="2fafa-151">ブール値</span><span class="sxs-lookup"><span data-stu-id="2fafa-151">boolean</span></span> | <span data-ttu-id="2fafa-152">Office 365 グループを含む、セキュリティが有効なグループに **true** を設定します。</span><span class="sxs-lookup"><span data-stu-id="2fafa-152">Set to **true** for security-enabled groups, including Office 365 groups.</span></span> <span data-ttu-id="2fafa-153">必須。</span><span class="sxs-lookup"><span data-stu-id="2fafa-153">Required.</span></span> |
| <span data-ttu-id="2fafa-154">owners</span><span class="sxs-lookup"><span data-stu-id="2fafa-154">owners</span></span> | <span data-ttu-id="2fafa-155">[directoryObject](../resources/directoryobject.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2fafa-155">[directoryObject](../resources/directoryobject.md) collection</span></span> | <span data-ttu-id="2fafa-156">このプロパティは、作成時のグループの所有者を表します。</span><span class="sxs-lookup"><span data-stu-id="2fafa-156">This property represents the owners for the group at creation time.</span></span> <span data-ttu-id="2fafa-157">省略可能。</span><span class="sxs-lookup"><span data-stu-id="2fafa-157">Optional.</span></span> |
| <span data-ttu-id="2fafa-158">members</span><span class="sxs-lookup"><span data-stu-id="2fafa-158">members</span></span> | <span data-ttu-id="2fafa-159">[directoryObject](../resources/directoryobject.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2fafa-159">[directoryObject](../resources/directoryobject.md) collection</span></span> | <span data-ttu-id="2fafa-160">このプロパティは、作成時のグループのメンバーを表します。</span><span class="sxs-lookup"><span data-stu-id="2fafa-160">This property represents the members for the group at creation time.</span></span> <span data-ttu-id="2fafa-161">省略可能。</span><span class="sxs-lookup"><span data-stu-id="2fafa-161">Optional.</span></span> |

> <span data-ttu-id="2fafa-162">**注**: Microsoft Azure portal を使用して作成されるグループでは、**securityEnabled** は最初は常に `true` に設定されます。</span><span class="sxs-lookup"><span data-stu-id="2fafa-162">**Note:** Groups created using the Microsoft Azure portal always have **securityEnabled** initially set to `true`.</span></span>

<span data-ttu-id="2fafa-163">**グループ** リソースは[拡張機能](/graph/extensibility-overview)をサポートしているため、`POST` 操作を使用して、リソースの作成時にカスタム プロパティを独自のデータとともにグループに追加することができます。</span><span class="sxs-lookup"><span data-stu-id="2fafa-163">Since the **group** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the group while creating it.</span></span>

><span data-ttu-id="2fafa-164">**注:** ユーザー コンテキストを使用せず、所有者を指定せずにプログラムで Office 365 グループを作成すると、そのグループは匿名で作成されます。</span><span class="sxs-lookup"><span data-stu-id="2fafa-164">**Note:** Creating an Office 365 Group programmatically without a user context and  without specifying owners will create the group anonymously.</span></span>  <span data-ttu-id="2fafa-165">この操作を行うと、さらに手動操作が行われるまで、関連付けられている SharePoint Online サイトが自動的に作成されない可能性があります。</span><span class="sxs-lookup"><span data-stu-id="2fafa-165">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  

<span data-ttu-id="2fafa-166">グループの必要に応じて他の書き込み可能なプロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="2fafa-166">Specify other writable properties as necessary for your group.</span></span> <span data-ttu-id="2fafa-167">詳細については、[group](../resources/group.md) リソースのプロパティをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="2fafa-167">For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

### <a name="grouptypes-options"></a><span data-ttu-id="2fafa-168">groupTypes オプション</span><span class="sxs-lookup"><span data-stu-id="2fafa-168">groupTypes options</span></span>

<span data-ttu-id="2fafa-169">以下に示すように、**groupTypes** プロパティを使用し、グループの種類とグループのメンバーシップを管理します:</span><span class="sxs-lookup"><span data-stu-id="2fafa-169">Use the **groupTypes** property to control the type of group and its membership, as shown below:</span></span>

| <span data-ttu-id="2fafa-170">グループの種類</span><span class="sxs-lookup"><span data-stu-id="2fafa-170">Type of group</span></span> | <span data-ttu-id="2fafa-171">割り当て済みのメンバーシップ</span><span class="sxs-lookup"><span data-stu-id="2fafa-171">Assigned membership</span></span> | <span data-ttu-id="2fafa-172">動的メンバーシップ</span><span class="sxs-lookup"><span data-stu-id="2fafa-172">Dynamic membership</span></span> |
|:--------------|:------------------------|:---------------|
| <span data-ttu-id="2fafa-173">Office 365 (統合グループともいいます)</span><span class="sxs-lookup"><span data-stu-id="2fafa-173">Office 365 (aka unified group)</span></span>| `["Unified"]` | `["Unified","DynamicMembership"]`
| <span data-ttu-id="2fafa-174">Dynamic</span><span class="sxs-lookup"><span data-stu-id="2fafa-174">Dynamic</span></span> | <span data-ttu-id="2fafa-175">`[]` (_null_)</span><span class="sxs-lookup"><span data-stu-id="2fafa-175">Null</span></span> | `["DynamicMembership"]`|

## <a name="response"></a><span data-ttu-id="2fafa-176">応答</span><span class="sxs-lookup"><span data-stu-id="2fafa-176">Response</span></span>

<span data-ttu-id="2fafa-177">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [group](../resources/group.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2fafa-177">If successful, this method returns `201 Created` response code and [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="2fafa-178">応答には、そのグループの既定のプロパティのみが含まれます。</span><span class="sxs-lookup"><span data-stu-id="2fafa-178">The response includes only the default properties of the group.</span></span>

## <a name="examples"></a><span data-ttu-id="2fafa-179">例</span><span class="sxs-lookup"><span data-stu-id="2fafa-179">Examples</span></span>

### <a name="example-1-create-an-office-365-group"></a><span data-ttu-id="2fafa-180">例 1: Office 365 グループを作成する</span><span class="sxs-lookup"><span data-stu-id="2fafa-180">Create an Office 365 group</span></span>

<span data-ttu-id="2fafa-181">次の例では、Office 365 グループを作成しています。</span><span class="sxs-lookup"><span data-stu-id="2fafa-181">The first example request creates an Office 365 Group.</span></span>

#### <a name="request"></a><span data-ttu-id="2fafa-182">要求</span><span class="sxs-lookup"><span data-stu-id="2fafa-182">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_group"
}-->
``` http
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

#### <a name="response"></a><span data-ttu-id="2fafa-183">応答</span><span class="sxs-lookup"><span data-stu-id="2fafa-183">Response</span></span>

<span data-ttu-id="2fafa-184">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2fafa-184">The following is an example of the response.</span></span>

><span data-ttu-id="2fafa-185">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="2fafa-185">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="2fafa-186">実際の呼び出しからは、すべての既定のプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="2fafa-186">All the default properties are returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="2fafa-187">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="2fafa-187">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="2fafa-188">C#</span><span class="sxs-lookup"><span data-stu-id="2fafa-188">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2fafa-189">Javascript</span><span class="sxs-lookup"><span data-stu-id="2fafa-189">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_group-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="example-2-create-an-office-365-group-with-an-owner-and-members"></a><span data-ttu-id="2fafa-190">例 2: 所有者とメンバーを使用して Office 365 グループを作成する</span><span class="sxs-lookup"><span data-stu-id="2fafa-190">Example 2: Create an Office 365 group with an owner and members</span></span>

<span data-ttu-id="2fafa-191">次の例では、所有者とメンバーを指定して Office 365 グループを作成しています。</span><span class="sxs-lookup"><span data-stu-id="2fafa-191">The second example request creates an Office 365 group with an owner and members specified.</span></span>

#### <a name="request"></a><span data-ttu-id="2fafa-192">要求</span><span class="sxs-lookup"><span data-stu-id="2fafa-192">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_prepopulated_group"
}-->
``` http
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

#### <a name="response"></a><span data-ttu-id="2fafa-193">応答</span><span class="sxs-lookup"><span data-stu-id="2fafa-193">Response</span></span> 

<span data-ttu-id="2fafa-194">成功応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2fafa-194">The following is an example of a successful response.</span></span> <span data-ttu-id="2fafa-195">既定のプロパティのみが含まれています。</span><span class="sxs-lookup"><span data-stu-id="2fafa-195">It includes only default properties.</span></span> <span data-ttu-id="2fafa-196">その後は、グループの **owners** ナビゲーション プロパティまたは **members** ナビゲーション プロパティを取得して所有者またはメンバーの詳細を確認できます。</span><span class="sxs-lookup"><span data-stu-id="2fafa-196">You can subsequently get the **owners** or **members** navigation properties of the group to verify the owner or members.</span></span> 

><span data-ttu-id="2fafa-197">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="2fafa-197">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="2fafa-198">実際の呼び出しからは、すべての既定のプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="2fafa-198">All the default properties are returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="2fafa-199">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="2fafa-199">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="2fafa-200">C#</span><span class="sxs-lookup"><span data-stu-id="2fafa-200">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_prepopulated_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2fafa-201">Javascript</span><span class="sxs-lookup"><span data-stu-id="2fafa-201">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_prepopulated_group-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="2fafa-202">関連項目</span><span class="sxs-lookup"><span data-stu-id="2fafa-202">See also</span></span>

- [<span data-ttu-id="2fafa-203">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="2fafa-203">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="2fafa-204">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="2fafa-204">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="2fafa-205">スキーマ拡張機能を使用したグループへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="2fafa-205">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-post-groups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-post-groups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/group-post-groups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-post-groups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
