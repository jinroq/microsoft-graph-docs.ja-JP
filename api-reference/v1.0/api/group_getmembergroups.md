# <a name="group-getmembergroups"></a><span data-ttu-id="b3c62-101">グループ: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="b3c62-101">group: getMemberGroups</span></span>
<span data-ttu-id="b3c62-p101">指定されたグループがメンバーであるすべてのグループを返します。チェックは推移的であり、グループが直接メンバーであるグループのみを返す [memberOf](../api/group_list_memberof.md) ナビゲーション プロパティの読み取りとは異なります。</span><span class="sxs-lookup"><span data-stu-id="b3c62-p101">Return all the groups that the specified group is a member of. The check is transitive, unlike reading the [memberOf](../api/group_list_memberof.md) navigation property, which returns only the groups that the group is a direct member of.</span></span>

<span data-ttu-id="b3c62-p102">この関数は、Office 365 と Azure AD でプロビジョニングされた他の種類のグループをサポートしています。各要求を返すことができるグループの最大数は 2046 です。Office 365 グループにグループを含めることはできません。そのため、Office 365 グループのメンバーシップは常にダイレクト メンバーシップです。</span><span class="sxs-lookup"><span data-stu-id="b3c62-p102">This function supports Office 365 and other types of groups provisioned in Azure AD. The maximum number of groups each request can return is 2046. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="b3c62-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b3c62-108">Permissions</span></span>
<span data-ttu-id="b3c62-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b3c62-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b3c62-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b3c62-111">Permission type</span></span>      | <span data-ttu-id="b3c62-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b3c62-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b3c62-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b3c62-113">Delegated (work or school account)</span></span> | <span data-ttu-id="b3c62-114">Group.Read.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b3c62-114">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b3c62-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b3c62-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3c62-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b3c62-116">Not supported.</span></span>    |
|<span data-ttu-id="b3c62-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b3c62-117">Application</span></span> | <span data-ttu-id="b3c62-118">Group.Read.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3c62-118">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b3c62-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b3c62-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/getMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="b3c62-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b3c62-120">Request headers</span></span>
| <span data-ttu-id="b3c62-121">名前</span><span class="sxs-lookup"><span data-stu-id="b3c62-121">Name</span></span>       | <span data-ttu-id="b3c62-122">型</span><span class="sxs-lookup"><span data-stu-id="b3c62-122">Type</span></span> | <span data-ttu-id="b3c62-123">説明</span><span class="sxs-lookup"><span data-stu-id="b3c62-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b3c62-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b3c62-124">Authorization</span></span>  | <span data-ttu-id="b3c62-125">string</span><span class="sxs-lookup"><span data-stu-id="b3c62-125">string</span></span>  | <span data-ttu-id="b3c62-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b3c62-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b3c62-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="b3c62-128">Request body</span></span>
<span data-ttu-id="b3c62-129">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="b3c62-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b3c62-130">パラメーター</span><span class="sxs-lookup"><span data-stu-id="b3c62-130">Parameter</span></span>    | <span data-ttu-id="b3c62-131">型</span><span class="sxs-lookup"><span data-stu-id="b3c62-131">Type</span></span>   |<span data-ttu-id="b3c62-132">説明</span><span class="sxs-lookup"><span data-stu-id="b3c62-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b3c62-133">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="b3c62-133">securityEnabledOnly</span></span>|<span data-ttu-id="b3c62-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3c62-134">Boolean</span></span>|<span data-ttu-id="b3c62-p105">**false** に設定します。セキュリティが有効なグループのみを返すことは、ユーザーに対してのみサポートされます。</span><span class="sxs-lookup"><span data-stu-id="b3c62-p105">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="b3c62-137">応答</span><span class="sxs-lookup"><span data-stu-id="b3c62-137">Response</span></span>
<span data-ttu-id="b3c62-138">成功した場合、このメソッドはグループがメンバーであるグループの ID を含んだ応答本文で `200 OK` 応答コードと文字列コレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="b3c62-138">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="b3c62-139">例</span><span class="sxs-lookup"><span data-stu-id="b3c62-139">Example</span></span>
#### <a name="request"></a><span data-ttu-id="b3c62-140">要求</span><span class="sxs-lookup"><span data-stu-id="b3c62-140">Request</span></span>
<span data-ttu-id="b3c62-141">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b3c62-141">The following is an example of the request body.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_getmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/getMemberGroups
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": false
}
```

#### <a name="response"></a><span data-ttu-id="b3c62-142">応答</span><span class="sxs-lookup"><span data-stu-id="b3c62-142">Response</span></span>
<span data-ttu-id="b3c62-143">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b3c62-143">The following is an example of a response.</span></span>
><span data-ttu-id="b3c62-144">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="b3c62-144">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b3c62-145">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="b3c62-145">All the properties will be returned from an actual call.</span></span>
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
  "description": "group: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
