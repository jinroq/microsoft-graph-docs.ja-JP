# <a name="get-drive"></a><span data-ttu-id="88e1a-101">ドライブを取得する</span><span class="sxs-lookup"><span data-stu-id="88e1a-101">Get Drive</span></span>

<span data-ttu-id="88e1a-p101">[Drive](../resources/drive.md) リソースのプロパティと関係を取得します。ドライブは、ファイル システムの最上位のコンテナーです。Graph API を使用すると、ユーザーの OneDrive または OneDrive for Business や SharePoint ドキュメント ライブラリのドライブ リソースにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="88e1a-p101">Retrieve the properties and relationships of a [Drive](../resources/drive.md) resource. A Drive is the top-level container for a file system. Graph API allows access to the Drive resource for a user's OneDrive or OneDrive for Business, or SharePoint document libraries.</span></span>

## <a name="permissions"></a><span data-ttu-id="88e1a-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="88e1a-105">Permissions</span></span>

<span data-ttu-id="88e1a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="88e1a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="88e1a-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="88e1a-108">Permission type</span></span>      | <span data-ttu-id="88e1a-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="88e1a-109">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="88e1a-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="88e1a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="88e1a-111">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88e1a-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    | 
|<span data-ttu-id="88e1a-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="88e1a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="88e1a-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88e1a-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    | 
|<span data-ttu-id="88e1a-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="88e1a-114">Application</span></span> | <span data-ttu-id="88e1a-115">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88e1a-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> | 

## <a name="get-a-users-onedrive"></a><span data-ttu-id="88e1a-116">ユーザーの OneDrive を取得する</span><span class="sxs-lookup"><span data-stu-id="88e1a-116">Get a user's OneDrive</span></span>

<span data-ttu-id="88e1a-117">ユーザーの OneDrive または OneDrive for Business にアクセスするには、[User](../resources/user.md) リソースについての**ドライブ**関係をアプリが要求する必要があります。</span><span class="sxs-lookup"><span data-stu-id="88e1a-117">To access a user's OneDrive or OneDrive for Business, your app must request the **drive** relationship on the [User](../resources/user.md) resource.</span></span>

## <a name="http-request"></a><span data-ttu-id="88e1a-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="88e1a-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/drive
GET /users/{idOrUserPrincipalName}/drive
```

## <a name="get-the-document-library-associated-with-a-group"></a><span data-ttu-id="88e1a-119">グループに関連付けられたドキュメント ライブラリを取得する</span><span class="sxs-lookup"><span data-stu-id="88e1a-119">Get the document library associated with a group</span></span>

<span data-ttu-id="88e1a-120">[グループの](../resources/group.md)既定のドキュメント ライブラリにアクセスするには、そのグループについての**ドライブ**関係をアプリが要求する必要があります。</span><span class="sxs-lookup"><span data-stu-id="88e1a-120">To access a [Group's](../resources/group.md) default document library, your app requests the **drive** relationship on the Group.</span></span>

## <a name="http-request"></a><span data-ttu-id="88e1a-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="88e1a-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/{idOrUserPrincipalName}/drive
```


## <a name="optional-query-parameters"></a><span data-ttu-id="88e1a-122">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="88e1a-122">Optional query parameters</span></span>

<span data-ttu-id="88e1a-123">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="88e1a-123">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-body"></a><span data-ttu-id="88e1a-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="88e1a-124">Request body</span></span>

<span data-ttu-id="88e1a-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="88e1a-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="88e1a-126">応答</span><span class="sxs-lookup"><span data-stu-id="88e1a-126">Response</span></span>

<span data-ttu-id="88e1a-127">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Drive](../resources/drive.md) リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="88e1a-127">If successful, this method returns a `200 OK` response code and [Drive](../resources/drive.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88e1a-128">例</span><span class="sxs-lookup"><span data-stu-id="88e1a-128">Example</span></span>

##### <a name="request"></a><span data-ttu-id="88e1a-129">要求</span><span class="sxs-lookup"><span data-stu-id="88e1a-129">Request</span></span>

<span data-ttu-id="88e1a-130">サインインしているユーザーの OneDrive または OneDrive for Business を取得する要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="88e1a-130">Here is an example of the request to get the sign-in user's OneDrive or OneDrive for Business.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_drive"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive
```

##### <a name="response"></a><span data-ttu-id="88e1a-131">応答</span><span class="sxs-lookup"><span data-stu-id="88e1a-131">Response</span></span>

<span data-ttu-id="88e1a-132">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="88e1a-132">Here is an example of the response.</span></span>

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
