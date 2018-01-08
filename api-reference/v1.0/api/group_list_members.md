# <a name="list-members"></a><span data-ttu-id="2f6b8-101">メンバーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="2f6b8-101">List members</span></span>
<span data-ttu-id="2f6b8-p101">グループの直接メンバーの一覧を取得します。グループは、ユーザー、連絡先、および他のグループをメンバーとして持つことができます。この操作は推移的ではありません。</span><span class="sxs-lookup"><span data-stu-id="2f6b8-p101">Get a list of the group's direct members. A group can have users, contacts, and other groups as members. This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="2f6b8-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2f6b8-105">Permissions</span></span>
<span data-ttu-id="2f6b8-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2f6b8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2f6b8-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2f6b8-108">Permission type</span></span>      | <span data-ttu-id="2f6b8-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2f6b8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2f6b8-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2f6b8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2f6b8-111">User.ReadBasic.All、User.Read.All、Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2f6b8-111">User.ReadBasic.All, User.Read.All, Directory.Read.All, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="2f6b8-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2f6b8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2f6b8-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2f6b8-113">Not supported.</span></span>    |
|<span data-ttu-id="2f6b8-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2f6b8-114">Application</span></span> | <span data-ttu-id="2f6b8-115">User.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="2f6b8-115">User.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2f6b8-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2f6b8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2f6b8-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="2f6b8-117">Optional query parameters</span></span>
<span data-ttu-id="2f6b8-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](../../../concepts/query_parameters.md)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="2f6b8-118">This method supports the [OData Query Parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2f6b8-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2f6b8-119">Request headers</span></span>
| <span data-ttu-id="2f6b8-120">名前</span><span class="sxs-lookup"><span data-stu-id="2f6b8-120">Name</span></span>       | <span data-ttu-id="2f6b8-121">型</span><span class="sxs-lookup"><span data-stu-id="2f6b8-121">Type</span></span> | <span data-ttu-id="2f6b8-122">説明</span><span class="sxs-lookup"><span data-stu-id="2f6b8-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2f6b8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f6b8-123">Authorization</span></span>  | <span data-ttu-id="2f6b8-124">string</span><span class="sxs-lookup"><span data-stu-id="2f6b8-124">string</span></span>  | <span data-ttu-id="2f6b8-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2f6b8-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2f6b8-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="2f6b8-127">Request body</span></span>
<span data-ttu-id="2f6b8-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2f6b8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2f6b8-129">応答</span><span class="sxs-lookup"><span data-stu-id="2f6b8-129">Response</span></span>
<span data-ttu-id="2f6b8-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="2f6b8-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f6b8-131">例</span><span class="sxs-lookup"><span data-stu-id="2f6b8-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="2f6b8-132">要求</span><span class="sxs-lookup"><span data-stu-id="2f6b8-132">Request</span></span>
<span data-ttu-id="2f6b8-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2f6b8-133">The following is an example of the request body.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/members
```

#### <a name="response"></a><span data-ttu-id="2f6b8-134">応答</span><span class="sxs-lookup"><span data-stu-id="2f6b8-134">Response</span></span>
<span data-ttu-id="2f6b8-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2f6b8-135">The following is an example of a response.</span></span>
><span data-ttu-id="2f6b8-136">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="2f6b8-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="2f6b8-137">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="2f6b8-137">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->