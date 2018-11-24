# <a name="list-domainnamereferences"></a><span data-ttu-id="5b314-101">domainNameReferences の一覧表示</span><span class="sxs-lookup"><span data-stu-id="5b314-101">List domainNameReferences</span></span>

<span data-ttu-id="5b314-p101">ドメインへの参照付きの [directoryObject](../resources/directoryobject.md) の一覧を取得します。返されるリストには、ドメインに依存するすべてのディレクトリ オブジェクトが含まれます。</span><span class="sxs-lookup"><span data-stu-id="5b314-p101">Retrieve a list of [directoryObject](../resources/directoryobject.md) with a reference to the domain. The returned list will contain all directory objects that have a dependency on the domain.</span></span>

## <a name="permissions"></a><span data-ttu-id="5b314-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5b314-104">Permissions</span></span>

<span data-ttu-id="5b314-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5b314-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="5b314-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5b314-107">Permission type</span></span>      | <span data-ttu-id="5b314-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5b314-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5b314-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5b314-109">Delegated (work or school account)</span></span> | <span data-ttu-id="5b314-110">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b314-110">Directory.Read.All</span></span>    |
|<span data-ttu-id="5b314-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5b314-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b314-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5b314-112">Not supported.</span></span>    |
|<span data-ttu-id="5b314-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5b314-113">Application</span></span> | <span data-ttu-id="5b314-114">Directory.Read.All、Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b314-114">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5b314-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5b314-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}/domainNameReferences
```

> <span data-ttu-id="5b314-116">{Id} には、ドメインを完全修飾ドメイン名で指定します。</span><span class="sxs-lookup"><span data-stu-id="5b314-116">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="5b314-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="5b314-117">Optional query parameters</span></span>

<span data-ttu-id="5b314-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="5b314-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5b314-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5b314-119">Request headers</span></span>

| <span data-ttu-id="5b314-120">名前</span><span class="sxs-lookup"><span data-stu-id="5b314-120">Name</span></span>      |<span data-ttu-id="5b314-121">説明</span><span class="sxs-lookup"><span data-stu-id="5b314-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5b314-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b314-122">Authorization</span></span>  | <span data-ttu-id="5b314-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5b314-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5b314-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="5b314-125">Request body</span></span>

<span data-ttu-id="5b314-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="5b314-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5b314-127">応答</span><span class="sxs-lookup"><span data-stu-id="5b314-127">Response</span></span>

<span data-ttu-id="5b314-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="5b314-128">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b314-129">例</span><span class="sxs-lookup"><span data-stu-id="5b314-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5b314-130">要求</span><span class="sxs-lookup"><span data-stu-id="5b314-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_domainnamereferences"
}-->
```http
GET https://graph.microsoft.com/v1.0/domains/{domain-name}/domainNameReferences
```

##### <a name="response"></a><span data-ttu-id="5b314-131">応答</span><span class="sxs-lookup"><span data-stu-id="5b314-131">Response</span></span>
<span data-ttu-id="5b314-p104">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5b314-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "value": [
    {
        "odata.type": "Microsoft.DirectoryServices.User",
        "objectType": "User",
        "objectId": "567a0db6-289c-43f7-a650-2645c03cbbbb",
        "accountEnabled": true,
        "displayName": "TestUser1",
        "facsimileTelephoneNumber": null,
        "mailNickname": "testuser1",
        "mobile": null,
        "userPrincipalName": "testuser1@contoso.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List domainNameReferences",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->