# <a name="create-group"></a><span data-ttu-id="3ca0c-101">グループを作成する</span><span class="sxs-lookup"><span data-stu-id="3ca0c-101">Create group</span></span>

<span data-ttu-id="3ca0c-p101">この API を使用して、要求本文で指定した新しいグループを作成します。次に示す 3 種類のグループのうちの 1 つを作成できます。</span><span class="sxs-lookup"><span data-stu-id="3ca0c-p101">Use this API to create a new group as specified in the request body. You can create one of three types of groups:</span></span>

* <span data-ttu-id="3ca0c-104">Office 365 グループ (統合グループ)</span><span class="sxs-lookup"><span data-stu-id="3ca0c-104">Office 365 group (unified group)</span></span>
* <span data-ttu-id="3ca0c-105">動的グループ</span><span class="sxs-lookup"><span data-stu-id="3ca0c-105">Dynamic group</span></span>
* <span data-ttu-id="3ca0c-106">セキュリティ グループ</span><span class="sxs-lookup"><span data-stu-id="3ca0c-106">Security group</span></span>

> <span data-ttu-id="3ca0c-p102">**注**:Microsoft Teams は Office 365 グループでビルドされますが、この API を使用してチームを作成することは現在できません。Microsoft Teams UI で作成されたチームを管理するには、その他のグループ API を使用できます。</span><span class="sxs-lookup"><span data-stu-id="3ca0c-p102">**Note**: Although Microsoft Teams is built on Office 365 groups, you can't currently create a team via this API. You can use the other group APIs to manage a team that has been created in the Microsoft Teams UI.</span></span>

