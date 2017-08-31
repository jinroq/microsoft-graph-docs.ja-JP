# <a name="get-member-groups"></a><span data-ttu-id="b96fc-101">メンバー グループを取得する</span><span class="sxs-lookup"><span data-stu-id="b96fc-101">Get member groups</span></span>

<span data-ttu-id="b96fc-p101">指定したユーザー、グループ、またはディレクトリ オブジェクトがメンバーであるすべてのグループを返します。この関数は、推移的です。</span><span class="sxs-lookup"><span data-stu-id="b96fc-p101">Return all the groups that the specified user, group, or directory object is a member of. This function is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="b96fc-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b96fc-104">Permissions</span></span>
<span data-ttu-id="b96fc-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b96fc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b96fc-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b96fc-107">Permission type</span></span>      | <span data-ttu-id="b96fc-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b96fc-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b96fc-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b96fc-109">Delegated (work or school account)</span></span> | <span data-ttu-id="b96fc-110">User.Read.All、Group.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="b96fc-110">User.Read.All and Group.Read.All, Directory.Read.All</span></span>    |
|<span data-ttu-id="b96fc-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b96fc-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b96fc-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b96fc-112">Not supported.</span></span>    |
|<span data-ttu-id="b96fc-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b96fc-113">Application</span></span> | <span data-ttu-id="b96fc-114">User.Read.All、Group.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="b96fc-114">User.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b96fc-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b96fc-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMemberGroups
POST /users/{id | userPrincipalName}/getMemberGroups
POST /groups/{id}/getMemberGroups
POST /directoryObjects/{id}/getMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="b96fc-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b96fc-116">Request headers</span></span>
| <span data-ttu-id="b96fc-117">名前</span><span class="sxs-lookup"><span data-stu-id="b96fc-117">Name</span></span>       | <span data-ttu-id="b96fc-118">型</span><span class="sxs-lookup"><span data-stu-id="b96fc-118">Type</span></span> | <span data-ttu-id="b96fc-119">説明</span><span class="sxs-lookup"><span data-stu-id="b96fc-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b96fc-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="b96fc-120">Authorization</span></span>  | <span data-ttu-id="b96fc-121">string</span><span class="sxs-lookup"><span data-stu-id="b96fc-121">string</span></span>  | <span data-ttu-id="b96fc-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b96fc-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b96fc-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b96fc-124">Content-Type</span></span>  | <span data-ttu-id="b96fc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b96fc-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b96fc-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="b96fc-126">Request body</span></span>
<span data-ttu-id="b96fc-127">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="b96fc-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b96fc-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="b96fc-128">Parameter</span></span>    | <span data-ttu-id="b96fc-129">型</span><span class="sxs-lookup"><span data-stu-id="b96fc-129">Type</span></span>   |<span data-ttu-id="b96fc-130">説明</span><span class="sxs-lookup"><span data-stu-id="b96fc-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b96fc-131">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="b96fc-131">securityEnabledOnly</span></span>|<span data-ttu-id="b96fc-132">ブール型</span><span class="sxs-lookup"><span data-stu-id="b96fc-132">Boolean</span></span>| <span data-ttu-id="b96fc-p104">エンティティがメンバーであるセキュリティ グループのみを返すように指定するには **true**、がメンバーであるすべてのグループとディレクトリ ロールを返すように指定するには **false** を設定します。**注**:パラメーターが **true** の場合、関数はユーザーでのみ呼び出せます。</span><span class="sxs-lookup"><span data-stu-id="b96fc-p104">**true** to specify that only security groups that the entity is a member of should be returned; **false** to specify that all groups and directory roles that the entity is a member of should be returned. **Note**: The function can only be called on a user if the parameter is **true**.</span></span> |

## <a name="response"></a><span data-ttu-id="b96fc-135">応答</span><span class="sxs-lookup"><span data-stu-id="b96fc-135">Response</span></span>

<span data-ttu-id="b96fc-136">成功した場合、このメソッドは `200, OK` 応答コードと、応答本文で文字列コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b96fc-136">If successful, this method returns `200, OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b96fc-137">例</span><span class="sxs-lookup"><span data-stu-id="b96fc-137">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b96fc-138">要求</span><span class="sxs-lookup"><span data-stu-id="b96fc-138">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "directoryobject_getmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/getMemberGroups
Content-type: application/json

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="b96fc-139">応答</span><span class="sxs-lookup"><span data-stu-id="b96fc-139">Response</span></span>
<span data-ttu-id="b96fc-p105">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b96fc-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
        "e0c3beaf-eeb4-43d8-abc5-94f037a65697"
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
