# <a name="create-group"></a><span data-ttu-id="8ca6f-101">グループを作成する</span><span class="sxs-lookup"><span data-stu-id="8ca6f-101">Create group</span></span>
<span data-ttu-id="8ca6f-p101">この API を使用して、要求本文で指定した新しいグループを作成します。次に示す 3 種類のグループのうちの 1 つを作成できます。</span><span class="sxs-lookup"><span data-stu-id="8ca6f-p101">Use this API to create a new group as specified in the request body. You can create one of three types of groups:</span></span>

* <span data-ttu-id="8ca6f-104">Office 365 グループ (統合グループ)</span><span class="sxs-lookup"><span data-stu-id="8ca6f-104">Office 365 group (unified group)</span></span>
* <span data-ttu-id="8ca6f-105">動的グループ</span><span class="sxs-lookup"><span data-stu-id="8ca6f-105">Dynamic group</span></span>
* <span data-ttu-id="8ca6f-106">セキュリティ グループ</span><span class="sxs-lookup"><span data-stu-id="8ca6f-106">Security group</span></span>

> <span data-ttu-id="8ca6f-p102">**注**:Microsoft Teams は Office 365 グループでビルドされますが、この API を使用してチームを作成することは現在できません。Microsoft Teams UI で作成されたチームを管理するには、その他のグループ API を使用できます。</span><span class="sxs-lookup"><span data-stu-id="8ca6f-p102">**Note**: Although Microsoft Teams is built on Office 365 groups, you can't currently create a team via this API. You can use the other group APIs to manage a team that has been created in the Microsoft Teams UI.</span></span>

## <a name="permissions"></a><span data-ttu-id="8ca6f-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8ca6f-109">Permissions</span></span>
<span data-ttu-id="8ca6f-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8ca6f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8ca6f-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8ca6f-112">Permission type</span></span>      | <span data-ttu-id="8ca6f-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8ca6f-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8ca6f-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8ca6f-114">Delegated (work or school account)</span></span> | <span data-ttu-id="8ca6f-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ca6f-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8ca6f-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8ca6f-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ca6f-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8ca6f-117">Not supported.</span></span>    |
|<span data-ttu-id="8ca6f-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8ca6f-118">Application</span></span> | <span data-ttu-id="8ca6f-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ca6f-119">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8ca6f-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8ca6f-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="8ca6f-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8ca6f-121">Request headers</span></span>
| <span data-ttu-id="8ca6f-122">名前</span><span class="sxs-lookup"><span data-stu-id="8ca6f-122">Name</span></span>       | <span data-ttu-id="8ca6f-123">型</span><span class="sxs-lookup"><span data-stu-id="8ca6f-123">Type</span></span> | <span data-ttu-id="8ca6f-124">説明</span><span class="sxs-lookup"><span data-stu-id="8ca6f-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8ca6f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="8ca6f-125">Authorization</span></span>  | <span data-ttu-id="8ca6f-126">string</span><span class="sxs-lookup"><span data-stu-id="8ca6f-126">string</span></span>  | <span data-ttu-id="8ca6f-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8ca6f-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8ca6f-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="8ca6f-129">Request body</span></span>
<span data-ttu-id="8ca6f-130">次の表は、グループを作成するときに最低限指定する必要のある [group](../resources/group.md) リソースのプロパティを示しています。</span><span class="sxs-lookup"><span data-stu-id="8ca6f-130">The following table shows the properties of the [group](../resources/group.md) resource that you must specify at a minimum when you create a group.</span></span> 

