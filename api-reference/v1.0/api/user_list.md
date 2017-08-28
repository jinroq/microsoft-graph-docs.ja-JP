# <a name="list-users"></a><span data-ttu-id="8a812-101">ユーザーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="8a812-101">List users</span></span>

<span data-ttu-id="8a812-102">ユーザー オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="8a812-102">Retrieve a list of user objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="8a812-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8a812-103">Permissions</span></span>

<span data-ttu-id="8a812-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8a812-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8a812-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8a812-106">Permission type</span></span>      | <span data-ttu-id="8a812-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8a812-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8a812-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8a812-108">Delegated (work or school account)</span></span> | <span data-ttu-id="8a812-109">User.ReadBasic.All、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8a812-109">One of the following scopes is required to execute this API: User.ReadBasic.All; User.Read.All; User.ReadWrite.All; Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8a812-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8a812-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a812-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8a812-111">Not supported.</span></span>    |
|<span data-ttu-id="8a812-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8a812-112">Application</span></span> | <span data-ttu-id="8a812-113">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a812-113">One of the following scopes is required to execute this API: User.Read.All; User.ReadWrite.All; Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8a812-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8a812-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8a812-115">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="8a812-115">Optional query parameters</span></span>

<span data-ttu-id="8a812-116">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="8a812-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="8a812-117">既定では、限定的なプロパティのセットのみが返されます (_businessPhones、displayName、givenName、id、jobTitle、mail、mobilePhone、officeLocation、preferredLanguage、surname、userPrincipalName_)。</span><span class="sxs-lookup"><span data-stu-id="8a812-117">By default, only a limited set of properties are returned (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_).</span></span> 

<span data-ttu-id="8a812-p102">別のプロパティ セットを返すには、ODATA `$select` クエリ パラメーターを使用して、目的の[ユーザー](../resources/user.md) プロパティのセットを指定する必要があります。たとえば、_displayName_、_givenName_、_id_ および _postalCode_ を返すには、クエリに `$select=displayName,givenName,postalCode` を追加します。</span><span class="sxs-lookup"><span data-stu-id="8a812-p102">To return an alternative property set, you must specify the desired set of [user](../resources/user.md) properties using the ODATA `$select` query parameter. For example, to return _displayName_, _givenName_, _id_ and _postalCode_, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

> <span data-ttu-id="8a812-p103">注意: 特定のプロパティは、ユーザー コレクションでは返すことができません。[単一のユーザーを取得する](./user_get.md)場合にのみ、_aboutMe、birthday、hireDate、interests、mySite、pastProjects, preferredName、responsibilities、schools、skills、mailboxSettings_ の各プロパティがサポートされます。</span><span class="sxs-lookup"><span data-stu-id="8a812-p103">Note: Certain properties cannot be returned within a user collection. The following properties are only supported when [retrieving an single user](./user_get.md): _aboutMe, birthday, hireDate, interests, mySite, pastProjects, preferredName, responsibilities, schools, skills, mailboxSettings_</span></span>

## <a name="request-headers"></a><span data-ttu-id="8a812-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8a812-122">Request headers</span></span>

| <span data-ttu-id="8a812-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8a812-123">Header</span></span>        | <span data-ttu-id="8a812-124">値</span><span class="sxs-lookup"><span data-stu-id="8a812-124">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="8a812-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="8a812-125">Authorization</span></span> | <span data-ttu-id="8a812-126">Bearer {トークン} (必須)</span><span class="sxs-lookup"><span data-stu-id="8a812-126">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="8a812-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8a812-127">Content-Type</span></span>  | <span data-ttu-id="8a812-128">application/json</span><span class="sxs-lookup"><span data-stu-id="8a812-128">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="8a812-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="8a812-129">Request body</span></span>

<span data-ttu-id="8a812-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="8a812-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8a812-131">応答</span><span class="sxs-lookup"><span data-stu-id="8a812-131">Response</span></span>

<span data-ttu-id="8a812-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [user](../resources/user.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="8a812-132">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a812-133">例</span><span class="sxs-lookup"><span data-stu-id="8a812-133">Example</span></span>

##### <a name="request"></a><span data-ttu-id="8a812-134">要求</span><span class="sxs-lookup"><span data-stu-id="8a812-134">Request</span></span>

<span data-ttu-id="8a812-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8a812-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/v1.0/users
```

##### <a name="response"></a><span data-ttu-id="8a812-136">応答</span><span class="sxs-lookup"><span data-stu-id="8a812-136">Response</span></span>

<span data-ttu-id="8a812-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8a812-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 608

{
  "value": [
    {
      "businessPhones": [
        "businessPhones-value"
      ],
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "jobTitle": "jobTitle-value",
      "mail": "mail-value",
      "mobilePhone": "mobilePhone-value",
      "officeLocation": "officeLocation-value",
      "preferredLanguage": "preferredLanguage-value",
      "surname": "surname-value",
      "userPrincipalName": "userPrincipalName-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List users",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
