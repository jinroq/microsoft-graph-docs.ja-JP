---
title: グループを作成する
description: 新しい Office 365 グループまたはセキュリティ グループを作成してください。
author: dkershaw10
localization_priority: Priority
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 0f0bbd5d242936e01c61a13f7e81ff46bf6270e8
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36323263"
---
# <a name="create-group"></a><span data-ttu-id="60ec8-103">グループを作成する</span><span class="sxs-lookup"><span data-stu-id="60ec8-103">Create group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60ec8-104">要求本文で指定した新しい[グループ](../resources/group.md)を作成します。</span><span class="sxs-lookup"><span data-stu-id="60ec8-104">Use this API to create a new [group](../resources/group.md) as specified in the request body.</span></span> <span data-ttu-id="60ec8-105">以下のいずれかのグループを作成できます:</span><span class="sxs-lookup"><span data-stu-id="60ec8-105">You can create one of the following groups:</span></span>

* <span data-ttu-id="60ec8-106">Office 365 グループ (統合グループ)</span><span class="sxs-lookup"><span data-stu-id="60ec8-106">Office 365 Group (unified group)</span></span>
* <span data-ttu-id="60ec8-107">セキュリティ グループ</span><span class="sxs-lookup"><span data-stu-id="60ec8-107">Security group</span></span>

