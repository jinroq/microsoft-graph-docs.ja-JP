# <a name="directoryrole-resource-type"></a><span data-ttu-id="036c1-101">directoryRole リソース型</span><span class="sxs-lookup"><span data-stu-id="036c1-101">directoryRole resource type</span></span>

<span data-ttu-id="036c1-102">Azure AD ディレクトリの役割を表します。</span><span class="sxs-lookup"><span data-stu-id="036c1-102">Represents an Azure AD directory role.</span></span> <span data-ttu-id="036c1-103">Azure AD ディレクトリの役割は、*管理者の役割*とも呼ばれます。</span><span class="sxs-lookup"><span data-stu-id="036c1-103">Azure AD directory roles are also known as *administrator roles*.</span></span> <span data-ttu-id="036c1-104">ディレクトリ (管理者) の役割の詳細については、 [Azure AD の管理者ロールの割り当て](http://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="036c1-104">For more information about directory (administrator) roles, see [Assigning administrator roles in Azure AD](http://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/).</span></span> <span data-ttu-id="036c1-105">Graph とには、ターゲットのロールのアクセス許可を付与するディレクトリのロールにユーザーを割り当てることができます。</span><span class="sxs-lookup"><span data-stu-id="036c1-105">With the Microsoft Graph, you can assign users to directory roles to grant them the permissions of the target role.</span></span> <span data-ttu-id="036c1-106">ディレクトリのロールの読み取りや、そのメンバーにする必要があります最初でアクティブにするテナントです。</span><span class="sxs-lookup"><span data-stu-id="036c1-106">To read a directory role or update its members, it must first be activated in the tenant.</span></span> <span data-ttu-id="036c1-107">会社の管理者のディレクトリの役割のみが既定でアクティブにします。</span><span class="sxs-lookup"><span data-stu-id="036c1-107">Only the Company Administrators directory role is activated by default.</span></span> <span data-ttu-id="036c1-108">ディレクトリの役割の基になる[directoryRoleTemplate](directoryroletemplate.md)の ID で POST 要求を送信するその他の利用可能なディレクトリの役割をアクティブ化します。</span><span class="sxs-lookup"><span data-stu-id="036c1-108">To activate other available directory roles you send a POST request with the ID of the [directoryRoleTemplate](directoryroletemplate.md) on which the directory role is based.</span></span> <span data-ttu-id="036c1-109">[directoryObject](directoryobject.md) から継承します。</span><span class="sxs-lookup"><span data-stu-id="036c1-109">Inherits from [directoryObject](directoryobject.md).</span></span>
<span data-ttu-id="036c1-110">このリソースは以下をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="036c1-110">This resource supports:</span></span>

- <span data-ttu-id="036c1-111">[デルタ](../api/directoryrole_delta.md)関数を提供することにより、[デルタ クエリ](../../../concepts/delta_query_overview.md)を使用して、増分の追加、削除、更新を追跡します。</span><span class="sxs-lookup"><span data-stu-id="036c1-111">Using [delta query](../../../concepts/delta_query_overview.md) to track incremental additions, deletions, and updates, by providing a [delta](../api/directoryrole_delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="036c1-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="036c1-112">Methods</span></span>

| <span data-ttu-id="036c1-113">メソッド</span><span class="sxs-lookup"><span data-stu-id="036c1-113">Method</span></span>       | <span data-ttu-id="036c1-114">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="036c1-114">Return Type</span></span>  |<span data-ttu-id="036c1-115">説明</span><span class="sxs-lookup"><span data-stu-id="036c1-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="036c1-116">Get directoryRole</span><span class="sxs-lookup"><span data-stu-id="036c1-116">Get directoryRole</span></span>](../api/directoryrole_get.md) | [<span data-ttu-id="036c1-117">directoryRole</span><span class="sxs-lookup"><span data-stu-id="036c1-117">directoryRole</span></span>](directoryrole.md) | <span data-ttu-id="036c1-118">directoryRole オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="036c1-118">Read properties and relationships of directoryRole object.</span></span> |
|[<span data-ttu-id="036c1-119">directoryRoles を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="036c1-119">List directoryRoles</span></span>](../api/directoryrole_list.md) | <span data-ttu-id="036c1-120">[directoryRole](directoryrole.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="036c1-120">[directoryRole](directoryrole.md) collection</span></span> | <span data-ttu-id="036c1-121">テナントでアクティブになっているディレクトリ ロールを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="036c1-121">List the directory roles that are activated in the tenant.</span></span> |
|[<span data-ttu-id="036c1-122">メンバーを追加する</span><span class="sxs-lookup"><span data-stu-id="036c1-122">Add member</span></span>](../api/directoryrole_post_members.md) |[<span data-ttu-id="036c1-123">directoryObject</span><span class="sxs-lookup"><span data-stu-id="036c1-123">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="036c1-124">members ナビゲーション プロパティを送信することで、ユーザーをディレクトリ ロールに追加します。</span><span class="sxs-lookup"><span data-stu-id="036c1-124">Add a user to the directory role by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="036c1-125">List members</span><span class="sxs-lookup"><span data-stu-id="036c1-125">List members</span></span>](../api/directoryrole_list_members.md) |<span data-ttu-id="036c1-126">[directoryObject](directoryobject.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="036c1-126">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="036c1-127">members ナビゲーション プロパティから、ディレクトリ ロールのメンバーであるユーザーを取得します。</span><span class="sxs-lookup"><span data-stu-id="036c1-127">Get the users that are members of the directory role from the members navigation property.</span></span>|
|[<span data-ttu-id="036c1-128">メンバーを削除する</span><span class="sxs-lookup"><span data-stu-id="036c1-128">Remove a member</span></span>](../api/directoryrole_delete_member.md) |[<span data-ttu-id="036c1-129">directoryObject</span><span class="sxs-lookup"><span data-stu-id="036c1-129">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="036c1-130">ディレクトリ ロールからユーザーを削除します。</span><span class="sxs-lookup"><span data-stu-id="036c1-130">Remove a user from the directory role.</span></span>|
|[<span data-ttu-id="036c1-131">Activate directoryRole</span><span class="sxs-lookup"><span data-stu-id="036c1-131">Activate directoryRole</span></span>](../api/directoryrole_post_directoryroles.md) |[<span data-ttu-id="036c1-132">directoryRole</span><span class="sxs-lookup"><span data-stu-id="036c1-132">directoryRole</span></span>](directoryrole.md) | <span data-ttu-id="036c1-133">ディレクトリ ロールをアクティブにします。</span><span class="sxs-lookup"><span data-stu-id="036c1-133">Activate a directory role.</span></span>|
|[<span data-ttu-id="036c1-134">delta</span><span class="sxs-lookup"><span data-stu-id="036c1-134">delta</span></span>](../api/directoryrole_delta.md)|<span data-ttu-id="036c1-135">directoryRole コレクション</span><span class="sxs-lookup"><span data-stu-id="036c1-135">directoryRole collection</span></span>| <span data-ttu-id="036c1-136">ディレクトリの役割の増分の変更を取得します。</span><span class="sxs-lookup"><span data-stu-id="036c1-136">Get incremental changes for directory roles.</span></span> |

## <a name="properties"></a><span data-ttu-id="036c1-137">プロパティ</span><span class="sxs-lookup"><span data-stu-id="036c1-137">Properties</span></span>
| <span data-ttu-id="036c1-138">プロパティ</span><span class="sxs-lookup"><span data-stu-id="036c1-138">Property</span></span>   | <span data-ttu-id="036c1-139">型</span><span class="sxs-lookup"><span data-stu-id="036c1-139">Type</span></span> | <span data-ttu-id="036c1-140">説明</span><span class="sxs-lookup"><span data-stu-id="036c1-140">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="036c1-141">説明</span><span class="sxs-lookup"><span data-stu-id="036c1-141">description</span></span>|<span data-ttu-id="036c1-142">文字列</span><span class="sxs-lookup"><span data-stu-id="036c1-142">String</span></span>|<span data-ttu-id="036c1-p102">ディレクトリ ロールの説明。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="036c1-p102">The description for the directory role. Read-only.</span></span> |
|<span data-ttu-id="036c1-145">displayName</span><span class="sxs-lookup"><span data-stu-id="036c1-145">displayName</span></span>|<span data-ttu-id="036c1-146">文字列</span><span class="sxs-lookup"><span data-stu-id="036c1-146">String</span></span>|<span data-ttu-id="036c1-p103">ディレクトリ ロールの表示名。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="036c1-p103">The display name for the directory role. Read-only.</span></span> |
|<span data-ttu-id="036c1-149">id</span><span class="sxs-lookup"><span data-stu-id="036c1-149">id</span></span>|<span data-ttu-id="036c1-150">文字列</span><span class="sxs-lookup"><span data-stu-id="036c1-150">String</span></span>|<span data-ttu-id="036c1-p104">ディレクトリ ロールの一意識別子。[directoryObject](directoryobject.md) から継承されます。キーであり、Null は許容されません。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="036c1-p104">The unique identifier for the directory role. Inherited from [directoryObject](directoryobject.md). Key, Not nullable, Read-only.</span></span>|
|<span data-ttu-id="036c1-154">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="036c1-154">roleTemplateId</span></span>|<span data-ttu-id="036c1-155">String</span><span class="sxs-lookup"><span data-stu-id="036c1-155">String</span></span>| <span data-ttu-id="036c1-p105">このロールが基づいている [directoryRoleTemplate](directoryroletemplate.md) の **id**。このプロパティは、POST 操作でテナント内のディレクトリ ロールをアクティブ化するときに指定する必要があります。そのディレクトリ ロールがアクティブ化されると、このプロパティは読み取り専用になります。</span><span class="sxs-lookup"><span data-stu-id="036c1-p105">The **id** of the [directoryRoleTemplate](directoryroletemplate.md) that this role is based on. The property must be specified when activating a directory role in a tenant with a POST operation. After the directory role has been activated, the property is read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="036c1-159">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="036c1-159">Relationships</span></span>
| <span data-ttu-id="036c1-160">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="036c1-160">Relationship</span></span> | <span data-ttu-id="036c1-161">型</span><span class="sxs-lookup"><span data-stu-id="036c1-161">Type</span></span> |<span data-ttu-id="036c1-162">説明</span><span class="sxs-lookup"><span data-stu-id="036c1-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="036c1-163">members</span><span class="sxs-lookup"><span data-stu-id="036c1-163">members</span></span>|<span data-ttu-id="036c1-164">[directoryObject](directoryobject.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="036c1-164">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="036c1-p106">このディレクトリ ロールのメンバーであるユーザー。HTTP メソッド: GET、POST、DELETE。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="036c1-p106">Users that are members of this directory role. HTTP Methods: GET, POST, DELETE. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="036c1-169">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="036c1-169">JSON representation</span></span>

<span data-ttu-id="036c1-170">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="036c1-170">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [
    "memberOf",
    "members",
    "ownedObjects",
    "owners"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.directoryObject",
  "@odata.type": "microsoft.graph.directoryRole",
  "@odata.annotations": [
    {
      "capabilities": {
        "toppable": false
      }
    }
  ]
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
