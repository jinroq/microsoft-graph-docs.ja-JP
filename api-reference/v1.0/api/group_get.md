# <a name="get-group"></a><span data-ttu-id="6bfd9-101">グループを取得する</span><span class="sxs-lookup"><span data-stu-id="6bfd9-101">Get group</span></span>

<span data-ttu-id="6bfd9-102">グループ オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="6bfd9-102">Get the properties and relationships of a group object.</span></span>

##### <a name="default-properties"></a><span data-ttu-id="6bfd9-103">既定のプロパティ</span><span class="sxs-lookup"><span data-stu-id="6bfd9-103">Default properties</span></span>

<span data-ttu-id="6bfd9-p101">以下は、グループを取得または一覧表示するときに返されるプロパティの既定のセットを表します。これらは、利用可能なすべてのプロパティのサブセットです。</span><span class="sxs-lookup"><span data-stu-id="6bfd9-p101">The following represent the default set of properties that are returned when getting or listing groups. These are a subset of all available properties.</span></span> 

* <span data-ttu-id="6bfd9-106">description</span><span class="sxs-lookup"><span data-stu-id="6bfd9-106">description</span></span>
* <span data-ttu-id="6bfd9-107">displayName</span><span class="sxs-lookup"><span data-stu-id="6bfd9-107">displayName</span></span>
* <span data-ttu-id="6bfd9-108">groupTypes</span><span class="sxs-lookup"><span data-stu-id="6bfd9-108">groupTypes</span></span>
* <span data-ttu-id="6bfd9-109">id</span><span class="sxs-lookup"><span data-stu-id="6bfd9-109">id</span></span>
* <span data-ttu-id="6bfd9-110">mail</span><span class="sxs-lookup"><span data-stu-id="6bfd9-110">mail</span></span>
* <span data-ttu-id="6bfd9-111">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="6bfd9-111">mailEnabled</span></span>
* <span data-ttu-id="6bfd9-112">mailNickname</span><span class="sxs-lookup"><span data-stu-id="6bfd9-112">mailNickname</span></span>
* <span data-ttu-id="6bfd9-113">onPremisesLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="6bfd9-113">onPremisesLastSyncDateTime</span></span>
* <span data-ttu-id="6bfd9-114">onPremisesSecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="6bfd9-114">onPremisesSecurityIdentifier</span></span>
* <span data-ttu-id="6bfd9-115">onPremisesSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="6bfd9-115">onPremisesSyncEnabled</span></span>
* <span data-ttu-id="6bfd9-116">proxyAddresses</span><span class="sxs-lookup"><span data-stu-id="6bfd9-116">proxyAddresses</span></span>
* <span data-ttu-id="6bfd9-117">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="6bfd9-117">securityEnabled</span></span>
* <span data-ttu-id="6bfd9-118">visibility</span><span class="sxs-lookup"><span data-stu-id="6bfd9-118">visibility</span></span>

<span data-ttu-id="6bfd9-119">次のグループ プロパティは既定では返されません。</span><span class="sxs-lookup"><span data-stu-id="6bfd9-119">The following group properties are not returned by default:</span></span>

* <span data-ttu-id="6bfd9-120">allowExternalSenders</span><span class="sxs-lookup"><span data-stu-id="6bfd9-120">allowExternalSenders</span></span>
* <span data-ttu-id="6bfd9-121">autoSubscribeNewMembers</span><span class="sxs-lookup"><span data-stu-id="6bfd9-121">autoSubscribeNewMembers</span></span>
* <span data-ttu-id="6bfd9-122">isSubscribedByMail</span><span class="sxs-lookup"><span data-stu-id="6bfd9-122">isSubscribedByMail</span></span>
* <span data-ttu-id="6bfd9-123">unseenCount</span><span class="sxs-lookup"><span data-stu-id="6bfd9-123">unseenCount</span></span>

<span data-ttu-id="6bfd9-p102">これらのプロパティを取得するには、**$select** クエリ パラメーターを使用します。次に、例を示します。</span><span class="sxs-lookup"><span data-stu-id="6bfd9-p102">To get these properties, use the **$select** query parameter. The following are examples:</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/groups/c28c1cc9-e1ab-4c4d-98d1-d8fdf128b60f?$select=allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount

GET https://graph.microsoft.com/v1.0/groups/c28c1cc9-e1ab-4c4d-98d1-d8fdf128b60f?$select=description,allowExternalSenders
```


## <a name="prerequisites"></a><span data-ttu-id="6bfd9-126">前提条件</span><span class="sxs-lookup"><span data-stu-id="6bfd9-126">Prerequisites</span></span>
<span data-ttu-id="6bfd9-127">この API を実行するには、以下のいずれかの**スコープ**が必要です。*Group.Read.All* または *Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="6bfd9-127">One of the following **scopes** is required to execute this API: *Group.Read.All* or *Group.ReadWrite.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="6bfd9-128">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6bfd9-128">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6bfd9-129">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="6bfd9-129">Optional query parameters</span></span>
<span data-ttu-id="6bfd9-130">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="6bfd9-130">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6bfd9-131">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6bfd9-131">Request headers</span></span>
| <span data-ttu-id="6bfd9-132">名前</span><span class="sxs-lookup"><span data-stu-id="6bfd9-132">Name</span></span>       | <span data-ttu-id="6bfd9-133">型</span><span class="sxs-lookup"><span data-stu-id="6bfd9-133">Type</span></span> | <span data-ttu-id="6bfd9-134">説明</span><span class="sxs-lookup"><span data-stu-id="6bfd9-134">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6bfd9-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="6bfd9-135">Authorization</span></span>  | <span data-ttu-id="6bfd9-136">string</span><span class="sxs-lookup"><span data-stu-id="6bfd9-136">string</span></span>  | <span data-ttu-id="6bfd9-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6bfd9-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6bfd9-139">要求本文</span><span class="sxs-lookup"><span data-stu-id="6bfd9-139">Request body</span></span>
<span data-ttu-id="6bfd9-140">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6bfd9-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6bfd9-141">応答</span><span class="sxs-lookup"><span data-stu-id="6bfd9-141">Response</span></span>

<span data-ttu-id="6bfd9-142">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[グループ](../resources/group.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6bfd9-142">If successful, this method returns a `200 OK` response code and [group](../resources/group.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6bfd9-143">例</span><span class="sxs-lookup"><span data-stu-id="6bfd9-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6bfd9-144">要求</span><span class="sxs-lookup"><span data-stu-id="6bfd9-144">Request</span></span>
<span data-ttu-id="6bfd9-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6bfd9-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}
```
##### <a name="response"></a><span data-ttu-id="6bfd9-146">応答</span><span class="sxs-lookup"><span data-stu-id="6bfd9-146">Response</span></span>
<span data-ttu-id="6bfd9-147">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="6bfd9-147">Here is an example of the response.</span></span>

<span data-ttu-id="6bfd9-p104">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。実際の呼び出しでは、上で示すように既定のプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="6bfd9-p104">Note: The response object shown here may be truncated for brevity. The default properties will be returned from an actual call, as described above.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx

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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
