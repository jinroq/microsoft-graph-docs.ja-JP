# <a name="restore-deleted-item"></a><span data-ttu-id="f3b8e-101">削除済みアイテムを復元する</span><span class="sxs-lookup"><span data-stu-id="f3b8e-101">Restore deleted item</span></span>

<span data-ttu-id="f3b8e-102">[[削除済みアイテム]](../resources/directory.md) から、最近削除されたアイテムを復元します。</span><span class="sxs-lookup"><span data-stu-id="f3b8e-102">Restores a recently deleted item from [deleted items](../resources/directory.md).</span></span> 

<span data-ttu-id="f3b8e-103">現在、[削除済みアイテム] 機能は [group](../resources/group.md) および [user](../resources/user.md) リソースに対してのみサポートされています。</span><span class="sxs-lookup"><span data-stu-id="f3b8e-103">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="f3b8e-104">アイテムを誤って削除してしまった場合、そのアイテムを完全に復元できます。</span><span class="sxs-lookup"><span data-stu-id="f3b8e-104">If an item was accidentally deleted, you can fully restore the item.</span></span>

<span data-ttu-id="f3b8e-105">最近削除されたアイテムは、最大 30 日間、使用可能な状態に維持されます。</span><span class="sxs-lookup"><span data-stu-id="f3b8e-105">A recently deleted item will remain available for up to 30 days.</span></span> <span data-ttu-id="f3b8e-106">30 日が経過すると、アイテムは完全に削除されます。</span><span class="sxs-lookup"><span data-stu-id="f3b8e-106">After 30 days, the item is permanently deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="f3b8e-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f3b8e-107">Permissions</span></span>
<span data-ttu-id="f3b8e-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f3b8e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

### <a name="for-users"></a><span data-ttu-id="f3b8e-110">ユーザーの場合:</span><span class="sxs-lookup"><span data-stu-id="f3b8e-110">For users:</span></span>

|<span data-ttu-id="f3b8e-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f3b8e-111">Permission type</span></span>      | <span data-ttu-id="f3b8e-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f3b8e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f3b8e-113">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="f3b8e-113">Delegated (work or school account)</span></span> | <span data-ttu-id="f3b8e-114">User.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f3b8e-114">User.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="f3b8e-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f3b8e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f3b8e-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f3b8e-116">Not supported.</span></span> |
|<span data-ttu-id="f3b8e-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f3b8e-117">Application</span></span> | <span data-ttu-id="f3b8e-118">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3b8e-118">User.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="f3b8e-119">グループの場合:</span><span class="sxs-lookup"><span data-stu-id="f3b8e-119">For groups:</span></span>

|<span data-ttu-id="f3b8e-120">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f3b8e-120">Permission type</span></span>      | <span data-ttu-id="f3b8e-121">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f3b8e-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f3b8e-122">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="f3b8e-122">Delegated (work or school account)</span></span> | <span data-ttu-id="f3b8e-123">Group.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f3b8e-123">Group.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="f3b8e-124">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f3b8e-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f3b8e-125">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f3b8e-125">Not supported.</span></span>    |
|<span data-ttu-id="f3b8e-126">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f3b8e-126">Application</span></span> | <span data-ttu-id="f3b8e-127">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3b8e-127">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f3b8e-128">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f3b8e-128">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directory/deletedItems/{id}/restore
```

## <a name="request-headers"></a><span data-ttu-id="f3b8e-129">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f3b8e-129">Request headers</span></span>
| <span data-ttu-id="f3b8e-130">名前</span><span class="sxs-lookup"><span data-stu-id="f3b8e-130">Name</span></span>       | <span data-ttu-id="f3b8e-131">説明</span><span class="sxs-lookup"><span data-stu-id="f3b8e-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f3b8e-132">承認</span><span class="sxs-lookup"><span data-stu-id="f3b8e-132">Authorization</span></span>  | <span data-ttu-id="f3b8e-133">ベアラー &lt;コード&gt; が*必要*</span><span class="sxs-lookup"><span data-stu-id="f3b8e-133">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="f3b8e-134">承諾</span><span class="sxs-lookup"><span data-stu-id="f3b8e-134">Accept</span></span> | <span data-ttu-id="f3b8e-135">application/json</span><span class="sxs-lookup"><span data-stu-id="f3b8e-135">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="f3b8e-136">要求本文</span><span class="sxs-lookup"><span data-stu-id="f3b8e-136">Request body</span></span>
<span data-ttu-id="f3b8e-137">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f3b8e-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f3b8e-138">応答</span><span class="sxs-lookup"><span data-stu-id="f3b8e-138">Response</span></span>

<span data-ttu-id="f3b8e-139">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f3b8e-139">If successful, this method returns `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3b8e-140">例</span><span class="sxs-lookup"><span data-stu-id="f3b8e-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f3b8e-141">要求</span><span class="sxs-lookup"><span data-stu-id="f3b8e-141">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directory"
}-->
```http
POST https://graph.microsoft.com/v1.0/directory/deletedItems/{object-id}/restore
```
<span data-ttu-id="f3b8e-142">要求本文に、[directoryObject](../resources/directoryobject.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f3b8e-142">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="f3b8e-143">応答</span><span class="sxs-lookup"><span data-stu-id="f3b8e-143">Response</span></span>
<span data-ttu-id="f3b8e-p104">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f3b8e-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#directoryObjects/$entity",
  "@odata.type":"#microsoft.graph.group",
  "id":"46cc6179-19d0-473e-97ad-6ff84347bbbb",
  "displayName":"SampleGroup",
  "groupTypes":["Unified"],
  "mail":"example@contoso.com",
  "mailEnabled":true,
  "mailNickname":"Example",
  "securityEnabled":false,
  "visibility":"Public"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create deletedItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->