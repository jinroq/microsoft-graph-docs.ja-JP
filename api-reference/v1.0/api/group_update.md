# <a name="update-group"></a><span data-ttu-id="3e88b-101">グループを更新する</span><span class="sxs-lookup"><span data-stu-id="3e88b-101">Update group</span></span>
<span data-ttu-id="3e88b-102">グループ オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="3e88b-102">Update the properties of a group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3e88b-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3e88b-103">Permissions</span></span>
<span data-ttu-id="3e88b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3e88b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3e88b-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3e88b-106">Permission type</span></span>      | <span data-ttu-id="3e88b-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3e88b-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3e88b-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3e88b-108">Delegated (work or school account)</span></span> | <span data-ttu-id="3e88b-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e88b-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3e88b-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3e88b-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e88b-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3e88b-111">Not supported.</span></span>    |
|<span data-ttu-id="3e88b-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3e88b-112">Application</span></span> | <span data-ttu-id="3e88b-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e88b-113">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3e88b-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3e88b-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="3e88b-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3e88b-115">Request headers</span></span>

| <span data-ttu-id="3e88b-116">名前</span><span class="sxs-lookup"><span data-stu-id="3e88b-116">Name</span></span>       | <span data-ttu-id="3e88b-117">型</span><span class="sxs-lookup"><span data-stu-id="3e88b-117">Type</span></span> | <span data-ttu-id="3e88b-118">説明</span><span class="sxs-lookup"><span data-stu-id="3e88b-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3e88b-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e88b-119">Authorization</span></span>  | <span data-ttu-id="3e88b-120">string</span><span class="sxs-lookup"><span data-stu-id="3e88b-120">string</span></span>  | <span data-ttu-id="3e88b-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3e88b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3e88b-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="3e88b-123">Request body</span></span>

<span data-ttu-id="3e88b-p103">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="3e88b-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3e88b-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3e88b-127">Property</span></span>     | <span data-ttu-id="3e88b-128">型</span><span class="sxs-lookup"><span data-stu-id="3e88b-128">Type</span></span>   |<span data-ttu-id="3e88b-129">説明</span><span class="sxs-lookup"><span data-stu-id="3e88b-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3e88b-130">autoSubscribeNewMembers</span><span class="sxs-lookup"><span data-stu-id="3e88b-130">autoSubscribeNewMembers</span></span>|<span data-ttu-id="3e88b-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="3e88b-131">Boolean</span></span>|<span data-ttu-id="3e88b-p104">既定値は **false** です。グループに追加された新しいメンバーが、電子メールの通知を受信するように自動的にサブスクライブされるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="3e88b-p104">Default is **false**. Indicates if new members added to the group will be auto-subscribed to receive email notifications.</span></span>|
|<span data-ttu-id="3e88b-134">description</span><span class="sxs-lookup"><span data-stu-id="3e88b-134">description</span></span>|<span data-ttu-id="3e88b-135">String</span><span class="sxs-lookup"><span data-stu-id="3e88b-135">String</span></span>|<span data-ttu-id="3e88b-136">グループに関するオプションの説明。</span><span class="sxs-lookup"><span data-stu-id="3e88b-136">An optional description for the group.</span></span> |
|<span data-ttu-id="3e88b-137">displayName</span><span class="sxs-lookup"><span data-stu-id="3e88b-137">displayName</span></span>|<span data-ttu-id="3e88b-138">String</span><span class="sxs-lookup"><span data-stu-id="3e88b-138">String</span></span>|<span data-ttu-id="3e88b-p105">グループの表示名。このプロパティは、グループの作成時の必須プロパティであり、更新時にクリアすることはできません。$filter および $orderby をサポートします。</span><span class="sxs-lookup"><span data-stu-id="3e88b-p105">The display name for the group. This property is required when a group is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="3e88b-142">groupTypes</span><span class="sxs-lookup"><span data-stu-id="3e88b-142">groupTypes</span></span>|<span data-ttu-id="3e88b-143">String collection</span><span class="sxs-lookup"><span data-stu-id="3e88b-143">String collection</span></span>|<span data-ttu-id="3e88b-p106">作成するグループの種類を指定します。使用可能な値は **Unified** (Office 365 のグループを作成する場合) または **DynamicMembership** (動的なグループを作成する場合) です。その他のグループの種類 (セキュリティが有効なグループやメールが有効なセキュリティ グループなど) の場合、このプロパティは設定しないでください。</span><span class="sxs-lookup"><span data-stu-id="3e88b-p106">Specifies the type of group to create. Possible values are **Unified** to create an Office 365 group, or **DynamicMembership** for dynamic groups.  For all other group types, like security-enabled groups and email-enabled security groups, do not set this property.</span></span>|
|<span data-ttu-id="3e88b-147">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="3e88b-147">mailEnabled</span></span>|<span data-ttu-id="3e88b-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="3e88b-148">Boolean</span></span>|<span data-ttu-id="3e88b-p107">メールが有効なグループであるかどうかを指定します。**securityEnabled** プロパティも **true** の場合、グループはメールが有効なセキュリティ グループになります。それ以外の場合は、Microsoft Exchange 配布グループになります。</span><span class="sxs-lookup"><span data-stu-id="3e88b-p107">Specifies whether the group is mail-enabled. If the **securityEnabled** property is also **true**, the group is a mail-enabled security group; otherwise, the group is a Microsoft Exchange distribution group.</span></span>|
|<span data-ttu-id="3e88b-151">mailNickname</span><span class="sxs-lookup"><span data-stu-id="3e88b-151">mailNickname</span></span>|<span data-ttu-id="3e88b-152">String</span><span class="sxs-lookup"><span data-stu-id="3e88b-152">String</span></span>|<span data-ttu-id="3e88b-p108">グループの電子メール エイリアス。このプロパティは、グループの作成時に指定する必要があります。$filter をサポートします。</span><span class="sxs-lookup"><span data-stu-id="3e88b-p108">The mail alias for the group. This property must be specified when a group is created. Supports $filter.</span></span>|
|<span data-ttu-id="3e88b-156">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="3e88b-156">securityEnabled</span></span>|<span data-ttu-id="3e88b-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="3e88b-157">Boolean</span></span>|<span data-ttu-id="3e88b-p109">グループがセキュリティ グループであるかどうかを指定します。**mailEnabled** プロパティも true の場合、グループはメールが有効なセキュリティ グループになります。それ以外の場合は、セキュリティ グループになります。Office 365 グループの場合、**false** にする必要があります。$filter をサポートします。</span><span class="sxs-lookup"><span data-stu-id="3e88b-p109">Specifies whether the group is a security group. If the **mailEnabled** property is also true, the group is a mail-enabled security group; otherwise it is a security group. Must be **false** for Office 365 groups. Supports $filter..</span></span>|
|<span data-ttu-id="3e88b-162">visibility</span><span class="sxs-lookup"><span data-stu-id="3e88b-162">visibility</span></span>|<span data-ttu-id="3e88b-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="3e88b-163">Boolean</span></span>|<span data-ttu-id="3e88b-p110">Office 365 グループの表示を指定します。使用可能な値は次のとおりです。**Private**、**Public**、または空 (**Public** として解釈されます)。</span><span class="sxs-lookup"><span data-stu-id="3e88b-p110">Specifies the visibility of an Office 365 group. Possible values are: **Private**, **Public**, or empty (which is interpreted as **Public**).</span></span>|

