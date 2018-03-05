# <a name="list-users"></a><span data-ttu-id="d1bc7-101">ユーザーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="d1bc7-101">List users</span></span>

<span data-ttu-id="d1bc7-102">ユーザー オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="d1bc7-102">Retrieve a list of user objects.</span></span> <span data-ttu-id="d1bc7-103">これらのユーザーオブジェクトには、教育機関に固有のプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="d1bc7-103">These user objects will include education-specific properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="d1bc7-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d1bc7-104">Permissions</span></span>
<span data-ttu-id="d1bc7-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d1bc7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d1bc7-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d1bc7-107">Permission type</span></span>      | <span data-ttu-id="d1bc7-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d1bc7-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d1bc7-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d1bc7-109">Delegated (work or school account)</span></span> |  <span data-ttu-id="d1bc7-110">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d1bc7-110">Not supported.</span></span>  |
|<span data-ttu-id="d1bc7-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d1bc7-111">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d1bc7-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d1bc7-112">Not supported.</span></span>  |
|<span data-ttu-id="d1bc7-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d1bc7-113">Application</span></span> | <span data-ttu-id="d1bc7-114">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1bc7-114">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d1bc7-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d1bc7-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/users
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d1bc7-116">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="d1bc7-116">Optional query parameters</span></span>
<span data-ttu-id="d1bc7-117">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://graph.microsoft.io/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="d1bc7-117">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d1bc7-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d1bc7-118">Request headers</span></span>
| <span data-ttu-id="d1bc7-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d1bc7-119">Header</span></span>       | <span data-ttu-id="d1bc7-120">値</span><span class="sxs-lookup"><span data-stu-id="d1bc7-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d1bc7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d1bc7-121">Authorization</span></span>  | <span data-ttu-id="d1bc7-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d1bc7-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d1bc7-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="d1bc7-124">Request body</span></span>
<span data-ttu-id="d1bc7-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d1bc7-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d1bc7-126">応答</span><span class="sxs-lookup"><span data-stu-id="d1bc7-126">Response</span></span>
<span data-ttu-id="d1bc7-127">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [educationUser](../resources/educationuser.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="d1bc7-127">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d1bc7-128">例</span><span class="sxs-lookup"><span data-stu-id="d1bc7-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d1bc7-129">要求</span><span class="sxs-lookup"><span data-stu-id="d1bc7-129">Request</span></span>
<span data-ttu-id="d1bc7-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d1bc7-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/users
```
##### <a name="response"></a><span data-ttu-id="d1bc7-131">応答</span><span class="sxs-lookup"><span data-stu-id="d1bc7-131">Response</span></span>
<span data-ttu-id="d1bc7-132">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d1bc7-132">The following is an example of the response.</span></span> 

><span data-ttu-id="d1bc7-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="d1bc7-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 593

{
  "value": [
    {
      "id": "13012",
      "displayName": "Dion Matheson",
      "givenName": "Dion",
      "middleName": null,
      "surname": "Matheson",
      "mail": "DionM@contoso.com",
      "mobilePhone": "+1 (253) 555-0101",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012"
        }
      },
      "externalSource": "sis",
      "mailingAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
      "primaryRole": "student",
      "residenceAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      }
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
