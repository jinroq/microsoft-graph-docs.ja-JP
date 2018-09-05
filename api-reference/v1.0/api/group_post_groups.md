# <a name="create-group"></a><span data-ttu-id="d42a0-101">グループを作成する</span><span class="sxs-lookup"><span data-stu-id="d42a0-101">Create group</span></span>
<span data-ttu-id="d42a0-p101">この API を使用して、要求本文で指定した新しいグループを作成します。次に示す 3 種類のグループのうちの 1 つを作成できます。</span><span class="sxs-lookup"><span data-stu-id="d42a0-p101">Use this API to create a new group as specified in the request body. You can create one of three types of groups:</span></span>

* <span data-ttu-id="d42a0-104">Office 365 グループ (統合グループ)</span><span class="sxs-lookup"><span data-stu-id="d42a0-104">Office 365 Group (unified group)</span></span>
* <span data-ttu-id="d42a0-105">動的グループ</span><span class="sxs-lookup"><span data-stu-id="d42a0-105">Dynamic group</span></span>
* <span data-ttu-id="d42a0-106">セキュリティ グループ</span><span class="sxs-lookup"><span data-stu-id="d42a0-106">Security group</span></span>

> <span data-ttu-id="d42a0-p102">**注**:Microsoft Teams は Office 365 グループに基づいていますが、現在、この API を使用してチームを作成することはできません。Microsoft Teams UI で作成されたチームを管理するには、その他のグループ API を使用できます。</span><span class="sxs-lookup"><span data-stu-id="d42a0-p102">**Note**: Although Microsoft Teams is built on Office 365 Groups, you can't currently create a team via this API. You can use the other group APIs to manage a team that has been created in the Microsoft Teams UI.</span></span>

## <a name="permissions"></a><span data-ttu-id="d42a0-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d42a0-109">Permissions</span></span>
<span data-ttu-id="d42a0-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d42a0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d42a0-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d42a0-112">Permission type</span></span>      | <span data-ttu-id="d42a0-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d42a0-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d42a0-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d42a0-114">Delegated (work or school account)</span></span> | <span data-ttu-id="d42a0-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d42a0-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d42a0-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d42a0-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d42a0-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d42a0-117">Not supported.</span></span>    |
|<span data-ttu-id="d42a0-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d42a0-118">Application</span></span> | <span data-ttu-id="d42a0-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d42a0-119">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d42a0-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d42a0-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="d42a0-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d42a0-121">Request headers</span></span>
| <span data-ttu-id="d42a0-122">名前</span><span class="sxs-lookup"><span data-stu-id="d42a0-122">Name</span></span>       | <span data-ttu-id="d42a0-123">型</span><span class="sxs-lookup"><span data-stu-id="d42a0-123">Type</span></span> | <span data-ttu-id="d42a0-124">説明</span><span class="sxs-lookup"><span data-stu-id="d42a0-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d42a0-125">承認</span><span class="sxs-lookup"><span data-stu-id="d42a0-125">Authorization</span></span>  | <span data-ttu-id="d42a0-126">文字列</span><span class="sxs-lookup"><span data-stu-id="d42a0-126">string</span></span>  | <span data-ttu-id="d42a0-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d42a0-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d42a0-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="d42a0-129">Request body</span></span>
<span data-ttu-id="d42a0-130">次の表は、グループ作成時に指定する [group](../resources/group.md) リソースのプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d42a0-130">The following table shows the properties of the [group](../resources/group.md) resource that you must specify at a minimum when you create a group.</span></span> 

