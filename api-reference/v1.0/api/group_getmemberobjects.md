# <a name="group-getmemberobjects"></a><span data-ttu-id="610ce-101">group: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="610ce-101">group: getMemberObjects</span></span>
<span data-ttu-id="610ce-p101">このグループがメンバーであるすべてのグループを返します。チェックは推移的です。注:グループは、ディレクトリ ロールのメンバーになれないので、ディレクトリ ロールは返されません。</span><span class="sxs-lookup"><span data-stu-id="610ce-p101">Return all of the groups that this group is a member of. The check is transitive. Note: Groups cannot be members of directory roles, so no directory roles will be returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="610ce-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="610ce-105">Permissions</span></span>
<span data-ttu-id="610ce-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="610ce-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="610ce-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="610ce-108">Permission type</span></span>      | <span data-ttu-id="610ce-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="610ce-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="610ce-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="610ce-110">Delegated (work or school account)</span></span> | <span data-ttu-id="610ce-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="610ce-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="610ce-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="610ce-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="610ce-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="610ce-113">Not supported.</span></span>    |
|<span data-ttu-id="610ce-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="610ce-114">Application</span></span> | <span data-ttu-id="610ce-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="610ce-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="610ce-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="610ce-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/getMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="610ce-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="610ce-117">Request headers</span></span>
| <span data-ttu-id="610ce-118">名前</span><span class="sxs-lookup"><span data-stu-id="610ce-118">Name</span></span>       | <span data-ttu-id="610ce-119">型</span><span class="sxs-lookup"><span data-stu-id="610ce-119">Type</span></span> | <span data-ttu-id="610ce-120">説明</span><span class="sxs-lookup"><span data-stu-id="610ce-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="610ce-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="610ce-121">Authorization</span></span>  | <span data-ttu-id="610ce-122">string</span><span class="sxs-lookup"><span data-stu-id="610ce-122">string</span></span>  | <span data-ttu-id="610ce-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="610ce-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="610ce-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="610ce-125">Request body</span></span>
<span data-ttu-id="610ce-126">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="610ce-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="610ce-127">パラメーター</span><span class="sxs-lookup"><span data-stu-id="610ce-127">Parameter</span></span>    | <span data-ttu-id="610ce-128">型</span><span class="sxs-lookup"><span data-stu-id="610ce-128">Type</span></span>   |<span data-ttu-id="610ce-129">説明</span><span class="sxs-lookup"><span data-stu-id="610ce-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="610ce-130">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="610ce-130">securityEnabledOnly</span></span>|<span data-ttu-id="610ce-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="610ce-131">Boolean</span></span>| <span data-ttu-id="610ce-p104">**false** に設定します。セキュリティが有効なグループのみを返すことは、ユーザーに対してのみサポートされます。</span><span class="sxs-lookup"><span data-stu-id="610ce-p104">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="610ce-134">応答</span><span class="sxs-lookup"><span data-stu-id="610ce-134">Response</span></span>
<span data-ttu-id="610ce-135">成功した場合、このメソッドはグループがメンバーであるグループの ID を含んだ応答本文で `200 OK` 応答コードと文字列コレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="610ce-135">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="610ce-136">例</span><span class="sxs-lookup"><span data-stu-id="610ce-136">Example</span></span>
#### <a name="request"></a><span data-ttu-id="610ce-137">要求</span><span class="sxs-lookup"><span data-stu-id="610ce-137">Request</span></span>
<span data-ttu-id="610ce-138">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="610ce-138">The following is an example of the request body.</span></span>
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

#### <a name="response"></a><span data-ttu-id="610ce-139">応答</span><span class="sxs-lookup"><span data-stu-id="610ce-139">Response</span></span>
<span data-ttu-id="610ce-140">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="610ce-140">The following is an example of a response.</span></span>
><span data-ttu-id="610ce-141">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="610ce-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="610ce-142">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="610ce-142">All the properties will be returned from an actual call.</span></span>
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
