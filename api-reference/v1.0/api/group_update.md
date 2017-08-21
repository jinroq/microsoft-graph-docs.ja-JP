# <a name="update-group"></a><span data-ttu-id="66ed5-101">グループを更新する</span><span class="sxs-lookup"><span data-stu-id="66ed5-101">Update group</span></span>

<span data-ttu-id="66ed5-102">グループ オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="66ed5-102">Update the properties of a group object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="66ed5-103">前提条件</span><span class="sxs-lookup"><span data-stu-id="66ed5-103">Prerequisites</span></span>
<span data-ttu-id="66ed5-104">この API を実行するには、以下の**スコープ**が必要です。*Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="66ed5-104">The following **scope** is required to execute this API: *Group.ReadWrite.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="66ed5-105">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="66ed5-105">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="66ed5-106">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="66ed5-106">Request headers</span></span>

| <span data-ttu-id="66ed5-107">名前</span><span class="sxs-lookup"><span data-stu-id="66ed5-107">Name</span></span>       | <span data-ttu-id="66ed5-108">型</span><span class="sxs-lookup"><span data-stu-id="66ed5-108">Type</span></span> | <span data-ttu-id="66ed5-109">説明</span><span class="sxs-lookup"><span data-stu-id="66ed5-109">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="66ed5-110">Authorization</span><span class="sxs-lookup"><span data-stu-id="66ed5-110">Authorization</span></span>  | <span data-ttu-id="66ed5-111">string</span><span class="sxs-lookup"><span data-stu-id="66ed5-111">string</span></span>  | <span data-ttu-id="66ed5-p101">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="66ed5-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="66ed5-114">要求本文</span><span class="sxs-lookup"><span data-stu-id="66ed5-114">Request body</span></span>

<span data-ttu-id="66ed5-p102">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="66ed5-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="66ed5-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="66ed5-118">Property</span></span>     | <span data-ttu-id="66ed5-119">型</span><span class="sxs-lookup"><span data-stu-id="66ed5-119">Type</span></span>   |<span data-ttu-id="66ed5-120">説明</span><span class="sxs-lookup"><span data-stu-id="66ed5-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="66ed5-121">autoSubscribeNewMembers</span><span class="sxs-lookup"><span data-stu-id="66ed5-121">autoSubscribeNewMembers</span></span>|<span data-ttu-id="66ed5-122">ブール値</span><span class="sxs-lookup"><span data-stu-id="66ed5-122">Boolean</span></span>|<span data-ttu-id="66ed5-p103">既定値は **false** です。グループに追加された新しいメンバーが、電子メールの通知を受信するように自動的にサブスクライブされるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="66ed5-p103">Default is **false**. Indicates if new members added to the group will be auto-subscribed to receive email notifications.</span></span>|
|<span data-ttu-id="66ed5-125">description</span><span class="sxs-lookup"><span data-stu-id="66ed5-125">description</span></span>|<span data-ttu-id="66ed5-126">String</span><span class="sxs-lookup"><span data-stu-id="66ed5-126">String</span></span>|<span data-ttu-id="66ed5-127">グループに関するオプションの説明。</span><span class="sxs-lookup"><span data-stu-id="66ed5-127">An optional description for the group.</span></span> |
|<span data-ttu-id="66ed5-128">displayName</span><span class="sxs-lookup"><span data-stu-id="66ed5-128">displayName</span></span>|<span data-ttu-id="66ed5-129">String</span><span class="sxs-lookup"><span data-stu-id="66ed5-129">String</span></span>|<span data-ttu-id="66ed5-p104">グループの表示名。このプロパティは、グループの作成時の必須プロパティであり、更新時にクリアすることはできません。$filter および $orderby をサポートします。</span><span class="sxs-lookup"><span data-stu-id="66ed5-p104">The display name for the group. This property is required when a group is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="66ed5-133">groupTypes</span><span class="sxs-lookup"><span data-stu-id="66ed5-133">groupTypes</span></span>|<span data-ttu-id="66ed5-134">String collection</span><span class="sxs-lookup"><span data-stu-id="66ed5-134">String collection</span></span>|<span data-ttu-id="66ed5-p105">作成するグループの種類を指定します。使用可能な値は **Unified** (Office 365 のグループを作成する場合) または **DynamicMembership** (動的なグループを作成する場合) です。その他のグループの種類 (セキュリティが有効なグループやメールが有効なセキュリティ グループなど) の場合、このプロパティは設定しないでください。</span><span class="sxs-lookup"><span data-stu-id="66ed5-p105">Specifies the type of group to create. Possible values are **Unified** to create an Office 365 group, or **DynamicMembership** for dynamic groups.  For all other group types, like security-enabled groups and email-enabled security groups, do not set this property.</span></span>|
|<span data-ttu-id="66ed5-138">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="66ed5-138">mailEnabled</span></span>|<span data-ttu-id="66ed5-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="66ed5-139">Boolean</span></span>|<span data-ttu-id="66ed5-p106">メールが有効なグループであるかどうかを指定します。**securityEnabled** プロパティも **true** の場合、グループはメールが有効なセキュリティ グループになります。それ以外の場合は、Microsoft Exchange 配布グループになります。</span><span class="sxs-lookup"><span data-stu-id="66ed5-p106">Specifies whether the group is mail-enabled. If the **securityEnabled** property is also **true**, the group is a mail-enabled security group; otherwise, the group is a Microsoft Exchange distribution group.</span></span>|
|<span data-ttu-id="66ed5-142">mailNickname</span><span class="sxs-lookup"><span data-stu-id="66ed5-142">mailNickname</span></span>|<span data-ttu-id="66ed5-143">String</span><span class="sxs-lookup"><span data-stu-id="66ed5-143">String</span></span>|<span data-ttu-id="66ed5-p107">グループの電子メール エイリアス。このプロパティは、グループの作成時に指定する必要があります。$filter をサポートします。</span><span class="sxs-lookup"><span data-stu-id="66ed5-p107">The mail alias for the group. This property must be specified when a group is created. Supports $filter.</span></span>|
|<span data-ttu-id="66ed5-147">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="66ed5-147">securityEnabled</span></span>|<span data-ttu-id="66ed5-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="66ed5-148">Boolean</span></span>|<span data-ttu-id="66ed5-p108">グループがセキュリティ グループであるかどうかを指定します。**mailEnabled** プロパティも true の場合、グループはメールが有効なセキュリティ グループになります。それ以外の場合は、セキュリティ グループになります。Office 365 グループの場合、**false** にする必要があります。$filter をサポートします。</span><span class="sxs-lookup"><span data-stu-id="66ed5-p108">Specifies whether the group is a security group. If the **mailEnabled** property is also true, the group is a mail-enabled security group; otherwise it is a security group. Must be **false** for Office 365 groups. Supports $filter..</span></span>|
|<span data-ttu-id="66ed5-153">visibility</span><span class="sxs-lookup"><span data-stu-id="66ed5-153">visibility</span></span>|<span data-ttu-id="66ed5-154">ブール値</span><span class="sxs-lookup"><span data-stu-id="66ed5-154">Boolean</span></span>|<span data-ttu-id="66ed5-p109">Office 365 グループの表示を指定します。使用可能な値は次のとおりです。**Private**、**Public**、または空 (**Public** として解釈されます)。</span><span class="sxs-lookup"><span data-stu-id="66ed5-p109">Specifies the visibility of an Office 365 group. Possible values are: **Private**, **Public**, or empty (which is interpreted as **Public**).</span></span>|

