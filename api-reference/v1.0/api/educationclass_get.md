# <a name="get-educationclass"></a><span data-ttu-id="5fbab-101">Get educationClass</span><span class="sxs-lookup"><span data-stu-id="5fbab-101">Get educationClass</span></span>

<span data-ttu-id="5fbab-102">システムからクラスを取得します。</span><span class="sxs-lookup"><span data-stu-id="5fbab-102">Retrieve a class from the system.</span></span> <span data-ttu-id="5fbab-103">クラスは、グループがクラスであることをシステムに示す特別なプロパティを持つユニバーサル グループです。</span><span class="sxs-lookup"><span data-stu-id="5fbab-103">A class is a universal group with a special property that indicates to the system that the group is a class.</span></span> <span data-ttu-id="5fbab-104">グループのメンバーは学生を表します。グループ管理者はクラスの教師を表します。</span><span class="sxs-lookup"><span data-stu-id="5fbab-104">Group members represent the students;  group admins represent the teachers in the class.</span></span> <span data-ttu-id="5fbab-105">委任されたトークンを使用している場合、ユーザーはユーザーがメンバーになっているクラスのみを参照できます。</span><span class="sxs-lookup"><span data-stu-id="5fbab-105">If you're using the delegated token, the user will only see classes in which they are members.</span></span>

## <a name="permissions"></a><span data-ttu-id="5fbab-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5fbab-106">Permissions</span></span>
<span data-ttu-id="5fbab-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5fbab-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5fbab-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5fbab-109">Permission type</span></span>      | <span data-ttu-id="5fbab-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5fbab-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5fbab-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5fbab-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="5fbab-112">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="5fbab-112">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="5fbab-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5fbab-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="5fbab-114">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="5fbab-114">Not supported</span></span>  |
|<span data-ttu-id="5fbab-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5fbab-115">Application</span></span> | <span data-ttu-id="5fbab-116">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5fbab-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="5fbab-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5fbab-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5fbab-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="5fbab-118">Optional query parameters</span></span>
<span data-ttu-id="5fbab-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://graph.microsoft.io/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="5fbab-119">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5fbab-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5fbab-120">Request headers</span></span>
| <span data-ttu-id="5fbab-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5fbab-121">Header</span></span>       | <span data-ttu-id="5fbab-122">値</span><span class="sxs-lookup"><span data-stu-id="5fbab-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5fbab-123">承認</span><span class="sxs-lookup"><span data-stu-id="5fbab-123">Authorization</span></span>  | <span data-ttu-id="5fbab-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5fbab-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5fbab-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="5fbab-126">Request body</span></span>
<span data-ttu-id="5fbab-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="5fbab-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="5fbab-128">応答</span><span class="sxs-lookup"><span data-stu-id="5fbab-128">Response</span></span>
<span data-ttu-id="5fbab-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [educationClass](../resources/educationclass.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="5fbab-129">If successful, this method returns a `200 OK` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5fbab-130">例</span><span class="sxs-lookup"><span data-stu-id="5fbab-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5fbab-131">要求</span><span class="sxs-lookup"><span data-stu-id="5fbab-131">Request</span></span>
<span data-ttu-id="5fbab-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5fbab-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationclass"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/classes/{class-id}
```
##### <a name="response"></a><span data-ttu-id="5fbab-133">応答</span><span class="sxs-lookup"><span data-stu-id="5fbab-133">Response</span></span>
<span data-ttu-id="5fbab-134">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5fbab-134">The following is an example of the response.</span></span> 

><span data-ttu-id="5fbab-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="5fbab-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 224

{
  "id": "11023",
  "description": "English Level 2",
  "classCode": "11023",
  "createdBy": {
    "user": {
      "displayName": "Susana Rocha",
      "id": "14012",
    }
  },
  "displayName": "English - Language 2",
  "externalId": "301",
  "externalName": "English Level 1",
  "externalSource": "School of Fine Art",
  "mailNickname": "fineartschool.net "
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->