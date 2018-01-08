# <a name="list-memberof"></a><span data-ttu-id="e62bb-101">memberOf を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="e62bb-101">List memberOf</span></span>
<span data-ttu-id="e62bb-102">グループが直接メンバーであるグループを取得します。</span><span class="sxs-lookup"><span data-stu-id="e62bb-102">Get groups that the group is a direct member of.</span></span> 

<span data-ttu-id="e62bb-p101">この操作は推移的ではありません。ユーザーの Office 365 のグループ取得と異なり、これは Office 365 のグループだけでなく、すべての種類のグループを返します。</span><span class="sxs-lookup"><span data-stu-id="e62bb-p101">This operation is not transitive. Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="e62bb-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e62bb-105">Permissions</span></span>
<span data-ttu-id="e62bb-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e62bb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e62bb-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e62bb-108">Permission type</span></span>      | <span data-ttu-id="e62bb-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e62bb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e62bb-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e62bb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e62bb-111">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="e62bb-111">Group.Read.All</span></span>    |
|<span data-ttu-id="e62bb-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e62bb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e62bb-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e62bb-113">Not supported.</span></span>    |
|<span data-ttu-id="e62bb-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e62bb-114">Application</span></span> | <span data-ttu-id="e62bb-115">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="e62bb-115">Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e62bb-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e62bb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e62bb-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e62bb-117">Optional query parameters</span></span>
<span data-ttu-id="e62bb-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](../../../concepts/query_parameters.md)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="e62bb-118">This method supports the [OData Query Parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e62bb-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e62bb-119">Request headers</span></span>
| <span data-ttu-id="e62bb-120">名前</span><span class="sxs-lookup"><span data-stu-id="e62bb-120">Name</span></span>       | <span data-ttu-id="e62bb-121">型</span><span class="sxs-lookup"><span data-stu-id="e62bb-121">Type</span></span> | <span data-ttu-id="e62bb-122">説明</span><span class="sxs-lookup"><span data-stu-id="e62bb-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e62bb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e62bb-123">Authorization</span></span>  | <span data-ttu-id="e62bb-124">string</span><span class="sxs-lookup"><span data-stu-id="e62bb-124">string</span></span>  | <span data-ttu-id="e62bb-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e62bb-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e62bb-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="e62bb-127">Request body</span></span>
<span data-ttu-id="e62bb-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e62bb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e62bb-129">応答</span><span class="sxs-lookup"><span data-stu-id="e62bb-129">Response</span></span>
<span data-ttu-id="e62bb-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="e62bb-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e62bb-131">例</span><span class="sxs-lookup"><span data-stu-id="e62bb-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="e62bb-132">要求</span><span class="sxs-lookup"><span data-stu-id="e62bb-132">Request</span></span>
<span data-ttu-id="e62bb-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e62bb-133">The following is an example of the request body.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_memberof"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/memberOf
```

#### <a name="response"></a><span data-ttu-id="e62bb-134">応答</span><span class="sxs-lookup"><span data-stu-id="e62bb-134">Response</span></span>
<span data-ttu-id="e62bb-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e62bb-135">The following is an example of a response.</span></span>
><span data-ttu-id="e62bb-136">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="e62bb-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e62bb-137">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="e62bb-137">All the properties will be returned from an actual call.</span></span>
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
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->