<span data-ttu-id="3e88b-166">**注**</span><span class="sxs-lookup"><span data-stu-id="3e88b-166">**Note**</span></span>

- <span data-ttu-id="3e88b-167">**autoSubscribeNewMembers** は、独自の PATCH 要求で指定することによって更新できます。上の表にある他のプロパティは含めません。</span><span class="sxs-lookup"><span data-stu-id="3e88b-167">You can update **autoSubscribeNewMembers** by specifying it in its own PATCH request, without including the other properties in the table above.</span></span>
- <span data-ttu-id="3e88b-p111">コア グループの管理とマネージメントに関するグループ API のサブセットのみが、アプリケーションのアクセス許可と委任されたアクセス許可をサポートします。**autoSubscribeNewMembers** の更新を含む他のすべてのグループ API のメンバーは、委任されたアクセス許可のみをサポートします。例については、「[既知の問題](https://developer.microsoft.com/graph/docs/overview/release_notes#group-permission-scopes)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3e88b-p111">Only a subset of the group API pertaining to core group administration and management support application and delegated permissions. All other members of the group API, including updating  **autoSubscribeNewMembers**, support only delegated permissions. See [known issues](https://developer.microsoft.com/graph/docs/overview/release_notes#group-permission-scopes) for examples.</span></span>

## <a name="response"></a><span data-ttu-id="3e88b-171">応答</span><span class="sxs-lookup"><span data-stu-id="3e88b-171">Response</span></span>
<span data-ttu-id="3e88b-172">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="3e88b-172">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3e88b-173">例</span><span class="sxs-lookup"><span data-stu-id="3e88b-173">Example</span></span>

#### <a name="request"></a><span data-ttu-id="3e88b-174">要求</span><span class="sxs-lookup"><span data-stu-id="3e88b-174">Request</span></span>
<span data-ttu-id="3e88b-175">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3e88b-175">The following is an example of the request body.</span></span>
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

#### <a name="response"></a><span data-ttu-id="3e88b-176">応答</span><span class="sxs-lookup"><span data-stu-id="3e88b-176">Response</span></span>
<span data-ttu-id="3e88b-177">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3e88b-177">The following is an example of a response.</span></span>
><span data-ttu-id="3e88b-178">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="3e88b-178">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3e88b-179">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="3e88b-179">All the properties will be returned from an actual call.</span></span>
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