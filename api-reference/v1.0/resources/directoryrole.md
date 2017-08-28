# <a name="directoryrole-resource-type"></a><span data-ttu-id="1ed9b-101">directoryRole リソース型</span><span class="sxs-lookup"><span data-stu-id="1ed9b-101">directoryRole resource type</span></span>

<span data-ttu-id="1ed9b-p101">Azure AD ディレクトリ ロールを表します。Azure AD ディレクトリ ロールは、*管理者ロール*と呼ばれることもあります。ディレクトリ (管理者) ロールの詳細については、「[Azure Active Directory での管理者ロールの割り当て](http://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/)」を参照してください。Microsoft Graph では、ユーザーにディレクトリ ロールを割り当てることで、ターゲット ロールのアクセス許可をユーザーに付与できます。ディレクトリ ロールを読み取る場合や、そのメンバーを更新する場合は、まず、そのディレクトリ ロールをテナントでアクティブにする必要があります。既定では、会社の管理者 (Company Administrators) ディレクトリ ロールのみがアクティブ化されています。その他の使用可能なディレクトリ ロールをアクティブ化するには、[directoryRoleTemplate](directoryroletemplate.md) の ID を使用して POST 要求を送信します。この ID は、ディレクトリ ロールに基づきます。[directoryObject](directoryobject.md) から継承します。</span><span class="sxs-lookup"><span data-stu-id="1ed9b-p101">Represents an Azure AD directory role. Azure AD directory roles are also known as *administrator roles*. For more information about directory (administrator) roles, see [Assigning administrator roles in Azure AD](http://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/). With the Microsoft Graph, you can assign users to directory roles to grant them the permissions of the target role. To read a directory role or update its members, it must first be activated in the tenant. Only the Company Administrators directory role is activated by default. To activate other available directory roles you send a POST request with the ID of the [directoryRoleTemplate](directoryroletemplate.md) on which the directory role is based. Inherits from [directoryObject](directoryobject.md).</span></span>

## <a name="methods"></a><span data-ttu-id="1ed9b-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="1ed9b-110">Methods</span></span>

| <span data-ttu-id="1ed9b-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="1ed9b-111">Method</span></span>       | <span data-ttu-id="1ed9b-112">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="1ed9b-112">Return Type</span></span>  |<span data-ttu-id="1ed9b-113">説明</span><span class="sxs-lookup"><span data-stu-id="1ed9b-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1ed9b-114">Get directoryRole</span><span class="sxs-lookup"><span data-stu-id="1ed9b-114">Get directoryRole</span></span>](../api/directoryrole_get.md) | [<span data-ttu-id="1ed9b-115">directoryRole</span><span class="sxs-lookup"><span data-stu-id="1ed9b-115">directoryRole</span></span>](directoryrole.md) | <span data-ttu-id="1ed9b-116">directoryRole オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="1ed9b-116">Read properties and relationships of directoryRole object.</span></span> |
|[<span data-ttu-id="1ed9b-117">directoryRoles を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="1ed9b-117">List directoryRoles</span></span>](../api/directoryrole_list.md) | <span data-ttu-id="1ed9b-118">[directoryRole](directoryrole.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1ed9b-118">[directoryRole](directoryrole.md) collection</span></span> | <span data-ttu-id="1ed9b-119">テナントでアクティブになっているディレクトリ ロールを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="1ed9b-119">List the directory roles that are activated in the tenant.</span></span> |
|[<span data-ttu-id="1ed9b-120">メンバーを追加する</span><span class="sxs-lookup"><span data-stu-id="1ed9b-120">Add member</span></span>](../api/directoryrole_post_members.md) |[<span data-ttu-id="1ed9b-121">directoryObject</span><span class="sxs-lookup"><span data-stu-id="1ed9b-121">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="1ed9b-122">members ナビゲーション プロパティを送信することで、ユーザーをディレクトリ ロールに追加します。</span><span class="sxs-lookup"><span data-stu-id="1ed9b-122">Add a user to the directory role by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="1ed9b-123">List members</span><span class="sxs-lookup"><span data-stu-id="1ed9b-123">List members</span></span>](../api/directoryrole_list_members.md) |<span data-ttu-id="1ed9b-124">[directoryObject](directoryobject.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1ed9b-124">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="1ed9b-125">members ナビゲーション プロパティから、ディレクトリ ロールのメンバーであるユーザーを取得します。</span><span class="sxs-lookup"><span data-stu-id="1ed9b-125">Get the users that are members of the directory role from the members navigation property.</span></span>|
|[<span data-ttu-id="1ed9b-126">メンバーを削除する</span><span class="sxs-lookup"><span data-stu-id="1ed9b-126">Remove a member</span></span>](../api/directoryrole_delete_member.md) |[<span data-ttu-id="1ed9b-127">directoryObject</span><span class="sxs-lookup"><span data-stu-id="1ed9b-127">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="1ed9b-128">ディレクトリ ロールからユーザーを削除します。</span><span class="sxs-lookup"><span data-stu-id="1ed9b-128">Remove a user from the directory role.</span></span>|
|[<span data-ttu-id="1ed9b-129">Activate directoryRole</span><span class="sxs-lookup"><span data-stu-id="1ed9b-129">Activate directoryRole</span></span>](../api/directoryrole_post_directoryroles.md) |[<span data-ttu-id="1ed9b-130">directoryRole</span><span class="sxs-lookup"><span data-stu-id="1ed9b-130">directoryRole</span></span>](directoryrole.md) | <span data-ttu-id="1ed9b-131">ディレクトリ ロールをアクティブ化します。</span><span class="sxs-lookup"><span data-stu-id="1ed9b-131">Activate a directory role.</span></span>|

## <a name="properties"></a><span data-ttu-id="1ed9b-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1ed9b-132">Properties</span></span>
| <span data-ttu-id="1ed9b-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1ed9b-133">Property</span></span>   | <span data-ttu-id="1ed9b-134">型</span><span class="sxs-lookup"><span data-stu-id="1ed9b-134">Type</span></span> | <span data-ttu-id="1ed9b-135">説明</span><span class="sxs-lookup"><span data-stu-id="1ed9b-135">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="1ed9b-136">description</span><span class="sxs-lookup"><span data-stu-id="1ed9b-136">description</span></span>|<span data-ttu-id="1ed9b-137">String</span><span class="sxs-lookup"><span data-stu-id="1ed9b-137">String</span></span>|<span data-ttu-id="1ed9b-p102">ディレクトリ ロールの説明。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="1ed9b-p102">The description for the directory role. Read-only.</span></span> |
|<span data-ttu-id="1ed9b-140">displayName</span><span class="sxs-lookup"><span data-stu-id="1ed9b-140">displayName</span></span>|<span data-ttu-id="1ed9b-141">String</span><span class="sxs-lookup"><span data-stu-id="1ed9b-141">String</span></span>|<span data-ttu-id="1ed9b-p103">ディレクトリ ロールの表示名。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="1ed9b-p103">The display name for the directory role. Read-only.</span></span> |
|<span data-ttu-id="1ed9b-144">id</span><span class="sxs-lookup"><span data-stu-id="1ed9b-144">id</span></span>|<span data-ttu-id="1ed9b-145">文字列</span><span class="sxs-lookup"><span data-stu-id="1ed9b-145">String</span></span>|<span data-ttu-id="1ed9b-p104">ディレクトリ ロールの一意識別子。[directoryObject](directoryobject.md) から継承されます。キーであり、Null は許容されません。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="1ed9b-p104">The unique identifier for the directory role. Inherited from [directoryObject](directoryobject.md). Key, Not nullable, Read-only.</span></span>|
|<span data-ttu-id="1ed9b-149">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="1ed9b-149">roleTemplateId</span></span>|<span data-ttu-id="1ed9b-150">String</span><span class="sxs-lookup"><span data-stu-id="1ed9b-150">String</span></span>| <span data-ttu-id="1ed9b-p105">このロールが基づいている [directoryRoleTemplate](directoryroletemplate.md) の **id**。このプロパティは、POST 操作でテナント内のディレクトリ ロールをアクティブ化するときに指定する必要があります。そのディレクトリ ロールがアクティブ化されると、このプロパティは読み取り専用になります。</span><span class="sxs-lookup"><span data-stu-id="1ed9b-p105">The **id** of the [directoryRoleTemplate](directoryroletemplate.md) that this role is based on. The property must be specified when activating a directory role in a tenant with a POST operation. After the directory role has been activated, the property is read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="1ed9b-154">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1ed9b-154">Relationships</span></span>
| <span data-ttu-id="1ed9b-155">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1ed9b-155">Relationship</span></span> | <span data-ttu-id="1ed9b-156">型</span><span class="sxs-lookup"><span data-stu-id="1ed9b-156">Type</span></span> |<span data-ttu-id="1ed9b-157">説明</span><span class="sxs-lookup"><span data-stu-id="1ed9b-157">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1ed9b-158">members</span><span class="sxs-lookup"><span data-stu-id="1ed9b-158">members</span></span>|<span data-ttu-id="1ed9b-159">[directoryObject](directoryobject.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1ed9b-159">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="1ed9b-p106">このディレクトリ ロールのメンバーであるユーザー。HTTP メソッド: GET、POST、DELETE。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="1ed9b-p106">Users that are members of this directory role. HTTP Methods: GET, POST, DELETE. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1ed9b-164">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1ed9b-164">JSON representation</span></span>

<span data-ttu-id="1ed9b-165">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="1ed9b-165">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "memberOf",
    "members",
    "ownedObjects",
    "owners"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directoryRole"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)",
  "roleTemplateId": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