| <span data-ttu-id="d42a0-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d42a0-131">Property</span></span> | <span data-ttu-id="d42a0-132">タイプ</span><span class="sxs-lookup"><span data-stu-id="d42a0-132">Type</span></span> | <span data-ttu-id="d42a0-133">説明</span><span class="sxs-lookup"><span data-stu-id="d42a0-133">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d42a0-134">displayName</span><span class="sxs-lookup"><span data-stu-id="d42a0-134">displayName</span></span> | <span data-ttu-id="d42a0-135">文字列</span><span class="sxs-lookup"><span data-stu-id="d42a0-135">string</span></span> | <span data-ttu-id="d42a0-136">アドレス帳に表示するグループの名前。</span><span class="sxs-lookup"><span data-stu-id="d42a0-136">The name to display in the address book for the group.</span></span> <span data-ttu-id="d42a0-137">必須。</span><span class="sxs-lookup"><span data-stu-id="d42a0-137">Required.</span></span> |
| <span data-ttu-id="d42a0-138">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="d42a0-138">mailEnabled</span></span> | <span data-ttu-id="d42a0-139">ブール値</span><span class="sxs-lookup"><span data-stu-id="d42a0-139">boolean</span></span> | <span data-ttu-id="d42a0-140">メールが有効なグループの場合は、**true** に設定します。</span><span class="sxs-lookup"><span data-stu-id="d42a0-140">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="d42a0-141">Office 365 グループを作成する場合は、**true** に設定します。</span><span class="sxs-lookup"><span data-stu-id="d42a0-141">Set this to **true** if creating an Office 365 Group.</span></span> <span data-ttu-id="d42a0-142">動的グループまたはセキュリティ グループを作成する場合は、**false** に設定します。</span><span class="sxs-lookup"><span data-stu-id="d42a0-142">Set this to **false** if creating dynamic or security group.</span></span> <span data-ttu-id="d42a0-143">必須。</span><span class="sxs-lookup"><span data-stu-id="d42a0-143">Required.</span></span> |
| <span data-ttu-id="d42a0-144">mailNickname</span><span class="sxs-lookup"><span data-stu-id="d42a0-144">mailNickname</span></span> | <span data-ttu-id="d42a0-145">文字列</span><span class="sxs-lookup"><span data-stu-id="d42a0-145">string</span></span> | <span data-ttu-id="d42a0-146">グループの電子メール エイリアス。</span><span class="sxs-lookup"><span data-stu-id="d42a0-146">The mail alias for the group.</span></span> <span data-ttu-id="d42a0-147">必須。</span><span class="sxs-lookup"><span data-stu-id="d42a0-147">Required.</span></span> |
| <span data-ttu-id="d42a0-148">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="d42a0-148">securityEnabled</span></span> | <span data-ttu-id="d42a0-149">ブール値</span><span class="sxs-lookup"><span data-stu-id="d42a0-149">boolean</span></span> | <span data-ttu-id="d42a0-150">セキュリティが有効なグループの場合は、**  true** を設定します。</span><span class="sxs-lookup"><span data-stu-id="d42a0-150">Set to **true** for security-enabled groups.</span></span> <span data-ttu-id="d42a0-151">動的グループまたはセキュリティ グループを作成する場合は、**true** に設定します。</span><span class="sxs-lookup"><span data-stu-id="d42a0-151">Set this to **true** if creating a dynamic or security group.</span></span> <span data-ttu-id="d42a0-152">Office 365 グループを作成する場合は、**true** に設定します。</span><span class="sxs-lookup"><span data-stu-id="d42a0-152">Set this to **false** if creating an Office 365 group.</span></span> <span data-ttu-id="d42a0-153">必須。</span><span class="sxs-lookup"><span data-stu-id="d42a0-153">Required.</span></span> |
| <span data-ttu-id="d42a0-154">owners</span><span class="sxs-lookup"><span data-stu-id="d42a0-154">owners</span></span> | <span data-ttu-id="d42a0-155">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="d42a0-155">string collection</span></span> | <span data-ttu-id="d42a0-156">このプロパティは、作成時のグループの所有者を表します。</span><span class="sxs-lookup"><span data-stu-id="d42a0-156">This property represents the owners for the group at creation time.</span></span> <span data-ttu-id="d42a0-157">省略可能。</span><span class="sxs-lookup"><span data-stu-id="d42a0-157">Optional.</span></span> |
| <span data-ttu-id="d42a0-158">メンバー</span><span class="sxs-lookup"><span data-stu-id="d42a0-158">members</span></span> | <span data-ttu-id="d42a0-159">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="d42a0-159">string collection</span></span> | <span data-ttu-id="d42a0-160">このプロパティは、作成時のグループのメンバーを表します。</span><span class="sxs-lookup"><span data-stu-id="d42a0-160">This property represents the members for the group at creation time.</span></span> <span data-ttu-id="d42a0-161">省略可能。</span><span class="sxs-lookup"><span data-stu-id="d42a0-161">Optional.</span></span> |


<span data-ttu-id="d42a0-162">Office 365 グループまたは動的グループを作成している場合は、以下のように **groupTypes** プロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="d42a0-162">Specify the **groupTypes** property if you're creating an Office 365 or dynamic group, as stated below.</span></span>

