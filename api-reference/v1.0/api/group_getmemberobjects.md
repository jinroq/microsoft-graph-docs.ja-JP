# <a name="group-getmemberobjects"></a><span data-ttu-id="80fdd-101">group: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="80fdd-101">group: getMemberObjects</span></span>
<span data-ttu-id="80fdd-p101">このグループがメンバーであるすべてのグループを返します。チェックは推移的です。注:グループは、ディレクトリ ロールのメンバーになれないので、ディレクトリ ロールは返されません。</span><span class="sxs-lookup"><span data-stu-id="80fdd-p101">Return all of the groups that this group is a member of. The check is transitive. Note: Groups cannot be members of directory roles, so no directory roles will be returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="80fdd-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="80fdd-105">Permissions</span></span>
<span data-ttu-id="80fdd-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="80fdd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="80fdd-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="80fdd-108">Permission type</span></span>      | <span data-ttu-id="80fdd-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="80fdd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="80fdd-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="80fdd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="80fdd-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="80fdd-111">One of the following scopes is required to execute this API: Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="80fdd-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="80fdd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="80fdd-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="80fdd-113">Not supported.</span></span>    |
|<span data-ttu-id="80fdd-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="80fdd-114">Application</span></span> | <span data-ttu-id="80fdd-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80fdd-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="80fdd-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="80fdd-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/getMemberObjects
```
## <a name="request-headers"></a><span data-ttu-id="80fdd-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="80fdd-117">Request headers</span></span>
| <span data-ttu-id="80fdd-118">名前</span><span class="sxs-lookup"><span data-stu-id="80fdd-118">Name</span></span>       | <span data-ttu-id="80fdd-119">型</span><span class="sxs-lookup"><span data-stu-id="80fdd-119">Type</span></span> | <span data-ttu-id="80fdd-120">説明</span><span class="sxs-lookup"><span data-stu-id="80fdd-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="80fdd-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="80fdd-121">Authorization</span></span>  | <span data-ttu-id="80fdd-122">string</span><span class="sxs-lookup"><span data-stu-id="80fdd-122">string</span></span>  | <span data-ttu-id="80fdd-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="80fdd-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="80fdd-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="80fdd-125">Request body</span></span>
<span data-ttu-id="80fdd-126">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="80fdd-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="80fdd-127">パラメーター</span><span class="sxs-lookup"><span data-stu-id="80fdd-127">Parameter</span></span>    | <span data-ttu-id="80fdd-128">型</span><span class="sxs-lookup"><span data-stu-id="80fdd-128">Type</span></span>   |<span data-ttu-id="80fdd-129">説明</span><span class="sxs-lookup"><span data-stu-id="80fdd-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="80fdd-130">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="80fdd-130">securityEnabledOnly</span></span>|<span data-ttu-id="80fdd-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="80fdd-131">Boolean</span></span>| <span data-ttu-id="80fdd-p104">**false** に設定します。セキュリティが有効なグループのみを返すことは、ユーザーに対してのみサポートされます。</span><span class="sxs-lookup"><span data-stu-id="80fdd-p104">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="80fdd-134">応答</span><span class="sxs-lookup"><span data-stu-id="80fdd-134">Response</span></span>
<span data-ttu-id="80fdd-135">成功した場合、このメソッドはグループがメンバーであるグループの ID を含んだ応答本文で `200, OK` 応答コードと文字列コレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="80fdd-135">If successful, this method returns `200, OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="80fdd-136">例</span><span class="sxs-lookup"><span data-stu-id="80fdd-136">Example</span></span>
<span data-ttu-id="80fdd-137">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="80fdd-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="80fdd-138">要求</span><span class="sxs-lookup"><span data-stu-id="80fdd-138">Request</span></span>
<span data-ttu-id="80fdd-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="80fdd-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": false
}
```

##### <a name="response"></a><span data-ttu-id="80fdd-140">応答</span><span class="sxs-lookup"><span data-stu-id="80fdd-140">Response</span></span>
<span data-ttu-id="80fdd-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="80fdd-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "group: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
