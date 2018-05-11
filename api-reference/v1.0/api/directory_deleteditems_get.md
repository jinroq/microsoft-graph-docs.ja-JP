# <a name="get-deleted-item"></a><span data-ttu-id="ce0dd-101">削除済みアイテムを取得する</span><span class="sxs-lookup"><span data-stu-id="ce0dd-101">Get deleted item</span></span>

<span data-ttu-id="ce0dd-102">[[削除済みアイテム]](../resources/directory.md) から、最近削除されたアイテムのプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="ce0dd-102">Retrieve the properties of a recently deleted item in [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="ce0dd-103">現在、[削除済みアイテム] 機能は [group](../resources/group.md) および [user](../resources/user.md) リソースに対してのみサポートされています。</span><span class="sxs-lookup"><span data-stu-id="ce0dd-103">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="ce0dd-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ce0dd-104">Permissions</span></span>
<span data-ttu-id="ce0dd-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ce0dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

### <a name="for-users"></a><span data-ttu-id="ce0dd-107">ユーザーの場合:</span><span class="sxs-lookup"><span data-stu-id="ce0dd-107">For users:</span></span>

|<span data-ttu-id="ce0dd-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ce0dd-108">Permission type</span></span>      | <span data-ttu-id="ce0dd-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ce0dd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ce0dd-110">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="ce0dd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ce0dd-111">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ce0dd-111">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="ce0dd-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ce0dd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce0dd-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ce0dd-113">Not supported.</span></span> |
|<span data-ttu-id="ce0dd-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ce0dd-114">Application</span></span> | <span data-ttu-id="ce0dd-115">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce0dd-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="ce0dd-116">グループの場合:</span><span class="sxs-lookup"><span data-stu-id="ce0dd-116">For groups:</span></span>

|<span data-ttu-id="ce0dd-117">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ce0dd-117">Permission type</span></span>      | <span data-ttu-id="ce0dd-118">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ce0dd-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ce0dd-119">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="ce0dd-119">Delegated (work or school account)</span></span> | <span data-ttu-id="ce0dd-120">Group.Read.All、Group.ReadWrite.All、Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ce0dd-120">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="ce0dd-121">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ce0dd-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce0dd-122">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ce0dd-122">Not supported.</span></span>    |
|<span data-ttu-id="ce0dd-123">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ce0dd-123">Application</span></span> | <span data-ttu-id="ce0dd-124">Group.Read.All、Group.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce0dd-124">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ce0dd-125">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ce0dd-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directory/deleteditems/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ce0dd-126">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="ce0dd-126">Optional query parameters</span></span>
<span data-ttu-id="ce0dd-127">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://graph.microsoft.io/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="ce0dd-127">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ce0dd-128">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ce0dd-128">Request headers</span></span>
| <span data-ttu-id="ce0dd-129">名前</span><span class="sxs-lookup"><span data-stu-id="ce0dd-129">Name</span></span>      |<span data-ttu-id="ce0dd-130">説明</span><span class="sxs-lookup"><span data-stu-id="ce0dd-130">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ce0dd-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce0dd-131">Authorization</span></span>  | <span data-ttu-id="ce0dd-132">ベアラー &lt;コード&gt; が*必要*</span><span class="sxs-lookup"><span data-stu-id="ce0dd-132">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="ce0dd-133">Accept</span><span class="sxs-lookup"><span data-stu-id="ce0dd-133">Accept</span></span>  | <span data-ttu-id="ce0dd-134">application/json</span><span class="sxs-lookup"><span data-stu-id="ce0dd-134">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="ce0dd-135">要求本文</span><span class="sxs-lookup"><span data-stu-id="ce0dd-135">Request body</span></span>
<span data-ttu-id="ce0dd-136">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ce0dd-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ce0dd-137">応答</span><span class="sxs-lookup"><span data-stu-id="ce0dd-137">Response</span></span>

<span data-ttu-id="ce0dd-138">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ce0dd-138">If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ce0dd-139">例</span><span class="sxs-lookup"><span data-stu-id="ce0dd-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ce0dd-140">要求</span><span class="sxs-lookup"><span data-stu-id="ce0dd-140">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_directory"
}-->
```http
GET https://graph.microsoft.com/v1.0/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb
```
##### <a name="response"></a><span data-ttu-id="ce0dd-141">応答</span><span class="sxs-lookup"><span data-stu-id="ce0dd-141">Response</span></span>
<span data-ttu-id="ce0dd-p102">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ce0dd-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directory"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#directoryObjects/$entity",
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
  "description": "Get directory",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->