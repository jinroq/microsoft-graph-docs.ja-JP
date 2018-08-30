# <a name="get-member-objects"></a><span data-ttu-id="fbac7-101">メンバー オブジェクトを取得する</span><span class="sxs-lookup"><span data-stu-id="fbac7-101">Get member objects</span></span>

 <span data-ttu-id="fbac7-p101">ユーザー、グループ、またはディレクトリ オブジェクトがメンバーであるすべてのグループとディレクトリ ロールを返します。この関数は、推移的です。</span><span class="sxs-lookup"><span data-stu-id="fbac7-p101">Returns all the groups and directory roles that a user, group, or directory object is a member of. This function is transitive.</span></span> 
 > <span data-ttu-id="fbac7-104">注:ユーザーのみがディレクトリ ロールのメンバーになることができます。</span><span class="sxs-lookup"><span data-stu-id="fbac7-104">Note: Only users can be members of directory roles.</span></span>

## <a name="permissions"></a><span data-ttu-id="fbac7-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="fbac7-105">Permissions</span></span>
<span data-ttu-id="fbac7-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fbac7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fbac7-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fbac7-108">Permission type</span></span>      | <span data-ttu-id="fbac7-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="fbac7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fbac7-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fbac7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fbac7-111">User.Read.All、Group.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="fbac7-111">User.Read.All and Group.Read.All, Directory.Read.All</span></span>    |
|<span data-ttu-id="fbac7-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fbac7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fbac7-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fbac7-113">Not supported.</span></span>    |
|<span data-ttu-id="fbac7-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fbac7-114">Application</span></span> | <span data-ttu-id="fbac7-115">User.Read.All、Group.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="fbac7-115">User.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fbac7-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fbac7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMemberObjects
POST /users/{id | userPrincipalName}/getMemberObjects
POST /groups/{id}/getMemberGroups
POST /directoryObjects/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="fbac7-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fbac7-117">Request headers</span></span>
| <span data-ttu-id="fbac7-118">名前</span><span class="sxs-lookup"><span data-stu-id="fbac7-118">Name</span></span>       | <span data-ttu-id="fbac7-119">型</span><span class="sxs-lookup"><span data-stu-id="fbac7-119">Type</span></span> | <span data-ttu-id="fbac7-120">説明</span><span class="sxs-lookup"><span data-stu-id="fbac7-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fbac7-121">承認</span><span class="sxs-lookup"><span data-stu-id="fbac7-121">Authorization</span></span>  | <span data-ttu-id="fbac7-122">文字列</span><span class="sxs-lookup"><span data-stu-id="fbac7-122">string</span></span>  | <span data-ttu-id="fbac7-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="fbac7-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fbac7-125">コンテンツ タイプ</span><span class="sxs-lookup"><span data-stu-id="fbac7-125">Content-Type</span></span>   | <span data-ttu-id="fbac7-126">文字列</span><span class="sxs-lookup"><span data-stu-id="fbac7-126">string</span></span>  | <span data-ttu-id="fbac7-127">アプリケーション/json</span><span class="sxs-lookup"><span data-stu-id="fbac7-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fbac7-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="fbac7-128">Request body</span></span>
<span data-ttu-id="fbac7-129">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="fbac7-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="fbac7-130">パラメーター</span><span class="sxs-lookup"><span data-stu-id="fbac7-130">Parameter</span></span>    | <span data-ttu-id="fbac7-131">型</span><span class="sxs-lookup"><span data-stu-id="fbac7-131">Type</span></span>   |<span data-ttu-id="fbac7-132">説明</span><span class="sxs-lookup"><span data-stu-id="fbac7-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fbac7-133">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="fbac7-133">securityEnabledOnly</span></span>|<span data-ttu-id="fbac7-134">ブール型</span><span class="sxs-lookup"><span data-stu-id="fbac7-134">Boolean</span></span>| <span data-ttu-id="fbac7-p104">エンティティがメンバーであるセキュリティ グループのみを返すように指定するには **true**、がメンバーであるすべてのグループとディレクトリ ロールを返すように指定するには **false** を設定します。**注**:パラメーターが **true** の場合、関数はユーザーでのみ呼び出せます。</span><span class="sxs-lookup"><span data-stu-id="fbac7-p104">**true** to specify that only security groups that the entity is a member of should be returned; **false** to specify that all groups and directory roles that the entity is a member of should be returned. **Note**: The function can only be called on a user if the parameter is **true**.</span></span> |

## <a name="response"></a><span data-ttu-id="fbac7-137">応答</span><span class="sxs-lookup"><span data-stu-id="fbac7-137">Response</span></span>

<span data-ttu-id="fbac7-138">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で文字列コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="fbac7-138">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fbac7-139">例</span><span class="sxs-lookup"><span data-stu-id="fbac7-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="fbac7-140">要求</span><span class="sxs-lookup"><span data-stu-id="fbac7-140">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "directoryobject_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryObjects/{object-id}/getMemberObjects
Content-type: application/json

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="fbac7-141">応答</span><span class="sxs-lookup"><span data-stu-id="fbac7-141">Response</span></span>
<span data-ttu-id="fbac7-p105">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="fbac7-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(Edm.String)",
    "value": [
        "fee2c45b-915a-4a64-b130-f4eb9e75525e",
        "4fe90ae7-065a-478b-9400-e0a0e1cbd540",
        "c9ee2d50-9e8a-4352-b97c-4c2c99557c22",
        "e0c3beaf-eeb4-43d8-abc5-94f037a65697"
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
