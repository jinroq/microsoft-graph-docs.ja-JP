# <a name="list-groups"></a><span data-ttu-id="5773d-101">グループを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="5773d-101">List groups</span></span>
<span data-ttu-id="5773d-p101">Office 365 のグループを含み、それに限定されない組織で使用可能なすべてのグループを一覧表示します。各グループの[既定のプロパティ](../api/group_get.md#default-properties)が返されます。</span><span class="sxs-lookup"><span data-stu-id="5773d-p101">List all the groups available in an organization, including but not limited to Office 365 Groups. The [default properties](../api/group_get.md#default-properties) of each group are returned.</span></span>

<span data-ttu-id="5773d-104">Office 365 グループ (別名統合グループ) のみを一覧表示するには、**groupTypes** にフィルターを適用します。</span><span class="sxs-lookup"><span data-stu-id="5773d-104">To list only Office 365 Groups (aka unified groups), apply a filter on **groupTypes**:</span></span>
```
GET https://graph.microsoft.com/v1.0/groups?$filter=groupTypes/any(c:c+eq+'Unified')
```

<span data-ttu-id="5773d-105">OData クエリ オプション `$orderby` を使用して、以下の例のように、組織内のグループを **displayName** 値で並べ替えることができます。</span><span class="sxs-lookup"><span data-stu-id="5773d-105">You can use the OData query option `$orderby` to sort groups in an organization by the **displayName** values, as shown in the following example:</span></span>
```
GET https://graph.microsoft.com/v1.0/groups?$orderby=displayName
```

## <a name="permissions"></a><span data-ttu-id="5773d-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5773d-106">Permissions</span></span>
<span data-ttu-id="5773d-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5773d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5773d-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5773d-109">Permission type</span></span>      | <span data-ttu-id="5773d-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5773d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5773d-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5773d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5773d-112">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5773d-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5773d-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5773d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5773d-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5773d-114">Not supported.</span></span>    |
|<span data-ttu-id="5773d-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5773d-115">Application</span></span> | <span data-ttu-id="5773d-116">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5773d-116">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5773d-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5773d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5773d-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="5773d-118">Optional query parameters</span></span>
<span data-ttu-id="5773d-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](../../../concepts/query_parameters.md)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="5773d-119">This method supports the [OData Query Parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5773d-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5773d-120">Request headers</span></span>
| <span data-ttu-id="5773d-121">名前</span><span class="sxs-lookup"><span data-stu-id="5773d-121">Name</span></span>       | <span data-ttu-id="5773d-122">型</span><span class="sxs-lookup"><span data-stu-id="5773d-122">Type</span></span> | <span data-ttu-id="5773d-123">説明</span><span class="sxs-lookup"><span data-stu-id="5773d-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5773d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5773d-124">Authorization</span></span>  | <span data-ttu-id="5773d-125">string</span><span class="sxs-lookup"><span data-stu-id="5773d-125">string</span></span>  | <span data-ttu-id="5773d-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5773d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5773d-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="5773d-128">Request body</span></span>
<span data-ttu-id="5773d-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="5773d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5773d-130">応答</span><span class="sxs-lookup"><span data-stu-id="5773d-130">Response</span></span>
<span data-ttu-id="5773d-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [group](../resources/group.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="5773d-131">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5773d-132">例</span><span class="sxs-lookup"><span data-stu-id="5773d-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="5773d-133">要求</span><span class="sxs-lookup"><span data-stu-id="5773d-133">Request</span></span>
<span data-ttu-id="5773d-134">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5773d-134">The following is an example of the request body.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groups"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups
```

#### <a name="response"></a><span data-ttu-id="5773d-135">応答</span><span class="sxs-lookup"><span data-stu-id="5773d-135">Response</span></span>
<span data-ttu-id="5773d-136">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5773d-136">The following is an example of a response.</span></span>

><span data-ttu-id="5773d-137">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="5773d-137">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="5773d-138">実際の呼び出しでは [既定のプロパティ](../api/group_get.md#default-properties)が返されます。</span><span class="sxs-lookup"><span data-stu-id="5773d-138">All default properties will be returned from the actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx

 {
  "value": [
    {
      "id": "id-value",
      "description": "description-value",
      "displayName": "displayName-value",
      "groupTypes": [
        "groupTypes-value"
      ],
      "mail": "mail-value",
      "mailEnabled": true,
      "mailNickname": "mailNickname-value",
      "onPremisesLastSyncDateTime": "onPremisesLastSyncDateTime-value",
      "onPremisesSecurityIdentifier": "onPremisesSecurityIdentifier-value",
      "onPremisesSyncEnabled": true,
      "proxyAddresses": [
        "proxyAddresses-value"
      ],
      "securityEnabled": true,
      "visibility": "visibility-value"
    }
  ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