## <a name="permissions"></a><span data-ttu-id="3ca0c-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3ca0c-109">Permissions</span></span>
<span data-ttu-id="3ca0c-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3ca0c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3ca0c-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3ca0c-112">Permission type</span></span>      | <span data-ttu-id="3ca0c-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3ca0c-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3ca0c-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3ca0c-114">Delegated (work or school account)</span></span> | <span data-ttu-id="3ca0c-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ca0c-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3ca0c-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3ca0c-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ca0c-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3ca0c-117">Not supported.</span></span>    |
|<span data-ttu-id="3ca0c-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3ca0c-118">Application</span></span> | <span data-ttu-id="3ca0c-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ca0c-119">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3ca0c-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3ca0c-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```
## <a name="request-headers"></a><span data-ttu-id="3ca0c-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3ca0c-121">Request headers</span></span>
| <span data-ttu-id="3ca0c-122">名前</span><span class="sxs-lookup"><span data-stu-id="3ca0c-122">Name</span></span>       | <span data-ttu-id="3ca0c-123">型</span><span class="sxs-lookup"><span data-stu-id="3ca0c-123">Type</span></span> | <span data-ttu-id="3ca0c-124">説明</span><span class="sxs-lookup"><span data-stu-id="3ca0c-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3ca0c-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ca0c-125">Authorization</span></span>  | <span data-ttu-id="3ca0c-126">string</span><span class="sxs-lookup"><span data-stu-id="3ca0c-126">string</span></span>  | <span data-ttu-id="3ca0c-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3ca0c-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3ca0c-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="3ca0c-129">Request body</span></span>
<span data-ttu-id="3ca0c-130">次の表は、グループを作成するときに最低限指定する必要のある [group](../resources/group.md) リソースのプロパティを示しています。</span><span class="sxs-lookup"><span data-stu-id="3ca0c-130">The following table shows the properties of the [group](../resources/group.md) resource that you must specify at a minimum when you create a group.</span></span> 

| <span data-ttu-id="3ca0c-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3ca0c-131">Property</span></span> | <span data-ttu-id="3ca0c-132">型</span><span class="sxs-lookup"><span data-stu-id="3ca0c-132">Type</span></span> | <span data-ttu-id="3ca0c-133">説明</span><span class="sxs-lookup"><span data-stu-id="3ca0c-133">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3ca0c-134">displayName</span><span class="sxs-lookup"><span data-stu-id="3ca0c-134">displayName</span></span> | <span data-ttu-id="3ca0c-135">string</span><span class="sxs-lookup"><span data-stu-id="3ca0c-135">string</span></span> | <span data-ttu-id="3ca0c-136">アドレス帳に表示するグループの名前。</span><span class="sxs-lookup"><span data-stu-id="3ca0c-136">The name to display in the address book for the group.</span></span> |
| <span data-ttu-id="3ca0c-137">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="3ca0c-137">mailEnabled</span></span> | <span data-ttu-id="3ca0c-138">boolean</span><span class="sxs-lookup"><span data-stu-id="3ca0c-138">boolean</span></span> | <span data-ttu-id="3ca0c-p105">メールが有効なグループの場合は、**true** に設定します。Office 365 グループを作成する場合は、これを **true** に設定します。動的グループまたはセキュリティ グループを作成する場合は、これを **false** に設定します。</span><span class="sxs-lookup"><span data-stu-id="3ca0c-p105">Set to **true** for mail-enabled groups. Set this to **true** if creating an Office 365 group. Set this to **false** if creating dynamic or security group.</span></span>|
| <span data-ttu-id="3ca0c-142">mailNickname</span><span class="sxs-lookup"><span data-stu-id="3ca0c-142">mailNickname</span></span> | <span data-ttu-id="3ca0c-143">string</span><span class="sxs-lookup"><span data-stu-id="3ca0c-143">string</span></span> | <span data-ttu-id="3ca0c-144">グループの電子メール エイリアス。</span><span class="sxs-lookup"><span data-stu-id="3ca0c-144">The mail alias for the group.</span></span> |
| <span data-ttu-id="3ca0c-145">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="3ca0c-145">securityEnabled</span></span> | <span data-ttu-id="3ca0c-146">boolean</span><span class="sxs-lookup"><span data-stu-id="3ca0c-146">boolean</span></span> | <span data-ttu-id="3ca0c-p106">セキュリティが有効なグループの場合は、**true** に設定します。動的グループまたはセキュリティ グループを作成する場合は、これを **true** に設定します。Office 365 グループを作成する場合は、これを **false** に設定します。</span><span class="sxs-lookup"><span data-stu-id="3ca0c-p106">Set to **true** for security-enabled groups. Set this to **true** if creating a dynamic or security group. Set this to **false** if creating an Office 365 group.</span></span> |

<span data-ttu-id="3ca0c-150">Office 365 グループまたは動的グループを作成している場合は、以下のように **groupTypes** プロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="3ca0c-150">Specify the **groupTypes** property if you're creating an Office 365 or dynamic group, as stated below.</span></span>

| <span data-ttu-id="3ca0c-151">グループの種類</span><span class="sxs-lookup"><span data-stu-id="3ca0c-151">Type of group</span></span> | <span data-ttu-id="3ca0c-152">**groupTypes** プロパティ</span><span class="sxs-lookup"><span data-stu-id="3ca0c-152">**groupTypes** property</span></span> |
|:--------------|:------------------------|
| <span data-ttu-id="3ca0c-153">Office 365 (統合グループともいいます)</span><span class="sxs-lookup"><span data-stu-id="3ca0c-153">Office 365 (aka unified group)</span></span>| <span data-ttu-id="3ca0c-154">"Unified"</span><span class="sxs-lookup"><span data-stu-id="3ca0c-154">"Unified"</span></span> |
| <span data-ttu-id="3ca0c-155">Dynamic</span><span class="sxs-lookup"><span data-stu-id="3ca0c-155">Dynamic</span></span> | <span data-ttu-id="3ca0c-156">"DynamicMembership"</span><span class="sxs-lookup"><span data-stu-id="3ca0c-156">"DynamicMembership"</span></span> |
| <span data-ttu-id="3ca0c-157">Security</span><span class="sxs-lookup"><span data-stu-id="3ca0c-157">Security</span></span> | <span data-ttu-id="3ca0c-158">設定しない。</span><span class="sxs-lookup"><span data-stu-id="3ca0c-158">Do not set.</span></span> |

<span data-ttu-id="3ca0c-p107">グループの必要に応じて他の書き込み可能なプロパティを指定します。詳細については、[group](../resources/group.md) リソースのプロパティをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="3ca0c-p107">Specify other writable properties as necessary for your group. For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

## <a name="response"></a><span data-ttu-id="3ca0c-161">応答</span><span class="sxs-lookup"><span data-stu-id="3ca0c-161">Response</span></span>

<span data-ttu-id="3ca0c-162">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で[グループ](../resources/group.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3ca0c-162">If successful, this method returns `201 Created` response code and [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ca0c-163">例</span><span class="sxs-lookup"><span data-stu-id="3ca0c-163">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3ca0c-164">要求</span><span class="sxs-lookup"><span data-stu-id="3ca0c-164">Request</span></span>
<span data-ttu-id="3ca0c-165">これは、Office 365 グループを作成する要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3ca0c-165">Here is an example of a request that creates an Office 365 group.</span></span>
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

##### <a name="response"></a><span data-ttu-id="3ca0c-166">応答</span><span class="sxs-lookup"><span data-stu-id="3ca0c-166">Response</span></span>
<span data-ttu-id="3ca0c-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。実際の呼び出しでは、さらに多くのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="3ca0c-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. More properties will be returned from an actual call.</span></span>
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