<span data-ttu-id="66ed5-157">**メモ**</span><span class="sxs-lookup"><span data-stu-id="66ed5-157">**Note**</span></span>

- <span data-ttu-id="66ed5-158">**autoSubscribeNewMembers** は、独自の PATCH 要求で指定することによって更新できます。上の表にある他のプロパティは含めません。</span><span class="sxs-lookup"><span data-stu-id="66ed5-158">You can update **autoSubscribeNewMembers** by specifying it in its own PATCH request, without including the other properties in the table above.</span></span>
- <span data-ttu-id="66ed5-p110">コア グループの管理とマネージメントに関するグループ API のサブセットのみが、アプリケーションのアクセス許可と委任されたアクセス許可をサポートします。**autoSubscribeNewMembers** の更新を含む他のすべてのグループ API のメンバーは、委任されたアクセス許可のみをサポートします。例については、「[既知の問題](https://developer.microsoft.com/en-us/graph/docs/overview/release_notes#group-permission-scopes)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="66ed5-p110">Only a subset of the group API pertaining to core group administration and management support application and delegated permissions. All other members of the group API, including updating  **autoSubscribeNewMembers**, support only delegated permissions. See [known issues](https://developer.microsoft.com/en-us/graph/docs/overview/release_notes#group-permission-scopes) for examples.</span></span>

## <a name="response"></a><span data-ttu-id="66ed5-162">応答</span><span class="sxs-lookup"><span data-stu-id="66ed5-162">Response</span></span>

<span data-ttu-id="66ed5-163">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="66ed5-163">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="66ed5-164">例</span><span class="sxs-lookup"><span data-stu-id="66ed5-164">Example</span></span>

##### <a name="request"></a><span data-ttu-id="66ed5-165">要求</span><span class="sxs-lookup"><span data-stu-id="66ed5-165">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_group"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groups/{id}
Content-type: application/json
Content-length: 211

{
  "description": "description-value",
  "displayName": "displayName-value",
  "groupTypes": [
    "groupTypes-value"
  ],
  "mail": "mail-value",
  "mailEnabled": true,
  "mailNickname": "mailNickname-value"
}
```

##### <a name="response"></a><span data-ttu-id="66ed5-166">応答</span><span class="sxs-lookup"><span data-stu-id="66ed5-166">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->