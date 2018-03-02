# <a name="list-classes"></a><span data-ttu-id="c71e8-101">クラスをリストする</span><span class="sxs-lookup"><span data-stu-id="c71e8-101">List classes</span></span>

<span data-ttu-id="c71e8-102">クラス オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="c71e8-102">Retrieve a list of chartpoints objects.</span></span> <span data-ttu-id="c71e8-103">委任されたトークンを使用した場合、メンバーは自分のクラスに関する情報以外を参照できません。</span><span class="sxs-lookup"><span data-stu-id="c71e8-103">Note that if the delegated token is used, members can only see information about their own classes.</span></span> 

<!-- Please verify the revision to the delegated token text. -->

## <a name="permissions"></a><span data-ttu-id="c71e8-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c71e8-104">Permissions</span></span>
<span data-ttu-id="c71e8-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c71e8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c71e8-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c71e8-107">Permission type</span></span>      | <span data-ttu-id="c71e8-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c71e8-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c71e8-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c71e8-109">Delegated (work or school account)</span></span> |  <span data-ttu-id="c71e8-110">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="c71e8-110">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="c71e8-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c71e8-111">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="c71e8-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c71e8-112">Not supported.</span></span>  |
|<span data-ttu-id="c71e8-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c71e8-113">Application</span></span> | <span data-ttu-id="c71e8-114">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c71e8-114">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c71e8-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c71e8-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/classes
GET /education/users/{id}/classes
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c71e8-116">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="c71e8-116">Optional query parameters</span></span>
<span data-ttu-id="c71e8-117">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://graph.microsoft.io/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c71e8-117">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c71e8-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c71e8-118">Request headers</span></span>
| <span data-ttu-id="c71e8-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c71e8-119">Header</span></span>       | <span data-ttu-id="c71e8-120">値</span><span class="sxs-lookup"><span data-stu-id="c71e8-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c71e8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c71e8-121">Authorization</span></span>  | <span data-ttu-id="c71e8-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c71e8-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c71e8-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="c71e8-124">Request body</span></span>
<span data-ttu-id="c71e8-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c71e8-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c71e8-126">応答</span><span class="sxs-lookup"><span data-stu-id="c71e8-126">Response</span></span>
<span data-ttu-id="c71e8-127">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [educationClass](../resources/educationclass.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="c71e8-127">If successful, this method returns a `200 OK` response code and collection of [groupSettingTemplate](../resources/educationclass.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c71e8-128">例</span><span class="sxs-lookup"><span data-stu-id="c71e8-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c71e8-129">要求</span><span class="sxs-lookup"><span data-stu-id="c71e8-129">Request</span></span>
<span data-ttu-id="c71e8-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c71e8-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_classes"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/me/classes
```
##### <a name="response"></a><span data-ttu-id="c71e8-131">応答</span><span class="sxs-lookup"><span data-stu-id="c71e8-131">Response</span></span>
<span data-ttu-id="c71e8-132">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c71e8-132">The following is an example of the response.</span></span> 

><span data-ttu-id="c71e8-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="c71e8-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 277

{
  "value": [
    {
      "id": "11019",
      "description": "Health Level 1",
      "classCode": "Health 501",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "displayName": "Health 1",
      "externalId": "11019",
      "externalName": "Health Level 1",
      "externalSource": "sis",
      "mailNickname": "fineartschool.net"
    } 
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List classes",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->