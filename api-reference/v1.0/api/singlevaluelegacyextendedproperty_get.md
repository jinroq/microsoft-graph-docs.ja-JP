# <a name="get-singlevaluelegacyextendedproperty"></a><span data-ttu-id="91b13-101">singleValueLegacyExtendedProperty を取得する</span><span class="sxs-lookup"><span data-stu-id="91b13-101">Get singleValueLegacyExtendedProperty</span></span>

<span data-ttu-id="91b13-102">`$expand` または `$filter` を使用して、単一値の拡張プロパティを含むリソース インスタンスを取得します。</span><span class="sxs-lookup"><span data-stu-id="91b13-102">Get resource instances that contain a single-value extended property by using `$expand` or `$filter`.</span></span>

<span data-ttu-id="91b13-p101">クエリ パラメーター `$expand` を使用すると、指示された拡張プロパティで展開された特定のインスタンスを取得できます。これは、現時点で、拡張プロパティを表す [singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md) オブジェクトを取得する唯一の方法です。</span><span class="sxs-lookup"><span data-stu-id="91b13-p101">Using the query parameter `$expand` allows you to get the specified instance expanded with the indicated extended property. This is currently the only way to get the [singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md) object that represents an extended property.</span></span>

<span data-ttu-id="91b13-p102">クエリ パラメーター `$filter` を使用すると、**id** プロパティと **value** プロパティに対するフィルターと一致する拡張プロパティを持つ、指定したリソースのすべてのインスタンスを取得できます。フィルターは、サインインしているユーザーのメールボックス内のリソースのすべてのインスタンスに適用されます。</span><span class="sxs-lookup"><span data-stu-id="91b13-p102">Using the query parameter `$filter` allows you to get all the instances of the specified resource that have an extended property matching a filter on the **id** and **value** properties. The filter is applied to all instances of the resource in the signed-in user's mailbox.</span></span>

<span data-ttu-id="91b13-107">次のユーザー リソースがサポートされます。</span><span class="sxs-lookup"><span data-stu-id="91b13-107">The following user resources are supported:</span></span>

- [<span data-ttu-id="91b13-108">message</span><span class="sxs-lookup"><span data-stu-id="91b13-108">message</span></span>](../resources/message.md)
- [<span data-ttu-id="91b13-109">mailFolder</span><span class="sxs-lookup"><span data-stu-id="91b13-109">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="91b13-110">event</span><span class="sxs-lookup"><span data-stu-id="91b13-110">event</span></span>](../resources/event.md)
- [<span data-ttu-id="91b13-111">calendar</span><span class="sxs-lookup"><span data-stu-id="91b13-111">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="91b13-112">contact</span><span class="sxs-lookup"><span data-stu-id="91b13-112">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="91b13-113">contactFolder</span><span class="sxs-lookup"><span data-stu-id="91b13-113">contactFolder</span></span>](../resources/contactfolder.md) 

<span data-ttu-id="91b13-114">次のグループ リソースもサポートされます。</span><span class="sxs-lookup"><span data-stu-id="91b13-114">As well as the following group resources:</span></span>

