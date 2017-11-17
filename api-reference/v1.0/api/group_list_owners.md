# <a name="list-owners"></a><span data-ttu-id="52089-101">所有者を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="52089-101">List owners</span></span>

<span data-ttu-id="52089-p101">グループの所有者の一覧を取得します。所有者は、グループ オブジェクトの変更を許可されている管理者以外のユーザーです。</span><span class="sxs-lookup"><span data-stu-id="52089-p101">Retrieve a list of the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span> 

## <a name="permissions"></a><span data-ttu-id="52089-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="52089-104">Permissions</span></span>
<span data-ttu-id="52089-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="52089-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="52089-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="52089-107">Permission type</span></span>      | <span data-ttu-id="52089-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="52089-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="52089-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="52089-109">Delegated (work or school account)</span></span> | <span data-ttu-id="52089-110">Group.Read.All と User.ReadBasic.All、Group.Read.All と User.Read.All、Group.Read.All と User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52089-110">Group.Read.All and User.ReadBasic.All, Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All</span></span>   |
|<span data-ttu-id="52089-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="52089-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="52089-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="52089-112">Not supported.</span></span>    |
|<span data-ttu-id="52089-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="52089-113">Application</span></span> | <span data-ttu-id="52089-114">Group.Read.All と User.Read.All、Group.Read.All と User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52089-114">Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="52089-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="52089-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/owners
```
## <a name="optional-query-parameters"></a><span data-ttu-id="52089-116">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="52089-116">Optional query parameters</span></span>
<span data-ttu-id="52089-117">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="52089-117">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="52089-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="52089-118">Request headers</span></span>
| <span data-ttu-id="52089-119">名前</span><span class="sxs-lookup"><span data-stu-id="52089-119">Name</span></span>       | <span data-ttu-id="52089-120">型</span><span class="sxs-lookup"><span data-stu-id="52089-120">Type</span></span> | <span data-ttu-id="52089-121">説明</span><span class="sxs-lookup"><span data-stu-id="52089-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="52089-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="52089-122">Authorization</span></span>  | <span data-ttu-id="52089-123">string</span><span class="sxs-lookup"><span data-stu-id="52089-123">string</span></span>  | <span data-ttu-id="52089-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="52089-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="52089-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="52089-126">Request body</span></span>
<span data-ttu-id="52089-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="52089-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="52089-128">応答</span><span class="sxs-lookup"><span data-stu-id="52089-128">Response</span></span>

<span data-ttu-id="52089-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [user](../resources/user.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="52089-129">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="52089-130">例</span><span class="sxs-lookup"><span data-stu-id="52089-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="52089-131">要求</span><span class="sxs-lookup"><span data-stu-id="52089-131">Request</span></span>
<span data-ttu-id="52089-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="52089-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/owners
```
##### <a name="response"></a><span data-ttu-id="52089-133">応答</span><span class="sxs-lookup"><span data-stu-id="52089-133">Response</span></span>
<span data-ttu-id="52089-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="52089-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
