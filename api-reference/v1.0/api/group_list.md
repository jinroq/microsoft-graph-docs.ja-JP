# <a name="list-groups"></a><span data-ttu-id="eeacf-101">グループを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="eeacf-101">List groups</span></span>

<span data-ttu-id="eeacf-p101">Office 365 のグループを含み、それに限定されない組織で使用可能なすべてのグループを一覧表示します。各グループの[既定のプロパティ](../api/group_get.md#default-properties)が返されます。</span><span class="sxs-lookup"><span data-stu-id="eeacf-p101">List all the groups available in an organization, including but not limited to Office 365 Groups. The [default properties](../api/group_get.md#default-properties) of each group are returned.</span></span>

<span data-ttu-id="eeacf-104">Office 365 グループ (別名統合グループ) のみを一覧表示するには、**groupTypes** にフィルターを適用します。</span><span class="sxs-lookup"><span data-stu-id="eeacf-104">To list only Office 365 Groups (aka unified groups), apply a filter on **groupTypes**:</span></span>
```
GET https://graph.microsoft.com/v1.0/groups?$filter=groupTypes/any(c:c+eq+'Unified')
```

<span data-ttu-id="eeacf-105">OData クエリ オプション `$orderby` を使用して、以下の例のように、組織内のグループを **displayName** 値で並べ替えることができます。</span><span class="sxs-lookup"><span data-stu-id="eeacf-105">You can use the OData query option `$orderby` to sort groups in an organization by the **displayName** values, as shown in the following example:</span></span>
```
GET https://graph.microsoft.com/v1.0/groups?$orderby=displayName
```


## <a name="permissions"></a><span data-ttu-id="eeacf-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="eeacf-106">Permissions</span></span>
<span data-ttu-id="eeacf-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="eeacf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="eeacf-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="eeacf-109">Permission type</span></span>      | <span data-ttu-id="eeacf-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="eeacf-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eeacf-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="eeacf-111">Delegated (work or school account)</span></span> | <span data-ttu-id="eeacf-112">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eeacf-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="eeacf-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="eeacf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eeacf-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eeacf-114">Not supported.</span></span>    |
|<span data-ttu-id="eeacf-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="eeacf-115">Application</span></span> | <span data-ttu-id="eeacf-116">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eeacf-116">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="eeacf-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="eeacf-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="eeacf-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="eeacf-118">Optional query parameters</span></span>
<span data-ttu-id="eeacf-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="eeacf-119">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="eeacf-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="eeacf-120">Request headers</span></span>
| <span data-ttu-id="eeacf-121">名前</span><span class="sxs-lookup"><span data-stu-id="eeacf-121">Name</span></span>       | <span data-ttu-id="eeacf-122">型</span><span class="sxs-lookup"><span data-stu-id="eeacf-122">Type</span></span> | <span data-ttu-id="eeacf-123">説明</span><span class="sxs-lookup"><span data-stu-id="eeacf-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="eeacf-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="eeacf-124">Authorization</span></span>  | <span data-ttu-id="eeacf-125">string</span><span class="sxs-lookup"><span data-stu-id="eeacf-125">string</span></span>  | <span data-ttu-id="eeacf-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="eeacf-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eeacf-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="eeacf-128">Request body</span></span>
<span data-ttu-id="eeacf-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="eeacf-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eeacf-130">応答</span><span class="sxs-lookup"><span data-stu-id="eeacf-130">Response</span></span>

<span data-ttu-id="eeacf-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [group](../resources/group.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="eeacf-131">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="eeacf-132">例</span><span class="sxs-lookup"><span data-stu-id="eeacf-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eeacf-133">要求</span><span class="sxs-lookup"><span data-stu-id="eeacf-133">Request</span></span>
<span data-ttu-id="eeacf-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="eeacf-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groups"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups
```
##### <a name="response"></a><span data-ttu-id="eeacf-135">応答</span><span class="sxs-lookup"><span data-stu-id="eeacf-135">Response</span></span>
<span data-ttu-id="eeacf-136">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="eeacf-136">Here is an example of the response.</span></span>

<span data-ttu-id="eeacf-p104">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。実際の呼び出しでは [既定のプロパティ](../api/group_get.md#default-properties)が返されます。</span><span class="sxs-lookup"><span data-stu-id="eeacf-p104">Note: The response object shown here may be truncated for brevity. The [default properties](../api/group_get.md#default-properties) will be returned from an actual call.</span></span>

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