- <span data-ttu-id="91b13-115">グループ [event](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="91b13-115">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="91b13-116">グループ [calendar](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="91b13-116">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="91b13-117">グループ [post](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="91b13-117">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="91b13-118">オープン拡張機能または拡張プロパティを使用するのに適した状況と、拡張プロパティを指定する方法の詳細については、「[拡張プロパティの概要](../resources/extended-properties-overview.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="91b13-118">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="91b13-119">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="91b13-119">Permissions</span></span>
<span data-ttu-id="91b13-p103">この API を呼び出すには、取得するリソースに応じて、以下のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="91b13-p103">One of the following permissions is required to call this API, depending on the resource you're getting. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

- <span data-ttu-id="91b13-122">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="91b13-122">Mail.Read</span></span>
- <span data-ttu-id="91b13-123">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="91b13-123">Calendars.Read</span></span>
- <span data-ttu-id="91b13-124">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="91b13-124">Contacts.Read</span></span>
- <span data-ttu-id="91b13-125">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="91b13-125">Group.Read.All</span></span> 

## <a name="http-request"></a><span data-ttu-id="91b13-126">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="91b13-126">HTTP request</span></span>

#### <a name="get-a-resource-instance-using-expand"></a><span data-ttu-id="91b13-127">`$expand` を使用してリソース インスタンスを取得する</span><span class="sxs-lookup"><span data-stu-id="91b13-127">GET a resource instance using `$expand`</span></span>
<span data-ttu-id="91b13-p104">**id** プロパティに対するフィルターと一致する拡張プロパティで展開された、リソース インスタンスを取得します。フィルター文字列内のスペース文字に [URL エンコード](http://www.w3schools.com/tags/ref_urlencode.asp)を適用していることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="91b13-p104">Get a resource instance expanded with the extended property which matches a filter on the **id** property. Make sure you apply [URL encoding](http://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the filter string.</span></span>

<span data-ttu-id="91b13-130">**message** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="91b13-130">Get a **message** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="91b13-131">**mailFolder** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="91b13-131">Get a **mailFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="91b13-132">**event** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="91b13-132">Get an **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="91b13-133">**calendar** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="91b13-133">Get a **calendar** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="91b13-134">**contact** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="91b13-134">Get a **contact** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="91b13-135">**contactFolder** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="91b13-135">Get a **contactFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="91b13-136">グループ **event** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="91b13-136">Get a group **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="91b13-137">グループ **post** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="91b13-137">Get a group **post** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

#### <a name="get-resource-instances-using-filter"></a><span data-ttu-id="91b13-138">`$filter` を使用してリソース インスタンスを取得する</span><span class="sxs-lookup"><span data-stu-id="91b13-138">GET resource instances using `$filter`</span></span>

<span data-ttu-id="91b13-p105">**id** プロパティと **value** プロパティに対するフィルターと一致する拡張プロパティを持つサポート対象リソースのインスタンスを取得します。フィルター文字列のスラッシュ文字とスペース文字に [URL エンコード](http://www.w3schools.com/tags/ref_urlencode.asp) を適用していることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="91b13-p105">Get instances of a supported resource that have the extended property matching a filter on the **id** and **value** properties. Make sure you apply [URL encoding](http://www.w3schools.com/tags/ref_urlencode.asp) to the following characters in the filter string - forward slash and space.</span></span>


<span data-ttu-id="91b13-141">**message** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="91b13-141">Get **message** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="91b13-142">**mailFolder** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="91b13-142">Get **mailFolder** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="91b13-143">**event** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="91b13-143">Get **event** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="91b13-144">**calendar** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="91b13-144">Get **calendar** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="91b13-145">**contact** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="91b13-145">Get **contact** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="91b13-146">**contactFolder** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="91b13-146">Get **contactFolder** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="91b13-147">グループ **event** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="91b13-147">Get group **event** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="91b13-148">グループ **post** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="91b13-148">Get group **post** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

## <a name="parameters"></a><span data-ttu-id="91b13-149">パラメーター</span><span class="sxs-lookup"><span data-stu-id="91b13-149">Parameters</span></span>
|<span data-ttu-id="91b13-150">**パラメーター**</span><span class="sxs-lookup"><span data-stu-id="91b13-150">**Parameter**</span></span>|<span data-ttu-id="91b13-151">**型**</span><span class="sxs-lookup"><span data-stu-id="91b13-151">**Type**</span></span>|<span data-ttu-id="91b13-152">**説明**</span><span class="sxs-lookup"><span data-stu-id="91b13-152">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="91b13-153">_URL parameters_</span><span class="sxs-lookup"><span data-stu-id="91b13-153">_URL parameters_</span></span>|
|<span data-ttu-id="91b13-154">id_value</span><span class="sxs-lookup"><span data-stu-id="91b13-154">id_value</span></span>|<span data-ttu-id="91b13-155">String</span><span class="sxs-lookup"><span data-stu-id="91b13-155">String</span></span>|<span data-ttu-id="91b13-p106">照合する拡張プロパティの ID。サポートされている形式のいずれかに従う必要があります。詳しくは、「[Outlook の拡張プロパティの概要](../resources/extended-properties-overview.md)」を参照してください。必須。</span><span class="sxs-lookup"><span data-stu-id="91b13-p106">The ID of the extended property to match. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|
|<span data-ttu-id="91b13-160">property_value</span><span class="sxs-lookup"><span data-stu-id="91b13-160">property_value</span></span>|<span data-ttu-id="91b13-161">String</span><span class="sxs-lookup"><span data-stu-id="91b13-161">String</span></span>|<span data-ttu-id="91b13-p107">照合する拡張プロパティの値。前述の「**HTTP 要求**」セクションに示した一覧で必要になります。</span><span class="sxs-lookup"><span data-stu-id="91b13-p107">The value of the extended property to match. Required where listed in the **HTTP request** section above.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="91b13-164">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="91b13-164">Request headers</span></span>
| <span data-ttu-id="91b13-165">名前</span><span class="sxs-lookup"><span data-stu-id="91b13-165">Name</span></span>      |<span data-ttu-id="91b13-166">説明</span><span class="sxs-lookup"><span data-stu-id="91b13-166">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="91b13-167">Authorization</span><span class="sxs-lookup"><span data-stu-id="91b13-167">Authorization</span></span>  | <span data-ttu-id="91b13-p108">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="91b13-p108">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="91b13-170">要求本文</span><span class="sxs-lookup"><span data-stu-id="91b13-170">Request body</span></span>
<span data-ttu-id="91b13-171">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="91b13-171">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="91b13-172">応答</span><span class="sxs-lookup"><span data-stu-id="91b13-172">Response</span></span>

<span data-ttu-id="91b13-173">成功した場合、このメソッドは `200 OK` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="91b13-173">If successful, this method returns a `200 OK` response code.</span></span>

#### <a name="get-resource-instance-using-expand"></a><span data-ttu-id="91b13-174">`$expand` を使用してリソース インスタンスを取得する</span><span class="sxs-lookup"><span data-stu-id="91b13-174">GET resource instance using `$expand`</span></span>
<span data-ttu-id="91b13-175">応答本文には、一致する [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) オブジェクトで展開された、要求したリソース インスタンスで表されるオブジェクトが含まれます。</span><span class="sxs-lookup"><span data-stu-id="91b13-175">The response body includes an object representing the requested resource instance, expanded with the matching [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object.</span></span>
  
#### <a name="get-resource-instances-using-filter"></a><span data-ttu-id="91b13-176">`$filter` を使用してリソース インスタンスを取得する</span><span class="sxs-lookup"><span data-stu-id="91b13-176">GET resource instances using `$filter`</span></span>
<span data-ttu-id="91b13-p109">応答本文には、一致する拡張プロパティを含むリソース インスタンスを表す 1 つ以上のオブジェクトが含まれます。応答本文には、拡張プロパティは含まれません。</span><span class="sxs-lookup"><span data-stu-id="91b13-p109">The response body includes one or more objects representing the resource instances that contain the matching extended property. The response body does not include the extended property.</span></span>

## <a name="example"></a><span data-ttu-id="91b13-179">例</span><span class="sxs-lookup"><span data-stu-id="91b13-179">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="91b13-180">要求 1</span><span class="sxs-lookup"><span data-stu-id="91b13-180">Request 1</span></span>

<span data-ttu-id="91b13-p110">最初の例では、単一値の拡張プロパティを含めることによって指定されたメッセージを取得して展開します。フィルターは、**id** が文字列 `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` と一致する拡張プロパティを返します (ここでは、読みやすくするため URL エンコードを削除しています)。</span><span class="sxs-lookup"><span data-stu-id="91b13-p110">The first example gets and expands the specified message by including a single-value extended property. The filter returns the extended property that has its **id** matching the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

<!-- {
  "blockType": "request",
  "name": "get_singlevaluelegacyextendedproperty_1"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages('AAMkAGE1M2_bs88AACHsLqWAAA=')?$expand=singleValueExtendedProperties($filter=id%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color')
```
##### <a name="response-1"></a><span data-ttu-id="91b13-183">応答 1</span><span class="sxs-lookup"><span data-stu-id="91b13-183">Response 1</span></span>
<span data-ttu-id="91b13-184">応答本文には、指定されたメッセージのすべてのプロパティと、フィルターから返される拡張プロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="91b13-184">The response body includes all the properties of the specified message and extended property returned from the filter.</span></span>

<span data-ttu-id="91b13-p111">注:簡潔にするために、ここに示す**メッセージ** オブジェクトは切り詰められています。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="91b13-p111">Note: The **message** object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages/$entity",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfcd489-628b-40d7-b48b-57002df800e5@1717622f-1d94-4d0c-9d74-709fad664b77')/messages('AAMkAGE1M2_bs88AACHsLqWAAA=')",
    "@odata.etag": "W/\"CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AACbyS4H\"",
    "id": "AAMkAGE1M2_bs88AACHsLqWAAA=",
    "subject": "RE: Talk about emergency prep",
    "sender": {
        "emailAddress": {
            "name": "Christine Irwin",
            "address": "christine@contoso.com"
        }
    },
    "from": null,
    "toRecipients": [
        {
            "emailAddress": {
                "name": "Christine Irwin",
                "address": "christine@contoso.com"
            }
        }
    ],
    "singleValueExtendedProperties@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages('AAMkAGE1M2_bs88AACHsLqWAAA%3D')/singleValueExtendedProperties",
    "singleValueExtendedProperties": [
        {
            "id": "String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color",
            "value": "Green"
        }
    ]
}
```

****

#### <a name="request-2"></a><span data-ttu-id="91b13-187">要求 2</span><span class="sxs-lookup"><span data-stu-id="91b13-187">Request 2</span></span>

<span data-ttu-id="91b13-p112">2 番目の例では、フィルターで指定された単一値の拡張プロパティを持つメッセージを取得します。フィルターは、次のものを持つ拡張のプロパティを返します。</span><span class="sxs-lookup"><span data-stu-id="91b13-p112">The second example gets messages that have the single-value extended property specified in the filter. The filter returns the extended property that has:</span></span>
- <span data-ttu-id="91b13-190">文字列 `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` と一致する **id** (ここでは、読みやすくするため URL エンコードを削除しています)。</span><span class="sxs-lookup"><span data-stu-id="91b13-190">Its **id** matching the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>
- <span data-ttu-id="91b13-191">**value** が `Green` であるもの。</span><span class="sxs-lookup"><span data-stu-id="91b13-191">Its **value** being `Green`.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/api/v1.0/Me/messages?$filter=singleValueExtendedProperties%2FAny(ep%3A%20ep%2Fid%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color'%20and%20ep%2Fvalue%20eq%20'Green')
```

##### <a name="response-2"></a><span data-ttu-id="91b13-192">応答 2</span><span class="sxs-lookup"><span data-stu-id="91b13-192">Response 2</span></span>

<span data-ttu-id="91b13-p113">正常な応答が `HTTP 200 OK` 応答コードによって示され、応答の本文には、フィルターに一致する拡張プロパティを持つメッセージのすべてのプロパティが含まれます。応答本文は、[メッセージのコレクションの取得](../api/user_list_messages.md)からの応答に似ています。応答は、一致する拡張プロパティを含みません。</span><span class="sxs-lookup"><span data-stu-id="91b13-p113">A successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the filter. The response body is similar to the response from [getting a message collection](../api/user_list_messages.md). The response does not include the matching extended property.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get singleValueLegacyExtendedProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->