### <a name="grouptypes-options"></a><span data-ttu-id="d42a0-163">groupTypes オプション</span><span class="sxs-lookup"><span data-stu-id="d42a0-163">groupTypes options</span></span>

| <span data-ttu-id="d42a0-164">グループの種類</span><span class="sxs-lookup"><span data-stu-id="d42a0-164">Type of group</span></span> | <span data-ttu-id="d42a0-165">**groupTypes** プロパティ</span><span class="sxs-lookup"><span data-stu-id="d42a0-165">**groupTypes** property</span></span> |
|:--------------|:------------------------|
| <span data-ttu-id="d42a0-166">Office 365 (統合グループともいいます)</span><span class="sxs-lookup"><span data-stu-id="d42a0-166">Office 365 (aka unified group)</span></span>| <span data-ttu-id="d42a0-167">"Unified"</span><span class="sxs-lookup"><span data-stu-id="d42a0-167">"Unified"</span></span> |
| <span data-ttu-id="d42a0-168">動的</span><span class="sxs-lookup"><span data-stu-id="d42a0-168">Dynamic</span></span> | <span data-ttu-id="d42a0-169">"DynamicMembership"</span><span class="sxs-lookup"><span data-stu-id="d42a0-169">"DynamicMembership"</span></span> |
| <span data-ttu-id="d42a0-170">セキュリティ</span><span class="sxs-lookup"><span data-stu-id="d42a0-170">Security</span></span> | <span data-ttu-id="d42a0-171">設定しない。</span><span class="sxs-lookup"><span data-stu-id="d42a0-171">Do not set.</span></span> |


><span data-ttu-id="d42a0-172">**注:** ユーザー コンテキストおよび所有者を指定せずにプログラムで Office 365 グループを作成すると、匿名のグループが作成されます。</span><span class="sxs-lookup"><span data-stu-id="d42a0-172">**Note:** Creating an Office 365 Group programmatically without a user context and  without specifying owners will create the group anonymously.</span></span>  <span data-ttu-id="d42a0-173">これを行うと、関連する SharePoint Online サイトは手動操作が行なわれるまで自動的に作成されなくなります。</span><span class="sxs-lookup"><span data-stu-id="d42a0-173">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  

<span data-ttu-id="d42a0-p112">グループの必要に応じて他の書き込み可能なプロパティを指定します。詳細については、[group](../resources/group.md) リソースのプロパティを参照してください。</span><span class="sxs-lookup"><span data-stu-id="d42a0-p112">Specify other writable properties as necessary for your group. For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

## <a name="response"></a><span data-ttu-id="d42a0-176">応答</span><span class="sxs-lookup"><span data-stu-id="d42a0-176">Response</span></span>
<span data-ttu-id="d42a0-177">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で[グループ](../resources/group.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d42a0-177">If successful, this method returns `201 Created` response code and [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d42a0-178">例</span><span class="sxs-lookup"><span data-stu-id="d42a0-178">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="d42a0-179">要求 1</span><span class="sxs-lookup"><span data-stu-id="d42a0-179">Request 1</span></span>
<span data-ttu-id="d42a0-180">最初の例は、Office 365 グループの作成を要求するものです。</span><span class="sxs-lookup"><span data-stu-id="d42a0-180">The following is an example of a request that creates an Office 365 Group.</span></span>
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

#### <a name="response-1"></a><span data-ttu-id="d42a0-181">応答 1</span><span class="sxs-lookup"><span data-stu-id="d42a0-181">Response 1</span></span>
<span data-ttu-id="d42a0-182">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d42a0-182">The following is an example of the response.</span></span>
><span data-ttu-id="d42a0-p113">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="d42a0-p113">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

#### <a name="request-2"></a><span data-ttu-id="d42a0-185">要求 2</span><span class="sxs-lookup"><span data-stu-id="d42a0-185">Request 2</span></span>
<span data-ttu-id="d42a0-186">2 番目の例は、指定した所有者で Office 365 グループの作成を要求するものです。</span><span class="sxs-lookup"><span data-stu-id="d42a0-186">The second example request creates an Office 365 Group with owners specified.</span></span>
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

#### <a name="response-2"></a><span data-ttu-id="d42a0-187">応答 2</span><span class="sxs-lookup"><span data-stu-id="d42a0-187">Response 2</span></span>
<span data-ttu-id="d42a0-188">成功した応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d42a0-188">The following is an example of the response.</span></span>
><span data-ttu-id="d42a0-p114">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="d42a0-p114">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
