<span data-ttu-id="8597c-p101">[Drive](../resources/drive.md) リソースのプロパティと関係を取得します。ドライブは、ファイル システムの最上位のコンテナーです。Graph API を使用すると、ユーザーの OneDrive または OneDrive for Business や SharePoint ドキュメント ライブラリのドライブ リソースにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="8597c-p101">Retrieve the properties and relationships of a [Drive](../resources/drive.md) resource. A Drive is the top-level container for a file system. Graph API allows access to the Drive resource for a user's OneDrive or OneDrive for Business, or SharePoint document libraries.</span></span>

[Drive](../resources/drive.md) リソースのプロパティと関係を取得します。ドライブは、ファイル システムの最上位のコンテナーです。Graph API を使用すると、ユーザーの OneDrive または OneDrive for Business や SharePoint ドキュメント ライブラリのドライブ リソースにアクセスできます。

## <span data-ttu-id="8597c-105">前提条件</span><span class="sxs-lookup"><span data-stu-id="8597c-105">Prerequisites</span></span>
<a id="prerequisites" class="xliff"></a>

<span data-ttu-id="8597c-106">この API を実行するには、以下のいずれかの**スコープ**が必要です。</span><span class="sxs-lookup"><span data-stu-id="8597c-106">One of the following **scopes** is required to execute this API:</span></span>

* <span data-ttu-id="8597c-107">Files.Read</span><span class="sxs-lookup"><span data-stu-id="8597c-107">Files.Read</span></span>
* <span data-ttu-id="8597c-108">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8597c-108">Files.ReadWrite</span></span>
* <span data-ttu-id="8597c-109">Files.Read.All</span><span class="sxs-lookup"><span data-stu-id="8597c-109">Files.Read.All</span></span>
* <span data-ttu-id="8597c-110">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8597c-110">Files.ReadWrite.All</span></span>
* <span data-ttu-id="8597c-111">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="8597c-111">Sites.Read.All</span></span>
* <span data-ttu-id="8597c-112">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8597c-112">Sites.ReadWrite.All</span></span>

## <span data-ttu-id="8597c-113">ユーザーの OneDrive を取得する</span><span class="sxs-lookup"><span data-stu-id="8597c-113">Get a user's OneDrive</span></span>
<a id="get-a-users-onedrive" class="xliff"></a>

<span data-ttu-id="8597c-114">ユーザーの OneDrive または OneDrive for Business にアクセスするには、[User](../resources/user.md) リソースについての**ドライブ**関係をアプリが要求する必要があります。</span><span class="sxs-lookup"><span data-stu-id="8597c-114">To access a user's OneDrive or OneDrive for Business, your app must request the **drive** relationship on the [User](../resources/user.md) resource.</span></span>

### <span data-ttu-id="8597c-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8597c-115">HTTP request</span></span>
<a id="http-request" class="xliff"></a>

<!-- { "blockType": "ignored" } -->

```http
GET /me/drive
GET /users/{idOrUserPrincipalName}/drive
```

## <span data-ttu-id="8597c-116">グループに関連付けられたドキュメント ライブラリを取得する</span><span class="sxs-lookup"><span data-stu-id="8597c-116">Get the document library associated with a group</span></span>
<a id="get-the-document-library-associated-with-a-group" class="xliff"></a>

<span data-ttu-id="8597c-117">[グループの](../resources/group.md)既定のドキュメント ライブラリにアクセスするには、そのグループについての**ドライブ**関係をアプリが要求する必要があります。</span><span class="sxs-lookup"><span data-stu-id="8597c-117">To access a [Group's](../resources/group.md) default document library, your app requests the **drive** relationship on the Group.</span></span>

### <span data-ttu-id="8597c-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8597c-118">HTTP request</span></span>
<a id="http-request" class="xliff"></a>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/{idOrUserPrincipalName}/drive
```


## <span data-ttu-id="8597c-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="8597c-119">Optional query parameters</span></span>
<a id="optional-query-parameters" class="xliff"></a>

<span data-ttu-id="8597c-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="8597c-120">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <span data-ttu-id="8597c-121">要求本文</span><span class="sxs-lookup"><span data-stu-id="8597c-121">Request body</span></span>
<a id="request-body" class="xliff"></a>

<span data-ttu-id="8597c-122">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="8597c-122">Do not supply a request body for this method.</span></span>

## <span data-ttu-id="8597c-123">応答</span><span class="sxs-lookup"><span data-stu-id="8597c-123">Response</span></span>
<a id="response" class="xliff"></a>

<span data-ttu-id="8597c-124">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Drive](../resources/drive.md) リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="8597c-124">If successful, this method returns a `200 OK` response code and [Drive](../resources/drive.md) resource in the response body.</span></span>

## <span data-ttu-id="8597c-125">例</span><span class="sxs-lookup"><span data-stu-id="8597c-125">Example</span></span>
<a id="example" class="xliff"></a>

##### <span data-ttu-id="8597c-126">要求</span><span class="sxs-lookup"><span data-stu-id="8597c-126">Request</span></span>
<a id="request" class="xliff"></a>

<span data-ttu-id="8597c-127">サインインしているユーザーの OneDrive または OneDrive for Business を取得する要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8597c-127">Here is an example of the request to get the sign-in user's OneDrive or OneDrive for Business.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_drive"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive
```

##### <span data-ttu-id="8597c-128">応答</span><span class="sxs-lookup"><span data-stu-id="8597c-128">Response</span></span>
<a id="response" class="xliff"></a>

<span data-ttu-id="8597c-129">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="8597c-129">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.drive"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "b!t18F8ybsHUq1z3LTz8xvZqP8zaSWjkFNhsME-Fepo75dTf9vQKfeRblBZjoSQrd7",
    "driveType": "business",    
    "owner": {
        "user": {
            "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
            "displayName": "Ryan Gregg"
        }
    },
    "quota": {
        "deleted": 256938,
        "remaining": 1099447353539,
        "state": "normal",
        "total": 1099511627776
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get metadata for a OneDrive, OneDrive for Business, or Office 365 group drive",
  "keywords": "drive,onedrive,default drive,group drive",
  "section": "documentation",
  "tocPath": "OneDrive/Drive/Get Drive"
}-->
