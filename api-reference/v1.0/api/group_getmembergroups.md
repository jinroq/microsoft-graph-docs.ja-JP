# <a name="group-getmembergroups"></a><span data-ttu-id="feffa-101">グループ: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="feffa-101">group: getMemberGroups</span></span>
<span data-ttu-id="feffa-p101">指定されたグループがメンバーであるすべてのグループを返します。チェックは推移的であり、グループが直接メンバーであるグループのみを返す [memberOf](../api/group_list_memberof.md) ナビゲーション プロパティの読み取りとは異なります。</span><span class="sxs-lookup"><span data-stu-id="feffa-p101">Return all the groups that the specified group is a member of. The check is transitive, unlike reading the [memberOf](../api/group_list_memberof.md) navigation property, which returns only the groups that the group is a direct member of.</span></span>

<span data-ttu-id="feffa-p102">この関数は、Office 365 と Azure AD でプロビジョニングされた他の種類のグループをサポートしています。各要求を返すことができるグループの最大数は 2046 です。Office 365 グループにグループを含めることはできません。そのため、Office 365 グループのメンバーシップは常にダイレクト メンバーシップです。</span><span class="sxs-lookup"><span data-stu-id="feffa-p102">This function supports Office 365 and other types of groups provisioned in Azure AD. The maximum number of groups each request can return is 2046. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="feffa-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="feffa-108">Permissions</span></span>
<span data-ttu-id="feffa-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="feffa-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

><span data-ttu-id="feffa-111">**注:** 現在この API には、Directory.Read.All 以上のアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="feffa-111">**Note:** This API currently requires the Directory.Read.All permission or higher.</span></span> <span data-ttu-id="feffa-112">Group.Read.All のアクセス許可を使用すると、エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="feffa-112">Using the Group.Read.All permission will return an error.</span></span> <span data-ttu-id="feffa-113">これは既知のバグです。</span><span class="sxs-lookup"><span data-stu-id="feffa-113">This is a known bug.</span></span>

|<span data-ttu-id="feffa-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="feffa-114">Permission type</span></span>      | <span data-ttu-id="feffa-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="feffa-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="feffa-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="feffa-116">Delegated (work or school account)</span></span> | <span data-ttu-id="feffa-117">*Group.Read.All*、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="feffa-117">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="feffa-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="feffa-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="feffa-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="feffa-119">Not supported.</span></span>    |
|<span data-ttu-id="feffa-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="feffa-120">Application</span></span> | <span data-ttu-id="feffa-121">*Group.Read.All*、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="feffa-121">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="feffa-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="feffa-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/getMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="feffa-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="feffa-123">Request headers</span></span>
| <span data-ttu-id="feffa-124">名前</span><span class="sxs-lookup"><span data-stu-id="feffa-124">Name</span></span>       | <span data-ttu-id="feffa-125">型</span><span class="sxs-lookup"><span data-stu-id="feffa-125">Type</span></span> | <span data-ttu-id="feffa-126">説明</span><span class="sxs-lookup"><span data-stu-id="feffa-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="feffa-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="feffa-127">Authorization</span></span>  | <span data-ttu-id="feffa-128">string</span><span class="sxs-lookup"><span data-stu-id="feffa-128">string</span></span>  | <span data-ttu-id="feffa-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="feffa-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="feffa-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="feffa-131">Request body</span></span>
<span data-ttu-id="feffa-132">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="feffa-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="feffa-133">パラメーター</span><span class="sxs-lookup"><span data-stu-id="feffa-133">Parameter</span></span>    | <span data-ttu-id="feffa-134">型</span><span class="sxs-lookup"><span data-stu-id="feffa-134">Type</span></span>   |<span data-ttu-id="feffa-135">説明</span><span class="sxs-lookup"><span data-stu-id="feffa-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="feffa-136">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="feffa-136">securityEnabledOnly</span></span>|<span data-ttu-id="feffa-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="feffa-137">Boolean</span></span>|<span data-ttu-id="feffa-p106">**false** に設定します。セキュリティが有効なグループのみを返すことは、ユーザーに対してのみサポートされます。</span><span class="sxs-lookup"><span data-stu-id="feffa-p106">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="feffa-140">応答</span><span class="sxs-lookup"><span data-stu-id="feffa-140">Response</span></span>
<span data-ttu-id="feffa-141">成功した場合、このメソッドはグループがメンバーであるグループの ID を含んだ応答本文で `200 OK` 応答コードと文字列コレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="feffa-141">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="feffa-142">例</span><span class="sxs-lookup"><span data-stu-id="feffa-142">Example</span></span>
#### <a name="request"></a><span data-ttu-id="feffa-143">要求</span><span class="sxs-lookup"><span data-stu-id="feffa-143">Request</span></span>
<span data-ttu-id="feffa-144">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="feffa-144">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="feffa-145">応答</span><span class="sxs-lookup"><span data-stu-id="feffa-145">Response</span></span>
<span data-ttu-id="feffa-146">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="feffa-146">The following is an example of the response.</span></span>
><span data-ttu-id="feffa-p107">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="feffa-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