<span data-ttu-id="60ec8-108">この操作は既定で各グループのプロパティのサブセットのみを返します。</span><span class="sxs-lookup"><span data-stu-id="60ec8-108">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="60ec8-109">これらの既定のプロパティは、「[プロパティ](../resources/group.md#properties)」セクションに記載されています。</span><span class="sxs-lookup"><span data-stu-id="60ec8-109">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span> <span data-ttu-id="60ec8-110">既定で_返されない_プロパティを取得するには、[GET 操作](group-get.md)を実行し、`$select` OData クエリ オプションでプロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="60ec8-110">To get properties that are _not_ returned by default, do a GET operation and specify the properties in a `$select` OData query option.</span></span>

><span data-ttu-id="60ec8-111">**注:** [チーム](../resources/team.md)を作成するには、まずグループを作成し、それからそのグループにチームを追加します。[チームの作成](../api/team-put-teams.md)に関するページを参照してください。</span><span class="sxs-lookup"><span data-stu-id="60ec8-111">**Note**: To create a [team](../resources/team.md), first create a group then add a team to it, see [create team](../api/team-put-teams.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="60ec8-112">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="60ec8-112">Permissions</span></span>
<span data-ttu-id="60ec8-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="60ec8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60ec8-115">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="60ec8-115">Permission type</span></span>      | <span data-ttu-id="60ec8-116">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="60ec8-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="60ec8-117">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="60ec8-117">Delegated (work or school account)</span></span> | <span data-ttu-id="60ec8-118">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="60ec8-118">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="60ec8-119">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="60ec8-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60ec8-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="60ec8-120">Not supported.</span></span>    |
|<span data-ttu-id="60ec8-121">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="60ec8-121">Application</span></span> | <span data-ttu-id="60ec8-122">Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60ec8-122">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="60ec8-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="60ec8-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="60ec8-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="60ec8-124">Request headers</span></span>

| <span data-ttu-id="60ec8-125">名前</span><span class="sxs-lookup"><span data-stu-id="60ec8-125">Name</span></span>       | <span data-ttu-id="60ec8-126">種類</span><span class="sxs-lookup"><span data-stu-id="60ec8-126">Type</span></span> | <span data-ttu-id="60ec8-127">説明</span><span class="sxs-lookup"><span data-stu-id="60ec8-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="60ec8-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="60ec8-128">Authorization</span></span>  | <span data-ttu-id="60ec8-129">string</span><span class="sxs-lookup"><span data-stu-id="60ec8-129">string</span></span>  | <span data-ttu-id="60ec8-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="60ec8-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="60ec8-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="60ec8-132">Request body</span></span>

<span data-ttu-id="60ec8-133">次の表は、グループを作成するときに指定する [group](../resources/group.md) リソースのプロパティを示しています。</span><span class="sxs-lookup"><span data-stu-id="60ec8-133">The following table shows the properties of the [group](../resources/group.md) resource to specify when you create a group.</span></span> 

| <span data-ttu-id="60ec8-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="60ec8-134">Property</span></span> | <span data-ttu-id="60ec8-135">型</span><span class="sxs-lookup"><span data-stu-id="60ec8-135">Type</span></span> | <span data-ttu-id="60ec8-136">説明</span><span class="sxs-lookup"><span data-stu-id="60ec8-136">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="60ec8-137">displayName</span><span class="sxs-lookup"><span data-stu-id="60ec8-137">displayName</span></span> | <span data-ttu-id="60ec8-138">string</span><span class="sxs-lookup"><span data-stu-id="60ec8-138">string</span></span> | <span data-ttu-id="60ec8-139">アドレス帳に表示するグループの名前。</span><span class="sxs-lookup"><span data-stu-id="60ec8-139">The name to display in the address book for the group.</span></span> <span data-ttu-id="60ec8-140">必須です。</span><span class="sxs-lookup"><span data-stu-id="60ec8-140">Required.</span></span> |
| <span data-ttu-id="60ec8-141">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="60ec8-141">mailEnabled</span></span> | <span data-ttu-id="60ec8-142">boolean</span><span class="sxs-lookup"><span data-stu-id="60ec8-142">boolean</span></span> | <span data-ttu-id="60ec8-143">メールが有効なグループの場合は、**true** に設定します。</span><span class="sxs-lookup"><span data-stu-id="60ec8-143">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="60ec8-144">必須。</span><span class="sxs-lookup"><span data-stu-id="60ec8-144">Required.</span></span> |
| <span data-ttu-id="60ec8-145">mailNickname</span><span class="sxs-lookup"><span data-stu-id="60ec8-145">mailNickname</span></span> | <span data-ttu-id="60ec8-146">string</span><span class="sxs-lookup"><span data-stu-id="60ec8-146">string</span></span> | <span data-ttu-id="60ec8-147">グループのメール エイリアス。</span><span class="sxs-lookup"><span data-stu-id="60ec8-147">The mail alias for the group.</span></span> <span data-ttu-id="60ec8-148">必須です。</span><span class="sxs-lookup"><span data-stu-id="60ec8-148">Required.</span></span> |
| <span data-ttu-id="60ec8-149">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="60ec8-149">securityEnabled</span></span> | <span data-ttu-id="60ec8-150">ブール値</span><span class="sxs-lookup"><span data-stu-id="60ec8-150">boolean</span></span> | <span data-ttu-id="60ec8-151">Office 365 グループを含む、セキュリティが有効なグループに **true** を設定します。</span><span class="sxs-lookup"><span data-stu-id="60ec8-151">Set to **true** for security-enabled groups, including Office 365 groups.</span></span> <span data-ttu-id="60ec8-152">必須。</span><span class="sxs-lookup"><span data-stu-id="60ec8-152">Required.</span></span> |
| <span data-ttu-id="60ec8-153">owners</span><span class="sxs-lookup"><span data-stu-id="60ec8-153">owners</span></span> | <span data-ttu-id="60ec8-154">[directoryObject](../resources/directoryobject.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="60ec8-154">[directoryObject](../resources/directoryobject.md) collection</span></span> | <span data-ttu-id="60ec8-155">このプロパティは、作成時のグループの所有者を表します。</span><span class="sxs-lookup"><span data-stu-id="60ec8-155">This property represents the owners for the group at creation time.</span></span> <span data-ttu-id="60ec8-156">省略可能。</span><span class="sxs-lookup"><span data-stu-id="60ec8-156">Optional.</span></span> |
| <span data-ttu-id="60ec8-157">members</span><span class="sxs-lookup"><span data-stu-id="60ec8-157">members</span></span> | <span data-ttu-id="60ec8-158">[directoryObject](../resources/directoryobject.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="60ec8-158">[directoryObject](../resources/directoryobject.md) collection</span></span> | <span data-ttu-id="60ec8-159">このプロパティは、作成時のグループのメンバーを表します。</span><span class="sxs-lookup"><span data-stu-id="60ec8-159">This property represents the members for the group at creation time.</span></span> <span data-ttu-id="60ec8-160">省略可能。</span><span class="sxs-lookup"><span data-stu-id="60ec8-160">Optional.</span></span> |

> <span data-ttu-id="60ec8-161">**注**: Microsoft Azure portal を使用して作成されるグループでは、**securityEnabled** は最初は常に `true` に設定されます。</span><span class="sxs-lookup"><span data-stu-id="60ec8-161">**Note:** Groups created using the Microsoft Azure portal always have **securityEnabled** initially set to `true`.</span></span>

<span data-ttu-id="60ec8-162">**グループ** リソースは[拡張機能](/graph/extensibility-overview)をサポートしているため、`POST` 操作を使用して、リソースの作成時にカスタム プロパティを独自のデータとともにグループに追加することができます。</span><span class="sxs-lookup"><span data-stu-id="60ec8-162">Since the **group** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the group while creating it.</span></span>

><span data-ttu-id="60ec8-163">**注:** アプリ専用コンテキストを使用し、所有者を指定せずにプログラムで Office 365 グループを作成すると、そのグループは匿名で作成されます。</span><span class="sxs-lookup"><span data-stu-id="60ec8-163">**Note:** Creating an Office 365 Group programmatically without a user context and  without specifying owners will create the group anonymously.</span></span> <span data-ttu-id="60ec8-164">この操作を行うと、さらに手動操作が行われるまで、関連付けられている SharePoint Online サイトが自動的に作成されない可能性があります。</span><span class="sxs-lookup"><span data-stu-id="60ec8-164">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  

<span data-ttu-id="60ec8-165">グループの必要に応じて他の書き込み可能なプロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="60ec8-165">Specify other writable properties as necessary for your group.</span></span> <span data-ttu-id="60ec8-166">詳細については、[group](../resources/group.md) リソースのプロパティをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="60ec8-166">For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

### <a name="grouptypes-options"></a><span data-ttu-id="60ec8-167">groupTypes オプション</span><span class="sxs-lookup"><span data-stu-id="60ec8-167">groupTypes options</span></span>

<span data-ttu-id="60ec8-168">示すように、**groupTypes** プロパティを使用し、グループの種類とグループのメンバーシップを管理します:</span><span class="sxs-lookup"><span data-stu-id="60ec8-168">Use the **groupTypes** property to control the type of group and its membership, as shown.</span></span>

| <span data-ttu-id="60ec8-169">グループの種類</span><span class="sxs-lookup"><span data-stu-id="60ec8-169">Type of group</span></span> | <span data-ttu-id="60ec8-170">割り当て済みのメンバーシップ</span><span class="sxs-lookup"><span data-stu-id="60ec8-170">Assigned membership</span></span> | <span data-ttu-id="60ec8-171">動的メンバーシップ</span><span class="sxs-lookup"><span data-stu-id="60ec8-171">Dynamic membership</span></span> |
|:--------------|:------------------------|:---------------|
| <span data-ttu-id="60ec8-172">Office 365 (統合グループともいいます)</span><span class="sxs-lookup"><span data-stu-id="60ec8-172">Office 365 (aka unified group)</span></span>| `["Unified"]` | `["Unified","DynamicMembership"]`
| <span data-ttu-id="60ec8-173">Dynamic</span><span class="sxs-lookup"><span data-stu-id="60ec8-173">Dynamic</span></span> | <span data-ttu-id="60ec8-174">`[]` (_null_)</span><span class="sxs-lookup"><span data-stu-id="60ec8-174">Null</span></span> | `["DynamicMembership"]`|

## <a name="response"></a><span data-ttu-id="60ec8-175">応答</span><span class="sxs-lookup"><span data-stu-id="60ec8-175">Response</span></span>

<span data-ttu-id="60ec8-176">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [group](../resources/group.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="60ec8-176">If successful, this method returns a `201 Created` response code and a [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="60ec8-177">応答には、そのグループの既定のプロパティのみが含まれます。</span><span class="sxs-lookup"><span data-stu-id="60ec8-177">The response includes only the default properties of the group.</span></span>

## <a name="examples"></a><span data-ttu-id="60ec8-178">例</span><span class="sxs-lookup"><span data-stu-id="60ec8-178">Examples</span></span>

### <a name="example-1-create-an-office-365-group"></a><span data-ttu-id="60ec8-179">例 1: Office 365 グループを作成する</span><span class="sxs-lookup"><span data-stu-id="60ec8-179">Create an Office 365 group</span></span>

<span data-ttu-id="60ec8-180">次の例では、Office 365 グループを作成します。</span><span class="sxs-lookup"><span data-stu-id="60ec8-180">The following example creates an Office 365 group.</span></span>

#### <a name="request"></a><span data-ttu-id="60ec8-181">要求</span><span class="sxs-lookup"><span data-stu-id="60ec8-181">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="60ec8-182">HTTP</span><span class="sxs-lookup"><span data-stu-id="60ec8-182">--Http</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="60ec8-183">C#</span><span class="sxs-lookup"><span data-stu-id="60ec8-183">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="60ec8-184">JavaScript</span><span class="sxs-lookup"><span data-stu-id="60ec8-184">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="60ec8-185">Objective-C</span><span class="sxs-lookup"><span data-stu-id="60ec8-185">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="60ec8-186">Java</span><span class="sxs-lookup"><span data-stu-id="60ec8-186">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="60ec8-187">応答</span><span class="sxs-lookup"><span data-stu-id="60ec8-187">Response</span></span>

<span data-ttu-id="60ec8-188">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="60ec8-188">The following is an example of the response.</span></span>

><span data-ttu-id="60ec8-189">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="60ec8-189">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="60ec8-190">実際の呼び出しからは、すべての既定のプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="60ec8-190">All the default properties are returned from an actual call.</span></span>

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

### <a name="example-2-create-an-office-365-group-with-an-owner-and-members"></a><span data-ttu-id="60ec8-191">例 2: 所有者とメンバーを指定して Office 365 グループを作成する</span><span class="sxs-lookup"><span data-stu-id="60ec8-191">Example 2: Create an Office 365 group with an owner and members</span></span>

<span data-ttu-id="60ec8-192">次の例では、所有者とメンバーを指定して Office 365 グループを作成しています。</span><span class="sxs-lookup"><span data-stu-id="60ec8-192">The second example request creates an Office 365 group with an owner and members specified.</span></span>

#### <a name="request"></a><span data-ttu-id="60ec8-193">要求</span><span class="sxs-lookup"><span data-stu-id="60ec8-193">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="60ec8-194">HTTP</span><span class="sxs-lookup"><span data-stu-id="60ec8-194">--Http</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="60ec8-195">C#</span><span class="sxs-lookup"><span data-stu-id="60ec8-195">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-prepopulated-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="60ec8-196">JavaScript</span><span class="sxs-lookup"><span data-stu-id="60ec8-196">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-prepopulated-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="60ec8-197">Objective-C</span><span class="sxs-lookup"><span data-stu-id="60ec8-197">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-prepopulated-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="60ec8-198">Java</span><span class="sxs-lookup"><span data-stu-id="60ec8-198">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-prepopulated-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="60ec8-199">応答</span><span class="sxs-lookup"><span data-stu-id="60ec8-199">Response</span></span> 

<span data-ttu-id="60ec8-200">成功応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="60ec8-200">The following is an example of a successful response.</span></span> <span data-ttu-id="60ec8-201">既定のプロパティのみが含まれています。</span><span class="sxs-lookup"><span data-stu-id="60ec8-201">It includes only default properties.</span></span> <span data-ttu-id="60ec8-202">その後は、グループの **owners** ナビゲーション プロパティまたは **members** ナビゲーション プロパティを取得して所有者またはメンバーの詳細を確認できます。</span><span class="sxs-lookup"><span data-stu-id="60ec8-202">You can subsequently get the **owners** or **members** navigation properties of the group to verify the owner or members.</span></span> 

><span data-ttu-id="60ec8-203">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="60ec8-203">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="60ec8-204">実際の呼び出しからは、すべての既定のプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="60ec8-204">All the default properties are returned from an actual call.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="60ec8-205">関連項目</span><span class="sxs-lookup"><span data-stu-id="60ec8-205">See also</span></span>

- [<span data-ttu-id="60ec8-206">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="60ec8-206">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="60ec8-207">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="60ec8-207">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="60ec8-208">スキーマ拡張機能を使用したグループへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="60ec8-208">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


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
  ]
}
-->
