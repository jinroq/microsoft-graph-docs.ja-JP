# <a name="get-group"></a><span data-ttu-id="1dcf5-101">グループを取得する</span><span class="sxs-lookup"><span data-stu-id="1dcf5-101">Get group</span></span>
<span data-ttu-id="1dcf5-102">グループ オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="1dcf5-102">Get the properties and relationships of a group object.</span></span>

##### <a name="default-properties"></a><span data-ttu-id="1dcf5-103">既定のプロパティ</span><span class="sxs-lookup"><span data-stu-id="1dcf5-103">Default properties</span></span>

<span data-ttu-id="1dcf5-p101">以下は、グループを取得または一覧表示するときに返されるプロパティの既定のセットを表します。これらは、利用可能なすべてのプロパティのサブセットです。</span><span class="sxs-lookup"><span data-stu-id="1dcf5-p101">The following represent the default set of properties that are returned when getting or listing groups. These are a subset of all available properties.</span></span> 

* <span data-ttu-id="1dcf5-106">description</span><span class="sxs-lookup"><span data-stu-id="1dcf5-106">description</span></span>
* <span data-ttu-id="1dcf5-107">displayName</span><span class="sxs-lookup"><span data-stu-id="1dcf5-107">displayName</span></span>
* <span data-ttu-id="1dcf5-108">groupTypes</span><span class="sxs-lookup"><span data-stu-id="1dcf5-108">groupTypes</span></span>
* <span data-ttu-id="1dcf5-109">id</span><span class="sxs-lookup"><span data-stu-id="1dcf5-109">id</span></span>
* <span data-ttu-id="1dcf5-110">mail</span><span class="sxs-lookup"><span data-stu-id="1dcf5-110">mail</span></span>
* <span data-ttu-id="1dcf5-111">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="1dcf5-111">mailEnabled</span></span>
* <span data-ttu-id="1dcf5-112">mailNickname</span><span class="sxs-lookup"><span data-stu-id="1dcf5-112">mailNickname</span></span>
* <span data-ttu-id="1dcf5-113">onPremisesLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="1dcf5-113">onPremisesLastSyncDateTime</span></span>
* <span data-ttu-id="1dcf5-114">onPremisesSecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="1dcf5-114">onPremisesSecurityIdentifier</span></span>
* <span data-ttu-id="1dcf5-115">onPremisesSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="1dcf5-115">onPremisesSyncEnabled</span></span>
* <span data-ttu-id="1dcf5-116">proxyAddresses</span><span class="sxs-lookup"><span data-stu-id="1dcf5-116">proxyAddresses</span></span>
* <span data-ttu-id="1dcf5-117">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="1dcf5-117">securityEnabled</span></span>
* <span data-ttu-id="1dcf5-118">visibility</span><span class="sxs-lookup"><span data-stu-id="1dcf5-118">visibility</span></span>

<span data-ttu-id="1dcf5-119">次のグループ プロパティは既定では返されません。</span><span class="sxs-lookup"><span data-stu-id="1dcf5-119">The following group properties are not returned by default:</span></span>

* <span data-ttu-id="1dcf5-120">allowExternalSenders</span><span class="sxs-lookup"><span data-stu-id="1dcf5-120">allowExternalSenders</span></span>
* <span data-ttu-id="1dcf5-121">autoSubscribeNewMembers</span><span class="sxs-lookup"><span data-stu-id="1dcf5-121">autoSubscribeNewMembers</span></span>
* <span data-ttu-id="1dcf5-122">isSubscribedByMail</span><span class="sxs-lookup"><span data-stu-id="1dcf5-122">isSubscribedByMail</span></span>
* <span data-ttu-id="1dcf5-123">unseenCount</span><span class="sxs-lookup"><span data-stu-id="1dcf5-123">unseenCount</span></span>

<span data-ttu-id="1dcf5-p102">これらのプロパティを取得するには、**$select** クエリ パラメーターを使用します。次に、例を示します。</span><span class="sxs-lookup"><span data-stu-id="1dcf5-p102">To get these properties, use the **$select** query parameter. The following are examples:</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/groups/c28c1cc9-e1ab-4c4d-98d1-d8fdf128b60f?$select=allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount

GET https://graph.microsoft.com/v1.0/groups/c28c1cc9-e1ab-4c4d-98d1-d8fdf128b60f?$select=description,allowExternalSenders
```


## <a name="permissions"></a><span data-ttu-id="1dcf5-126">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1dcf5-126">Permissions</span></span>
<span data-ttu-id="1dcf5-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1dcf5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1dcf5-129">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1dcf5-129">Permission type</span></span>      | <span data-ttu-id="1dcf5-130">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1dcf5-130">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1dcf5-131">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1dcf5-131">Delegated (work or school account)</span></span> | <span data-ttu-id="1dcf5-132">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1dcf5-132">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1dcf5-133">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1dcf5-133">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1dcf5-134">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1dcf5-134">Not supported.</span></span>    |
|<span data-ttu-id="1dcf5-135">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1dcf5-135">Application</span></span> | <span data-ttu-id="1dcf5-136">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1dcf5-136">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1dcf5-137">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1dcf5-137">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1dcf5-138">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="1dcf5-138">Optional query parameters</span></span>
<span data-ttu-id="1dcf5-139">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](../../../concepts/query_parameters.md)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="1dcf5-139">This method supports the [OData Query Parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1dcf5-140">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1dcf5-140">Request headers</span></span>
| <span data-ttu-id="1dcf5-141">名前</span><span class="sxs-lookup"><span data-stu-id="1dcf5-141">Name</span></span>       | <span data-ttu-id="1dcf5-142">型</span><span class="sxs-lookup"><span data-stu-id="1dcf5-142">Type</span></span> | <span data-ttu-id="1dcf5-143">説明</span><span class="sxs-lookup"><span data-stu-id="1dcf5-143">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1dcf5-144">Authorization</span><span class="sxs-lookup"><span data-stu-id="1dcf5-144">Authorization</span></span>  | <span data-ttu-id="1dcf5-145">string</span><span class="sxs-lookup"><span data-stu-id="1dcf5-145">string</span></span>  | <span data-ttu-id="1dcf5-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1dcf5-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1dcf5-148">要求本文</span><span class="sxs-lookup"><span data-stu-id="1dcf5-148">Request body</span></span>
<span data-ttu-id="1dcf5-149">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1dcf5-149">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1dcf5-150">応答</span><span class="sxs-lookup"><span data-stu-id="1dcf5-150">Response</span></span>
<span data-ttu-id="1dcf5-151">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[グループ](../resources/group.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1dcf5-151">If successful, this method returns a `200 OK` response code and [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1dcf5-152">例</span><span class="sxs-lookup"><span data-stu-id="1dcf5-152">Example</span></span>
#### <a name="request"></a><span data-ttu-id="1dcf5-153">要求</span><span class="sxs-lookup"><span data-stu-id="1dcf5-153">Request</span></span>
<span data-ttu-id="1dcf5-154">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1dcf5-154">The following is an example of the request body.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}
```

#### <a name="response"></a><span data-ttu-id="1dcf5-155">応答</span><span class="sxs-lookup"><span data-stu-id="1dcf5-155">Response</span></span>
<span data-ttu-id="1dcf5-156">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1dcf5-156">The following is an example of a response.</span></span>

><span data-ttu-id="1dcf5-157">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="1dcf5-157">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1dcf5-158">実際の呼び出しでは、前に示したように既定のプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="1dcf5-158">Note: The response object shown here may be truncated for brevity. The default properties will be returned from an actual call, as described above.</span></span>
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