| <span data-ttu-id="8ca6f-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8ca6f-131">Property</span></span> | <span data-ttu-id="8ca6f-132">型</span><span class="sxs-lookup"><span data-stu-id="8ca6f-132">Type</span></span> | <span data-ttu-id="8ca6f-133">説明</span><span class="sxs-lookup"><span data-stu-id="8ca6f-133">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8ca6f-134">displayName</span><span class="sxs-lookup"><span data-stu-id="8ca6f-134">displayName</span></span> | <span data-ttu-id="8ca6f-135">string</span><span class="sxs-lookup"><span data-stu-id="8ca6f-135">string</span></span> | <span data-ttu-id="8ca6f-136">アドレス帳に表示するグループの名前。</span><span class="sxs-lookup"><span data-stu-id="8ca6f-136">The name to display in the address book for the group.</span></span> |
| <span data-ttu-id="8ca6f-137">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="8ca6f-137">mailEnabled</span></span> | <span data-ttu-id="8ca6f-138">boolean</span><span class="sxs-lookup"><span data-stu-id="8ca6f-138">boolean</span></span> | <span data-ttu-id="8ca6f-p105">メールが有効なグループの場合は、**true** に設定します。Office 365 グループを作成する場合は、これを **true** に設定します。動的グループまたはセキュリティ グループを作成する場合は、これを **false** に設定します。</span><span class="sxs-lookup"><span data-stu-id="8ca6f-p105">Set to **true** for mail-enabled groups. Set this to **true** if creating an Office 365 group. Set this to **false** if creating dynamic or security group.</span></span>|
| <span data-ttu-id="8ca6f-142">mailNickname</span><span class="sxs-lookup"><span data-stu-id="8ca6f-142">mailNickname</span></span> | <span data-ttu-id="8ca6f-143">string</span><span class="sxs-lookup"><span data-stu-id="8ca6f-143">string</span></span> | <span data-ttu-id="8ca6f-144">グループの電子メール エイリアス。</span><span class="sxs-lookup"><span data-stu-id="8ca6f-144">The mail alias for the group.</span></span> |
| <span data-ttu-id="8ca6f-145">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="8ca6f-145">securityEnabled</span></span> | <span data-ttu-id="8ca6f-146">boolean</span><span class="sxs-lookup"><span data-stu-id="8ca6f-146">boolean</span></span> | <span data-ttu-id="8ca6f-p106">セキュリティが有効なグループの場合は、**true** に設定します。動的グループまたはセキュリティ グループを作成する場合は、これを **true** に設定します。Office 365 グループを作成する場合は、これを **false** に設定します。</span><span class="sxs-lookup"><span data-stu-id="8ca6f-p106">Set to **true** for security-enabled groups. Set this to **true** if creating a dynamic or security group. Set this to **false** if creating an Office 365 group.</span></span> |

<span data-ttu-id="8ca6f-150">Office 365 グループまたは動的グループを作成している場合は、以下のように **groupTypes** プロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="8ca6f-150">Specify the **groupTypes** property if you're creating an Office 365 or dynamic group, as stated below.</span></span>

| <span data-ttu-id="8ca6f-151">グループの種類</span><span class="sxs-lookup"><span data-stu-id="8ca6f-151">Type of group</span></span> | <span data-ttu-id="8ca6f-152">**groupTypes** プロパティ</span><span class="sxs-lookup"><span data-stu-id="8ca6f-152">**groupTypes** property</span></span> |
|:--------------|:------------------------|
| <span data-ttu-id="8ca6f-153">Office 365 (統合グループともいいます)</span><span class="sxs-lookup"><span data-stu-id="8ca6f-153">Office 365 (aka unified group)</span></span>| <span data-ttu-id="8ca6f-154">"Unified"</span><span class="sxs-lookup"><span data-stu-id="8ca6f-154">"Unified"</span></span> |
| <span data-ttu-id="8ca6f-155">Dynamic</span><span class="sxs-lookup"><span data-stu-id="8ca6f-155">Dynamic</span></span> | <span data-ttu-id="8ca6f-156">"DynamicMembership"</span><span class="sxs-lookup"><span data-stu-id="8ca6f-156">"DynamicMembership"</span></span> |
| <span data-ttu-id="8ca6f-157">Security</span><span class="sxs-lookup"><span data-stu-id="8ca6f-157">Security</span></span> | <span data-ttu-id="8ca6f-158">設定しない。</span><span class="sxs-lookup"><span data-stu-id="8ca6f-158">Do not set.</span></span> |

<span data-ttu-id="8ca6f-p107">グループの必要に応じて他の書き込み可能なプロパティを指定します。詳細については、[group](../resources/group.md) リソースのプロパティをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="8ca6f-p107">Specify other writable properties as necessary for your group. For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

## <a name="response"></a><span data-ttu-id="8ca6f-161">応答</span><span class="sxs-lookup"><span data-stu-id="8ca6f-161">Response</span></span>
<span data-ttu-id="8ca6f-162">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で[グループ](../resources/group.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8ca6f-162">If successful, this method returns `201 Created` response code and [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ca6f-163">例</span><span class="sxs-lookup"><span data-stu-id="8ca6f-163">Example</span></span>
#### <a name="request"></a><span data-ttu-id="8ca6f-164">要求</span><span class="sxs-lookup"><span data-stu-id="8ca6f-164">Request</span></span>
<span data-ttu-id="8ca6f-165">Office 365 グループを作成する要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8ca6f-165">Here is an example of a request that creates an Office 365 group.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_group_from_groups"
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

#### <a name="response"></a><span data-ttu-id="8ca6f-166">応答</span><span class="sxs-lookup"><span data-stu-id="8ca6f-166">Response</span></span>
<span data-ttu-id="8ca6f-167">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8ca6f-167">The following is an example of a response.</span></span>
><span data-ttu-id="8ca6f-168">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="8ca6f-168">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="8ca6f-169">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="8ca6f-169">All the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
