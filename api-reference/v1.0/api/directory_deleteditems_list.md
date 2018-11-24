# <a name="list-deleted-items"></a><span data-ttu-id="e6a17-101">削除済みアイテムを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="e6a17-101">List deleted items</span></span>

<span data-ttu-id="e6a17-102">[[削除済みアイテム]](../resources/directory.md) から、最近削除されたアイテムのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="e6a17-102">Retrieve a list of recently deleted items from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="e6a17-103">現在、[削除済みアイテム] 機能は [group](../resources/group.md) および [user](../resources/user.md) リソースに対してのみサポートされています。</span><span class="sxs-lookup"><span data-stu-id="e6a17-103">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="e6a17-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e6a17-104">Permissions</span></span>
<span data-ttu-id="e6a17-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e6a17-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

### <a name="for-users"></a><span data-ttu-id="e6a17-107">ユーザーの場合:</span><span class="sxs-lookup"><span data-stu-id="e6a17-107">For users:</span></span>

|<span data-ttu-id="e6a17-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e6a17-108">Permission type</span></span>      | <span data-ttu-id="e6a17-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e6a17-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e6a17-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e6a17-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e6a17-111">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e6a17-111">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="e6a17-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e6a17-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e6a17-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e6a17-113">Not supported.</span></span> |
|<span data-ttu-id="e6a17-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e6a17-114">Application</span></span> | <span data-ttu-id="e6a17-115">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6a17-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="e6a17-116">グループの場合:</span><span class="sxs-lookup"><span data-stu-id="e6a17-116">For groups:</span></span>

|<span data-ttu-id="e6a17-117">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e6a17-117">Permission type</span></span>      | <span data-ttu-id="e6a17-118">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e6a17-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e6a17-119">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="e6a17-119">Delegated (work or school account)</span></span> | <span data-ttu-id="e6a17-120">Group.Read.All、Group.ReadWrite.All、Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e6a17-120">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="e6a17-121">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e6a17-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e6a17-122">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e6a17-122">Not supported.</span></span>    |
|<span data-ttu-id="e6a17-123">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e6a17-123">Application</span></span> | <span data-ttu-id="e6a17-124">Group.Read.All、Group.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="e6a17-124">Group.Read.All, Group.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e6a17-125">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e6a17-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http 
GET /directory/deletedItems/microsoft.graph.group
GET /directory/deletedItems/microsoft.graph.user
```

<span data-ttu-id="e6a17-126">この API は現在、削除済みアイテムからのグループ (microsoft.graph.group) またはユーザー (microsoft.graph.user) のオブジェクト タイプの取得をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="e6a17-126">This API currently supports retrieving object types of groups (microsoft.graph.group) or users (microsoft.graph.user) from deleted items.</span></span> <span data-ttu-id="e6a17-127">タイムは、URI の必須部分として指定します。</span><span class="sxs-lookup"><span data-stu-id="e6a17-127">The type is specified as a required part of the URI.</span></span> <span data-ttu-id="e6a17-128">GET/ディレクトリ/を呼び出す型のない deletedItems はサポートされません。</span><span class="sxs-lookup"><span data-stu-id="e6a17-128">Calling GET /directory/deletedItems without a type is not supported.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="e6a17-129">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e6a17-129">Optional query parameters</span></span>
<span data-ttu-id="e6a17-130">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="e6a17-130">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e6a17-131">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e6a17-131">Request headers</span></span>
| <span data-ttu-id="e6a17-132">名前</span><span class="sxs-lookup"><span data-stu-id="e6a17-132">Name</span></span>      |<span data-ttu-id="e6a17-133">説明</span><span class="sxs-lookup"><span data-stu-id="e6a17-133">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e6a17-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="e6a17-134">Authorization</span></span>  | <span data-ttu-id="e6a17-135">ベアラー &lt;コード&gt; が*必要*</span><span class="sxs-lookup"><span data-stu-id="e6a17-135">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="e6a17-136">Accept</span><span class="sxs-lookup"><span data-stu-id="e6a17-136">Accept</span></span>  | <span data-ttu-id="e6a17-137">application/json</span><span class="sxs-lookup"><span data-stu-id="e6a17-137">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="e6a17-138">要求本文</span><span class="sxs-lookup"><span data-stu-id="e6a17-138">Request body</span></span>
<span data-ttu-id="e6a17-139">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e6a17-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e6a17-140">応答</span><span class="sxs-lookup"><span data-stu-id="e6a17-140">Response</span></span>

<span data-ttu-id="e6a17-141">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="e6a17-141">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e6a17-142">例</span><span class="sxs-lookup"><span data-stu-id="e6a17-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e6a17-143">要求</span><span class="sxs-lookup"><span data-stu-id="e6a17-143">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_deleteditems"
}-->
```http
GET https://graph.microsoft.com/v1.0/directory/deletedItems/microsoft.graph.group
```
##### <a name="response"></a><span data-ttu-id="e6a17-144">応答</span><span class="sxs-lookup"><span data-stu-id="e6a17-144">Response</span></span>
<span data-ttu-id="e6a17-p103">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e6a17-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "value": [
    {
      "id":"46cc6179-19d0-473e-97ad-6ff84347bbbb",
      "displayName":"SampleGroup",
      "groupTypes":["Unified"],
      "mail":"example@contoso.com",
      "mailEnabled":true,
      "mailNickname":"Example",
      "securityEnabled":false,
      "visibility":"Public"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List deleteditems",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->