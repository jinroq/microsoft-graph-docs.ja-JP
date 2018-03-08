# <a name="list-schools"></a><span data-ttu-id="d2023-101">学校をリストする</span><span class="sxs-lookup"><span data-stu-id="d2023-101">List schools</span></span>

<span data-ttu-id="d2023-102">ユーザーの学校のリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="d2023-102">Retrieve a list of licenseDetails objects for a user.</span></span>

><span data-ttu-id="d2023-103">**注:** 委任されたトークンを使用した場合、メンバーは自分の学校に関する情報以外を参照できません。</span><span class="sxs-lookup"><span data-stu-id="d2023-103">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="d2023-104">この場合は `...beta/education/me/schools` リソースを使用してください。</span><span class="sxs-lookup"><span data-stu-id="d2023-104">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="d2023-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d2023-105">Permissions</span></span>
<span data-ttu-id="d2023-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d2023-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d2023-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d2023-108">Permission type</span></span>      | <span data-ttu-id="d2023-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d2023-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d2023-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d2023-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="d2023-111">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="d2023-111">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="d2023-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d2023-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d2023-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d2023-113">Not supported.</span></span>  |
|<span data-ttu-id="d2023-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d2023-114">Application</span></span> | <span data-ttu-id="d2023-115">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2023-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d2023-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d2023-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/schools
GET /education/users/{id}/schools
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d2023-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="d2023-117">Optional query parameters</span></span>
<span data-ttu-id="d2023-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://graph.microsoft.io/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="d2023-118">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d2023-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d2023-119">Request headers</span></span>
| <span data-ttu-id="d2023-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d2023-120">Header</span></span>       | <span data-ttu-id="d2023-121">値</span><span class="sxs-lookup"><span data-stu-id="d2023-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d2023-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2023-122">Authorization</span></span>  | <span data-ttu-id="d2023-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d2023-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d2023-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="d2023-125">Request body</span></span>
<span data-ttu-id="d2023-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d2023-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d2023-127">応答</span><span class="sxs-lookup"><span data-stu-id="d2023-127">Response</span></span>
<span data-ttu-id="d2023-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [educationSchool](../resources/educationschool.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="d2023-128">If successful, this method returns a `200 OK` response code and collection of [groupSettingTemplate](../resources/educationschool.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d2023-129">例</span><span class="sxs-lookup"><span data-stu-id="d2023-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d2023-130">要求</span><span class="sxs-lookup"><span data-stu-id="d2023-130">Request</span></span>
<span data-ttu-id="d2023-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d2023-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_schools"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/me/schools
```
##### <a name="response"></a><span data-ttu-id="d2023-132">応答</span><span class="sxs-lookup"><span data-stu-id="d2023-132">Response</span></span>
<span data-ttu-id="d2023-133">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d2023-133">The following is an example of the response.</span></span> 

><span data-ttu-id="d2023-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="d2023-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 345

{
  "value": [
    {
      "id": "10001",
      "displayName": "Contoso High School",
      "description": "Public 9-12 high school",
      "status": "active",
      "externalSource": "sis",
      "principalEmail": "amyr@contoso.com",
      "principalName": "Amy Roebuck",
      "externalPrincipalId": "14007",
      "highestGrade": "12",
      "lowestGrade": "9",
      "schoolNumber": "10001",
      "address": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "externalId": "10001",
      "fax": "+1 (253) 555-0101",
      "phone": "+1 (253) 555-0102",
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List schools",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->