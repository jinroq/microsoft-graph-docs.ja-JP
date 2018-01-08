# <a name="list-owners"></a><span data-ttu-id="1543e-101">所有者を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="1543e-101">List owners</span></span>
<span data-ttu-id="1543e-p101">グループの所有者の一覧を取得します。所有者は、グループ オブジェクトの変更を許可されている管理者以外のユーザーです。</span><span class="sxs-lookup"><span data-stu-id="1543e-p101">Retrieve a list of the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span> 

## <a name="permissions"></a><span data-ttu-id="1543e-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1543e-104">Permissions</span></span>
<span data-ttu-id="1543e-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1543e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1543e-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1543e-107">Permission type</span></span>      | <span data-ttu-id="1543e-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1543e-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1543e-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1543e-109">Delegated (work or school account)</span></span> | <span data-ttu-id="1543e-110">Group.Read.All と User.ReadBasic.All、Group.Read.All と User.Read.All、Group.Read.All と User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1543e-110">Group.Read.All and User.ReadBasic.All, Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All</span></span>   |
|<span data-ttu-id="1543e-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1543e-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1543e-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1543e-112">Not supported.</span></span>    |
|<span data-ttu-id="1543e-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1543e-113">Application</span></span> | <span data-ttu-id="1543e-114">Group.Read.All と User.Read.All、Group.Read.All と User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1543e-114">Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1543e-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1543e-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/owners
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1543e-116">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="1543e-116">Optional query parameters</span></span>
<span data-ttu-id="1543e-117">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](../../../concepts/query_parameters.md)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="1543e-117">This method supports the [OData Query Parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1543e-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1543e-118">Request headers</span></span>
| <span data-ttu-id="1543e-119">名前</span><span class="sxs-lookup"><span data-stu-id="1543e-119">Name</span></span>       | <span data-ttu-id="1543e-120">型</span><span class="sxs-lookup"><span data-stu-id="1543e-120">Type</span></span> | <span data-ttu-id="1543e-121">説明</span><span class="sxs-lookup"><span data-stu-id="1543e-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1543e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1543e-122">Authorization</span></span>  | <span data-ttu-id="1543e-123">string</span><span class="sxs-lookup"><span data-stu-id="1543e-123">string</span></span>  | <span data-ttu-id="1543e-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1543e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1543e-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="1543e-126">Request body</span></span>
<span data-ttu-id="1543e-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1543e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1543e-128">応答</span><span class="sxs-lookup"><span data-stu-id="1543e-128">Response</span></span>
<span data-ttu-id="1543e-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [user](../resources/user.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="1543e-129">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1543e-130">例</span><span class="sxs-lookup"><span data-stu-id="1543e-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="1543e-131">要求</span><span class="sxs-lookup"><span data-stu-id="1543e-131">Request</span></span>
<span data-ttu-id="1543e-132">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1543e-132">The following is an example of the request body.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/owners
```

#### <a name="response"></a><span data-ttu-id="1543e-133">応答</span><span class="sxs-lookup"><span data-stu-id="1543e-133">Response</span></span>
<span data-ttu-id="1543e-134">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1543e-134">The following is an example of a response.</span></span>
><span data-ttu-id="1543e-135">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="1543e-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1543e-136">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="1543e-136">All the properties will be returned from an actual call.</span></span>
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
      "@odata.type": "#microsoft.graph.user"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
