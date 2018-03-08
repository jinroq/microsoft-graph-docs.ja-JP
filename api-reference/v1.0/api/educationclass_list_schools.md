# <a name="list-schools"></a><span data-ttu-id="1294f-101">学校をリストする</span><span class="sxs-lookup"><span data-stu-id="1294f-101">List schools</span></span>

<span data-ttu-id="1294f-102">クラスが授業を受けている学校のリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="1294f-102">Retrieve a list of schools in which the class is taught.</span></span>

## <a name="permissions"></a><span data-ttu-id="1294f-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1294f-103">Permissions</span></span>
<span data-ttu-id="1294f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1294f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1294f-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1294f-106">Permission type</span></span>      | <span data-ttu-id="1294f-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1294f-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1294f-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1294f-108">Delegated (work or school account)</span></span> |  <span data-ttu-id="1294f-109">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="1294f-109">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="1294f-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1294f-110">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="1294f-111">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="1294f-111">Not supported</span></span>  |
|<span data-ttu-id="1294f-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1294f-112">Application</span></span> | <span data-ttu-id="1294f-113">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1294f-113">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="1294f-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1294f-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/schools
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1294f-115">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="1294f-115">Optional query parameters</span></span>
<span data-ttu-id="1294f-116">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://graph.microsoft.io/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="1294f-116">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1294f-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1294f-117">Request headers</span></span>
| <span data-ttu-id="1294f-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1294f-118">Header</span></span>       | <span data-ttu-id="1294f-119">値</span><span class="sxs-lookup"><span data-stu-id="1294f-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1294f-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="1294f-120">Authorization</span></span>  | <span data-ttu-id="1294f-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1294f-p102">Bearer {token}. Required.</span></span>  |


## <a name="request-body"></a><span data-ttu-id="1294f-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="1294f-123">Request body</span></span>
<span data-ttu-id="1294f-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1294f-124">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="1294f-125">応答</span><span class="sxs-lookup"><span data-stu-id="1294f-125">Response</span></span>
<span data-ttu-id="1294f-126">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [educationSchool](../resources/educationschool.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="1294f-126">If successful, this method returns a `200 OK` response code and collection of [groupSettingTemplate](../resources/educationschool.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1294f-127">例</span><span class="sxs-lookup"><span data-stu-id="1294f-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1294f-128">要求</span><span class="sxs-lookup"><span data-stu-id="1294f-128">Request</span></span>
<span data-ttu-id="1294f-129">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1294f-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_schools"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/classes/11014/schools
```
##### <a name="response"></a><span data-ttu-id="1294f-130">応答</span><span class="sxs-lookup"><span data-stu-id="1294f-130">Response</span></span>
<span data-ttu-id="1294f-131">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1294f-131">The following is an example of the response.</span></span> 

><span data-ttu-id="1294f-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="1294f-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 892

{
  "value": [
    {
      "id": "10002",
      "displayName": "Fabrikam High School",
      "description": "Magnate school for the arts. Los Angeles School District",
      "status": "String",
      "externalSource": "String",
      "principalEmail": "AmyR@fabrikam.com",
      "principalName": "Amy Roebuck",
      "externalPrincipalId": "14007",
      "highestGrade": "12",
      "lowestGrade": "9",
      "schoolNumber": "10002",
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
      "externalId": "10002",
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