# <a name="user-getmemberobjects"></a><span data-ttu-id="dfa33-101">user: getMemberObjects　</span><span class="sxs-lookup"><span data-stu-id="dfa33-101">user: getMemberObjects</span></span>
<span data-ttu-id="dfa33-p101">ユーザーがメンバーになっているすべてのグループ、ディレクトリ ロール、管理単位を返します。チェックは推移的です。</span><span class="sxs-lookup"><span data-stu-id="dfa33-p101">Return all of the groups, directory roles and administrative units that the user is a member of. The check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="dfa33-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="dfa33-104">Permissions</span></span>
<span data-ttu-id="dfa33-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dfa33-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="dfa33-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="dfa33-107">Permission type</span></span>      | <span data-ttu-id="dfa33-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="dfa33-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dfa33-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="dfa33-109">Delegated (work or school account)</span></span> | <span data-ttu-id="dfa33-110">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="dfa33-110">One of the following scopes is required to execute this API: Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="dfa33-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="dfa33-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dfa33-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dfa33-112">Not supported.</span></span>    |
|<span data-ttu-id="dfa33-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="dfa33-113">Application</span></span> | <span data-ttu-id="dfa33-114">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dfa33-114">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dfa33-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="dfa33-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/getMemberObjects
```
## <a name="request-headers"></a><span data-ttu-id="dfa33-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dfa33-116">Request headers</span></span>
| <span data-ttu-id="dfa33-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dfa33-117">Header</span></span>       | <span data-ttu-id="dfa33-118">値</span><span class="sxs-lookup"><span data-stu-id="dfa33-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="dfa33-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="dfa33-119">Authorization</span></span>  | <span data-ttu-id="dfa33-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="dfa33-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="dfa33-122">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dfa33-122">Content-Type</span></span>  | <span data-ttu-id="dfa33-123">application/json</span><span class="sxs-lookup"><span data-stu-id="dfa33-123">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="dfa33-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="dfa33-124">Request body</span></span>
<span data-ttu-id="dfa33-125">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="dfa33-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="dfa33-126">パラメーター</span><span class="sxs-lookup"><span data-stu-id="dfa33-126">Parameter</span></span>    | <span data-ttu-id="dfa33-127">型</span><span class="sxs-lookup"><span data-stu-id="dfa33-127">Type</span></span>   |<span data-ttu-id="dfa33-128">説明</span><span class="sxs-lookup"><span data-stu-id="dfa33-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dfa33-129">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="dfa33-129">securityEnabledOnly</span></span>|<span data-ttu-id="dfa33-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="dfa33-130">Boolean</span></span>|<span data-ttu-id="dfa33-p104">ユーザーがメンバーであるセキュリティ グループのみを返すように指定するには **true**、ユーザーがメンバーであるすべてのグループとディレクトリ ロールを返すように指定するには **false** を設定します。注:このパラメーターの **true** 設定は、ユーザーに対してこのメソッドを呼び出したときにのみサポートされています。</span><span class="sxs-lookup"><span data-stu-id="dfa33-p104">**true** to specify that only security groups that the user is a member of should be returned; **false** to specify that all groups and directory roles that the user is a member of should be returned. Note: Setting this parameter to **true** is only supported when calling this method on a user.</span></span>|

## <a name="response"></a><span data-ttu-id="dfa33-133">応答</span><span class="sxs-lookup"><span data-stu-id="dfa33-133">Response</span></span>

<span data-ttu-id="dfa33-134">成功した場合、このメソッドは `200, OK` 応答コードと、応答本文で文字列コレクションを返します。応答本文には、ユーザーがメンバーであるグループとディレクトリ ロールの ID が含まれています。</span><span class="sxs-lookup"><span data-stu-id="dfa33-134">If successful, this method returns `200, OK` response code and String collection in the response body that contains the IDs of the groups and directory roles that the user is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="dfa33-135">例</span><span class="sxs-lookup"><span data-stu-id="dfa33-135">Example</span></span>
<span data-ttu-id="dfa33-136">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="dfa33-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="dfa33-137">要求</span><span class="sxs-lookup"><span data-stu-id="dfa33-137">Request</span></span>
<span data-ttu-id="dfa33-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="dfa33-138">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="dfa33-139">応答</span><span class="sxs-lookup"><span data-stu-id="dfa33-139">Response</span></span>
<span data-ttu-id="dfa33-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="dfa33-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
