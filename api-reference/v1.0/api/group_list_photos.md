# <a name="list-photos"></a><span data-ttu-id="22e48-101">写真の一覧表示</span><span class="sxs-lookup"><span data-stu-id="22e48-101">List photos</span></span>
<span data-ttu-id="22e48-102">[profilePhoto](../resources/profilephoto.md) オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="22e48-102">Retrieve a list of [profilePhoto](../resources/profilephoto.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="22e48-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="22e48-103">Permissions</span></span>
<span data-ttu-id="22e48-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="22e48-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="22e48-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="22e48-106">Permission type</span></span>      | <span data-ttu-id="22e48-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="22e48-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="22e48-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="22e48-108">Delegated (work or school account)</span></span> | <span data-ttu-id="22e48-109">Group.ReadBasic.All、Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22e48-109">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span> |
|<span data-ttu-id="22e48-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="22e48-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="22e48-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="22e48-111">Not supported.</span></span>    |
|<span data-ttu-id="22e48-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="22e48-112">Application</span></span> | <span data-ttu-id="22e48-113">Group.ReadBasic.All、Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22e48-113">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="22e48-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="22e48-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/photos
GET /users/{id | userPrincipalName}/joinedGroups/{id}/photos
```
## <a name="optional-query-parameters"></a><span data-ttu-id="22e48-115">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="22e48-115">Optional query parameters</span></span>
<span data-ttu-id="22e48-116">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](../../../concepts/query_parameters.md)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="22e48-116">This method supports the [OData Query Parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="22e48-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="22e48-117">Request headers</span></span>
| <span data-ttu-id="22e48-118">名前</span><span class="sxs-lookup"><span data-stu-id="22e48-118">Name</span></span>       | <span data-ttu-id="22e48-119">型</span><span class="sxs-lookup"><span data-stu-id="22e48-119">Type</span></span> | <span data-ttu-id="22e48-120">説明</span><span class="sxs-lookup"><span data-stu-id="22e48-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="22e48-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="22e48-121">Authorization</span></span>  | <span data-ttu-id="22e48-122">string</span><span class="sxs-lookup"><span data-stu-id="22e48-122">string</span></span>  | <span data-ttu-id="22e48-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="22e48-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="22e48-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="22e48-125">Request body</span></span>
<span data-ttu-id="22e48-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="22e48-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22e48-127">応答</span><span class="sxs-lookup"><span data-stu-id="22e48-127">Response</span></span>
<span data-ttu-id="22e48-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [profilePhoto](../resources/profilephoto.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="22e48-128">If successful, this method returns a `200 OK` response code and collection of [profilePhoto](../resources/profilephoto.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22e48-129">例</span><span class="sxs-lookup"><span data-stu-id="22e48-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="22e48-130">要求</span><span class="sxs-lookup"><span data-stu-id="22e48-130">Request</span></span>
<span data-ttu-id="22e48-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="22e48-131">The following is an example of the request body.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_photos"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/photos
```

#### <a name="response"></a><span data-ttu-id="22e48-132">応答</span><span class="sxs-lookup"><span data-stu-id="22e48-132">Response</span></span>
<span data-ttu-id="22e48-133">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="22e48-133">The following is an example of a response.</span></span>
><span data-ttu-id="22e48-134">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="22e48-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="22e48-135">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="22e48-135">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.profilePhoto",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 94

{
  "value": [
    {
      "height": 99,
      "width": 99,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List photos",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
