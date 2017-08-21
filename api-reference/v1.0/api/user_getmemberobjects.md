# <a name="user-getmemberobjects"></a><span data-ttu-id="0fb76-101">user: getMemberObjects　</span><span class="sxs-lookup"><span data-stu-id="0fb76-101">user: getMemberObjects</span></span>
<span data-ttu-id="0fb76-p101">ユーザーがメンバーになっているすべてのグループ、ディレクトリ ロール、管理単位を返します。チェックは推移的です。</span><span class="sxs-lookup"><span data-stu-id="0fb76-p101">Return all of the groups, directory roles and administrative units that the user is a member of. The check is transitive.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0fb76-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="0fb76-104">Prerequisites</span></span>
<span data-ttu-id="0fb76-105">この API を実行するには、以下のいずれかの**スコープ**が必要です。*Directory.Read.All または Directory.ReadWrite.All または Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="0fb76-105">One of the following **scopes** is required to execute this API: *Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="0fb76-106">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0fb76-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/getMemberObjects
```
## <a name="request-headers"></a><span data-ttu-id="0fb76-107">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0fb76-107">Request headers</span></span>
| <span data-ttu-id="0fb76-108">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0fb76-108">Header</span></span>       | <span data-ttu-id="0fb76-109">値</span><span class="sxs-lookup"><span data-stu-id="0fb76-109">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0fb76-110">Authorization</span><span class="sxs-lookup"><span data-stu-id="0fb76-110">Authorization</span></span>  | <span data-ttu-id="0fb76-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0fb76-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0fb76-113">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0fb76-113">Content-Type</span></span>  | <span data-ttu-id="0fb76-114">application/json</span><span class="sxs-lookup"><span data-stu-id="0fb76-114">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0fb76-115">要求本文</span><span class="sxs-lookup"><span data-stu-id="0fb76-115">Request body</span></span>
<span data-ttu-id="0fb76-116">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="0fb76-116">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0fb76-117">パラメーター</span><span class="sxs-lookup"><span data-stu-id="0fb76-117">Parameter</span></span>    | <span data-ttu-id="0fb76-118">型</span><span class="sxs-lookup"><span data-stu-id="0fb76-118">Type</span></span>   |<span data-ttu-id="0fb76-119">説明</span><span class="sxs-lookup"><span data-stu-id="0fb76-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0fb76-120">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="0fb76-120">securityEnabledOnly</span></span>|<span data-ttu-id="0fb76-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="0fb76-121">Boolean</span></span>|<span data-ttu-id="0fb76-p103">ユーザーがメンバーであるセキュリティ グループのみを返すように指定するには **true**、ユーザーがメンバーであるすべてのグループとディレクトリ ロールを返すように指定するには **false** を設定します。注:このパラメーターの **true** 設定は、ユーザーに対してこのメソッドを呼び出したときにのみサポートされています。</span><span class="sxs-lookup"><span data-stu-id="0fb76-p103">**true** to specify that only security groups that the user is a member of should be returned; **false** to specify that all groups and directory roles that the user is a member of should be returned. Note: Setting this parameter to **true** is only supported when calling this method on a user.</span></span>|

## <a name="response"></a><span data-ttu-id="0fb76-124">応答</span><span class="sxs-lookup"><span data-stu-id="0fb76-124">Response</span></span>

<span data-ttu-id="0fb76-125">成功した場合、このメソッドは `200, OK` 応答コードと、応答本文で文字列コレクションを返します。応答本文には、ユーザーがメンバーであるグループとディレクトリ ロールの ID が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0fb76-125">If successful, this method returns `200, OK` response code and String collection in the response body that contains the IDs of the groups and directory roles that the user is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="0fb76-126">例</span><span class="sxs-lookup"><span data-stu-id="0fb76-126">Example</span></span>
<span data-ttu-id="0fb76-127">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="0fb76-127">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0fb76-128">要求</span><span class="sxs-lookup"><span data-stu-id="0fb76-128">Request</span></span>
<span data-ttu-id="0fb76-129">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0fb76-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="0fb76-130">応答</span><span class="sxs-lookup"><span data-stu-id="0fb76-130">Response</span></span>
<span data-ttu-id="0fb76-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0fb76-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "value": [
    "string-value"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
