# <a name="get-singlevaluelegacyextendedproperty"></a><span data-ttu-id="8f250-101">singleValueLegacyExtendedProperty を取得する</span><span class="sxs-lookup"><span data-stu-id="8f250-101">Get singleValueLegacyExtendedProperty</span></span>

<span data-ttu-id="8f250-102">特定の拡張プロパティで展開された単一のリソース インスタンス、または 1 つのフィルターと一致する拡張プロパティを含むリソース インスタンスのコレクションを取得できます。</span><span class="sxs-lookup"><span data-stu-id="8f250-102">You can get a single resource instance expanded with a specific extended property, or a collection of resource instances that include extended properties matching a filter.</span></span>

<span data-ttu-id="8f250-103">クエリ パラメーター `$expand` を使用すると、指定した拡張プロパティで展開された特定のリソース インスタンスを取得できます。</span><span class="sxs-lookup"><span data-stu-id="8f250-103">Using the query parameter `$expand` allows you to get the specified instance expanded with the indicated extended property.</span></span> <span data-ttu-id="8f250-104">**id** プロパティ上で `$filter` および `eq` 演算子を使用して拡張プロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="8f250-104">Use a `$filter` and `eq` operator on the **id** property to specify the extended property.</span></span> <span data-ttu-id="8f250-105">これは、現時点で、拡張プロパティを表す [singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md) オブジェクトを取得する唯一の方法です。</span><span class="sxs-lookup"><span data-stu-id="8f250-105">This is currently the only way to get the [multiValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md) object that represents an extended property.</span></span> 

<span data-ttu-id="8f250-106">特定の拡張プロパティを含むリソース インスタンスを取得するには、`$filter` クエリ パラメーターを使用して、`eq` 演算子を **id** プロパティに適用します。</span><span class="sxs-lookup"><span data-stu-id="8f250-106">To get resource instances that have certain extended properties, use the `$filter` query parameter and apply an `eq` operator on the **id** property.</span></span> <span data-ttu-id="8f250-107">さらに、数値の拡張プロパティについては、**value** プロパティで `eq`、`ne`、`ge`、`gt`、`le`、`lt` 演算子のいずれかを適用します。</span><span class="sxs-lookup"><span data-stu-id="8f250-107">In addition, for numeric extended properties, apply one of the following operators on the **value** property: `eq`, `ne`,`ge`, `gt`, `le`, or `lt`.</span></span> <span data-ttu-id="8f250-108">文字列型の拡張プロパティについては、`contains`、`startswith`、`eq`、`ne` 演算子を **value** に適用します。</span><span class="sxs-lookup"><span data-stu-id="8f250-108">For string-typed extended properties, apply a `contains`, `startswith`, `eq`, or `ne` operator on **value**.</span></span>

<span data-ttu-id="8f250-109">フィルターは、サインインしているユーザーのメールボックスにあるリソースのインスタンスすべてに適用されます。</span><span class="sxs-lookup"><span data-stu-id="8f250-109">The filter is applied to all instances of the resource in the signed-in user's mailbox.</span></span> 

<span data-ttu-id="8f250-110">拡張プロパティの **id** で文字列名 (`Name`) をフィルタリングする場合は、大文字と小文字が区別されます。</span><span class="sxs-lookup"><span data-stu-id="8f250-110">Filtering the string name (`Name`) in the **id** of an extended property is case-sensitive.</span></span> <span data-ttu-id="8f250-111">拡張プロパティの **value** プロパティをフィルタリングする場合は、大文字と小文字が区別されません。</span><span class="sxs-lookup"><span data-stu-id="8f250-111">Filtering the **value** property of an extended property is case-insensitive.</span></span>

<span data-ttu-id="8f250-112">次のユーザー リソースがサポートされます。</span><span class="sxs-lookup"><span data-stu-id="8f250-112">The following user resources are supported:</span></span>

- [<span data-ttu-id="8f250-113">message</span><span class="sxs-lookup"><span data-stu-id="8f250-113">message</span></span>](../resources/message.md)
- [<span data-ttu-id="8f250-114">mailFolder</span><span class="sxs-lookup"><span data-stu-id="8f250-114">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="8f250-115">event</span><span class="sxs-lookup"><span data-stu-id="8f250-115">event</span></span>](../resources/event.md)
- [<span data-ttu-id="8f250-116">calendar</span><span class="sxs-lookup"><span data-stu-id="8f250-116">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="8f250-117">contact</span><span class="sxs-lookup"><span data-stu-id="8f250-117">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="8f250-118">contactFolder</span><span class="sxs-lookup"><span data-stu-id="8f250-118">contactFolder</span></span>](../resources/contactfolder.md) 

<span data-ttu-id="8f250-119">次のグループ リソースもサポートされます。</span><span class="sxs-lookup"><span data-stu-id="8f250-119">As well as the following group resources:</span></span>

- <span data-ttu-id="8f250-120">グループ [event](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="8f250-120">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="8f250-121">グループ [calendar](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="8f250-121">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="8f250-122">グループ [post](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="8f250-122">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="8f250-123">オープン拡張機能または拡張プロパティを使用するのに適した状況と、拡張プロパティを指定する方法の詳細については、「[拡張プロパティの概要](../resources/extended-properties-overview.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8f250-123">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="8f250-124">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8f250-124">Permissions</span></span>
<span data-ttu-id="8f250-p104">この API を呼び出すには、取得するリソースに応じて、以下のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8f250-p104">One of the following permissions is required to call this API, depending on the resource you're getting. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

- <span data-ttu-id="8f250-127">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="8f250-127">Mail.Read</span></span>
- <span data-ttu-id="8f250-128">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="8f250-128">Calendars.Read</span></span>
- <span data-ttu-id="8f250-129">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="8f250-129">Contacts.Read</span></span>
- <span data-ttu-id="8f250-130">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="8f250-130">Group.Read.All</span></span> 

## <a name="http-request"></a><span data-ttu-id="8f250-131">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8f250-131">HTTP request</span></span>

#### <a name="get-a-resource-instance-expanded-with-an-extended-property-that-matches-a-filter"></a><span data-ttu-id="8f250-132">フィルターと一致する拡張プロパティで展開されたリソース インスタンスを取得する</span><span class="sxs-lookup"><span data-stu-id="8f250-132">GET a resource instance expanded with an extended property that matches a filter</span></span>
<span data-ttu-id="8f250-p105">**id** プロパティに対するフィルターと一致する拡張プロパティで展開された、リソース インスタンスを取得します。フィルター文字列内のスペース文字に [URL エンコード](http://www.w3schools.com/tags/ref_urlencode.asp)を適用していることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="8f250-p105">Get a resource instance expanded with the extended property which matches a filter on the **id** property. Make sure you apply [URL encoding](http://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the filter string.</span></span>

<span data-ttu-id="8f250-135">**message** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="8f250-135">Get a **message** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="8f250-136">**mailFolder** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="8f250-136">Get a **mailFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="8f250-137">**event** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="8f250-137">Get an **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="8f250-138">**calendar** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="8f250-138">Get a **calendar** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="8f250-139">**contact** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="8f250-139">Get a **contact** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="8f250-140">**contactFolder** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="8f250-140">Get a **contactFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="8f250-141">グループ **event** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="8f250-141">Get a group **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="8f250-142">グループ **post** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="8f250-142">Get a group **post** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

#### <a name="get-resource-instances-that-include-numeric-extended-properties-matching-a-filter"></a><span data-ttu-id="8f250-143">フィルターと一致する数値の拡張プロパティを含むリソース インスタンスを取得する</span><span class="sxs-lookup"><span data-stu-id="8f250-143">GET resource instances that include numeric extended properties matching a filter</span></span>

<span data-ttu-id="8f250-144">フィルターと一致する数値の拡張プロパティを持つサポート対象リソースのインスタンスを取得します。</span><span class="sxs-lookup"><span data-stu-id="8f250-144">Get instances of a supported resource that have the extended property matching a filter on the id and value properties.</span></span> <span data-ttu-id="8f250-145">フィルターは **id** プロパティには `eq` 演算子を使用し、**value** プロパティには `eq`、`ne`、`ge`、`gt`、`le`、`lt` のいずれかの演算子を使用します。</span><span class="sxs-lookup"><span data-stu-id="8f250-145">The filter uses an `eq` operator on the **id** property, and one of the following operators on the **value** property: `eq`, `ne`,`ge`, `gt`, `le`, or `lt`.</span></span> <span data-ttu-id="8f250-146">フィルター文字列内のコロン、スラッシュ、スペースに [URL エンコード](http://www.w3schools.com/tags/ref_urlencode.asp)を適用していることをご確認ください。</span><span class="sxs-lookup"><span data-stu-id="8f250-146">Make sure you apply [URL encoding](http://www.w3schools.com/tags/ref_urlencode.asp) to the following characters in the filter string - colon, forward slash, and space.</span></span>

<span data-ttu-id="8f250-147">次の構文の行では、id に `eq` 演算子を使用し、プロパティ値にもう 1 つの `eq` 演算子を使用するフィルターを示しています。</span><span class="sxs-lookup"><span data-stu-id="8f250-147">The following syntax lines show a filter that uses an `eq` operator on the id, and another `eq` operator on the property value.</span></span> <span data-ttu-id="8f250-148">**value** に対する `eq` 演算子は、数値に適用される別の演算子 (`ne`、`ge`、`gt`、`le`、`lt`) のいずれかと置き換えることができます。</span><span class="sxs-lookup"><span data-stu-id="8f250-148">You can substitute the `eq` operator on the **value** by any one of the other operators (`ne`,`ge`, `gt`, `le`, or `lt`) that apply to numeric values.</span></span>

<span data-ttu-id="8f250-149">**message** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="8f250-149">Get **message** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="8f250-150">**mailFolder** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="8f250-150">Get **mailFolder** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="8f250-151">**event** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="8f250-151">Get **event** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="8f250-152">**calendar** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="8f250-152">Get **calendar** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="8f250-153">**contact** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="8f250-153">Get **contact** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="8f250-154">**contactFolder** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="8f250-154">Get **contactFolder** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="8f250-155">グループ **event** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="8f250-155">Get group **event** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="8f250-156">グループ **post** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="8f250-156">Get group **post** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

#### <a name="get-resource-instances-with-string-typed-extended-properties-matching-a-filter"></a><span data-ttu-id="8f250-157">フィルターと一致する文字列型の拡張プロパティを含むリソース インスタンスを取得する</span><span class="sxs-lookup"><span data-stu-id="8f250-157">GET resource instances with string-typed extended properties matching a filter</span></span>

<span data-ttu-id="8f250-158">フィルターと一致する文字列型の拡張プロパティを含む **message** または **event** リソースのインスタンスを取得します。</span><span class="sxs-lookup"><span data-stu-id="8f250-158">Get instances of the **message** or **event** resource that have a string-typed extended property matching a filter.</span></span> <span data-ttu-id="8f250-159">フィルターは **id** プロパティには `eq` 演算子を使用し、**value** プロパティには `contains`、`startswith`、`eq`、`ne` のいずれかの演算子を使用します。</span><span class="sxs-lookup"><span data-stu-id="8f250-159">The filter uses an `eq` operator on the **id** property, and one of the following operators on the **value** property: `contains`, `startswith`, `eq`, or `ne`.</span></span> <span data-ttu-id="8f250-160">フィルター文字列内のコロン、スラッシュ、スペースに [URL エンコード](http://www.w3schools.com/tags/ref_urlencode.asp)を適用していることをご確認ください。</span><span class="sxs-lookup"><span data-stu-id="8f250-160">Make sure you apply [URL encoding](http://www.w3schools.com/tags/ref_urlencode.asp) to the following characters in the filter string - colon, forward slash, and space.</span></span>


<span data-ttu-id="8f250-161">**message** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="8f250-161">Get **message** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))

GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))

GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')

GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
```

<span data-ttu-id="8f250-162">**event** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="8f250-162">Get **event** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))

GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))

GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')

GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
```

<span data-ttu-id="8f250-163">グループ **event** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="8f250-163">Get group **event** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
```


## <a name="parameters"></a><span data-ttu-id="8f250-164">パラメーター</span><span class="sxs-lookup"><span data-stu-id="8f250-164">Parameters</span></span>
|<span data-ttu-id="8f250-165">**パラメーター**</span><span class="sxs-lookup"><span data-stu-id="8f250-165">**Parameter**</span></span>|<span data-ttu-id="8f250-166">**型**</span><span class="sxs-lookup"><span data-stu-id="8f250-166">**Type**</span></span>|<span data-ttu-id="8f250-167">**説明**</span><span class="sxs-lookup"><span data-stu-id="8f250-167">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="8f250-168">_URL parameters_</span><span class="sxs-lookup"><span data-stu-id="8f250-168">_URL parameters_</span></span>|
|<span data-ttu-id="8f250-169">id_value</span><span class="sxs-lookup"><span data-stu-id="8f250-169">id_value</span></span>|<span data-ttu-id="8f250-170">String</span><span class="sxs-lookup"><span data-stu-id="8f250-170">String</span></span>|<span data-ttu-id="8f250-p109">照合する拡張プロパティの ID。サポートされている形式のいずれかに従う必要があります。詳しくは、「[Outlook の拡張プロパティの概要](../resources/extended-properties-overview.md)」を参照してください。必須。</span><span class="sxs-lookup"><span data-stu-id="8f250-p109">The ID of the extended property to match. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|
|<span data-ttu-id="8f250-175">property_value</span><span class="sxs-lookup"><span data-stu-id="8f250-175">property_value</span></span> |<span data-ttu-id="8f250-176">文字列</span><span class="sxs-lookup"><span data-stu-id="8f250-176">String</span></span>|<span data-ttu-id="8f250-177">照合する拡張プロパティの値。</span><span class="sxs-lookup"><span data-stu-id="8f250-177">The value of the extended property to match.</span></span> <span data-ttu-id="8f250-178">前述の「**HTTP 要求**」セクションに示した一覧で必要になります。</span><span class="sxs-lookup"><span data-stu-id="8f250-178">Required where listed in the **HTTP request** section above.</span></span> <span data-ttu-id="8f250-179">{property_value} が文字列ではない場合、`ep/value` を {property_value} と比較するときに、適切な Edm データ型に明示的にキャストしてください。</span><span class="sxs-lookup"><span data-stu-id="8f250-179">If {property_value} is not a string, make sure you explicitly cast `ep/value` to the appropriate Edm data type when comparing it with {property_value}.</span></span> <span data-ttu-id="8f250-180">例については、以下の[要求 4](#request-4) を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8f250-180">See [request 3](#request-4) below for examples.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="8f250-181">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8f250-181">Request headers</span></span>
| <span data-ttu-id="8f250-182">名前</span><span class="sxs-lookup"><span data-stu-id="8f250-182">Name</span></span>      |<span data-ttu-id="8f250-183">説明</span><span class="sxs-lookup"><span data-stu-id="8f250-183">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8f250-184">Authorization</span><span class="sxs-lookup"><span data-stu-id="8f250-184">Authorization</span></span>  | <span data-ttu-id="8f250-p111">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8f250-p111">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8f250-187">要求本文</span><span class="sxs-lookup"><span data-stu-id="8f250-187">Request body</span></span>
<span data-ttu-id="8f250-188">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="8f250-188">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8f250-189">応答</span><span class="sxs-lookup"><span data-stu-id="8f250-189">Response</span></span>

<span data-ttu-id="8f250-190">成功した場合、このメソッドは `200 OK` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="8f250-190">If successful, this method returns a `200 OK` response code.</span></span>

#### <a name="get-resource-instance-expanded-with-a-matching-extended-property"></a><span data-ttu-id="8f250-191">一致する拡張プロパティで展開されたリソース インスタンスを取得する</span><span class="sxs-lookup"><span data-stu-id="8f250-191">GET resource instance expanded with a matching extended property</span></span>
<span data-ttu-id="8f250-192">応答本文には、一致する [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) オブジェクトで展開された、要求したリソース インスタンスで表されるオブジェクトが含まれます。</span><span class="sxs-lookup"><span data-stu-id="8f250-192">The response body includes an object representing the requested resource instance, expanded with the matching [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object.</span></span>
  
#### <a name="get-resource-instances-that-contain-an-extended-property-matching-a-filter"></a><span data-ttu-id="8f250-193">フィルターと一致する拡張プロパティを含むリソース インスタンスを取得する</span><span class="sxs-lookup"><span data-stu-id="8f250-193">GET resource instances that contain an extended property matching a filter</span></span>
<span data-ttu-id="8f250-194">応答本文には、一致する拡張プロパティを含むリソース インスタンスを表す 1 つ以上のオブジェクトが含まれます。</span><span class="sxs-lookup"><span data-stu-id="8f250-194">The response body includes one or more objects representing the resource instances that contain the matching extended property. The response body does not include the extended property.</span></span> <span data-ttu-id="8f250-195">応答本文には、拡張プロパティは含まれません。</span><span class="sxs-lookup"><span data-stu-id="8f250-195">The response does not include the matching extended property.</span></span>

## <a name="example"></a><span data-ttu-id="8f250-196">例</span><span class="sxs-lookup"><span data-stu-id="8f250-196">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="8f250-197">要求 1</span><span class="sxs-lookup"><span data-stu-id="8f250-197">Request 1</span></span>

<span data-ttu-id="8f250-p113">最初の例では、単一値の拡張プロパティを含めることによって指定されたメッセージを取得して展開します。フィルターは、**id** が文字列 `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` と一致する拡張プロパティを返します (ここでは、読みやすくするため URL エンコードを削除しています)。</span><span class="sxs-lookup"><span data-stu-id="8f250-p113">The first example gets and expands the specified message by including a single-value extended property. The filter returns the extended property that has its **id** matching the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

<!-- {
  "blockType": "request",
  "name": "get_singlevaluelegacyextendedproperty_1"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages('AAMkAGE1M2_bs88AACHsLqWAAA=')?$expand=singleValueExtendedProperties($filter=id%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color')
```
#### <a name="response-1"></a><span data-ttu-id="8f250-200">応答 1</span><span class="sxs-lookup"><span data-stu-id="8f250-200">Response 1</span></span>
<span data-ttu-id="8f250-201">応答本文には、指定されたメッセージのすべてのプロパティと、フィルターから返される拡張プロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="8f250-201">The response body includes all the properties of the specified message and extended property returned from the filter.</span></span>

<span data-ttu-id="8f250-p114">注:簡潔にするために、ここに示す**メッセージ** オブジェクトは切り詰められています。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8f250-p114">Note: The **message** object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

#### <a name="request-2"></a><span data-ttu-id="8f250-204">要求 2</span><span class="sxs-lookup"><span data-stu-id="8f250-204">Request 2</span></span>

<span data-ttu-id="8f250-205">2 番目の例では、文字列で型指定され、フィルターで指定された単一値の拡張プロパティを持つメッセージを取得します。</span><span class="sxs-lookup"><span data-stu-id="8f250-205">The second example gets messages that have the string-typed single-value extended property specified in the filter.</span></span> <span data-ttu-id="8f250-206">フィルターは、以下のような拡張プロパティを検索します。</span><span class="sxs-lookup"><span data-stu-id="8f250-206">The filter looks for the extended property that has:</span></span>

- <span data-ttu-id="8f250-207">その **id** は文字列 `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` と一致します (ここでは、読みやすくするため URL エンコードを削除しています)。</span><span class="sxs-lookup"><span data-stu-id="8f250-207">Its **id** matching the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

- <span data-ttu-id="8f250-208">その **value** は文字列 `Green` と一致します。</span><span class="sxs-lookup"><span data-stu-id="8f250-208">Its value equal to the integer 12.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=singleValueExtendedProperties%2FAny(ep%3A%20ep%2Fid%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color'%20and%20ep%2Fvalue%20eq%20'Green')
```

#### <a name="response-2"></a><span data-ttu-id="8f250-209">応答 2</span><span class="sxs-lookup"><span data-stu-id="8f250-209">Response 2</span></span>

<span data-ttu-id="8f250-p116">正常な応答が `HTTP 200 OK` 応答コードによって示され、応答の本文には、フィルターに一致する拡張プロパティを持つメッセージのすべてのプロパティが含まれます。応答本文は、[メッセージのコレクションの取得](../api/user_list_messages.md)からの応答に似ています。応答は、一致する拡張プロパティを含みません。</span><span class="sxs-lookup"><span data-stu-id="8f250-p116">A successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the filter. The response body is similar to the response from [getting a message collection](../api/user_list_messages.md). The response does not include the matching extended property.</span></span>


#### <a name="request-3"></a><span data-ttu-id="8f250-213">要求 3</span><span class="sxs-lookup"><span data-stu-id="8f250-213">Request 3</span></span>

<span data-ttu-id="8f250-214">3 番目の例では、文字列で型指定され、フィルターで指定された単一値の拡張プロパティを持つメッセージを取得します。</span><span class="sxs-lookup"><span data-stu-id="8f250-214">The second example gets messages that have the string-typed single-value extended property specified in the filter.</span></span> <span data-ttu-id="8f250-215">フィルターは、以下のような拡張プロパティを検索します。</span><span class="sxs-lookup"><span data-stu-id="8f250-215">The filter looks for the extended property that has:</span></span>

- <span data-ttu-id="8f250-216">その **id** は文字列 `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` と一致します (ここでは、読みやすくするため URL エンコードを削除しています)。</span><span class="sxs-lookup"><span data-stu-id="8f250-216">Its **id** matching the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

- <span data-ttu-id="8f250-217">その **value** には文字列 `green` が含まれます。</span><span class="sxs-lookup"><span data-stu-id="8f250-217">Its **value** being the string `green`.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/Me/messages?$filter=singleValueExtendedProperties/any(ep:ep/Id eq 'String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color' and contains(ep/Value, 'green'))
```

#### <a name="response-3"></a><span data-ttu-id="8f250-218">応答 3</span><span class="sxs-lookup"><span data-stu-id="8f250-218">Response 3</span></span>

<span data-ttu-id="8f250-219">正常な応答が `HTTP 200 OK` 応答コードによって示され、応答の本文には、フィルターに一致する拡張プロパティを持つメッセージのすべてのプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="8f250-219">A successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the filter.</span></span> <span data-ttu-id="8f250-220">たとえば、**id** が文字列 `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color`、**value** `Light green` と等しい単一値の拡張プロパティのあるメッセージがフィルターと一致し、応答に含まれるとします。</span><span class="sxs-lookup"><span data-stu-id="8f250-220">For example, a message that has a single-value extended property with the **id** equal to the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color`, and the **value** `Light green`, would match the filter and be included in the response.</span></span>

<span data-ttu-id="8f250-221">応答本文は、[メッセージのコレクションの取得](../api/user_list_messages.md)からの応答に似ています。</span><span class="sxs-lookup"><span data-stu-id="8f250-221">The response body is similar to the response from [getting a message collection](../api/user_list_messages.md).</span></span> <span data-ttu-id="8f250-222">応答は、一致する拡張プロパティを含みません。</span><span class="sxs-lookup"><span data-stu-id="8f250-222">The response does not include the matching extended property.</span></span>


#### <a name="request-4"></a><span data-ttu-id="8f250-223">要求 4</span><span class="sxs-lookup"><span data-stu-id="8f250-223">Request 4</span></span>

<span data-ttu-id="8f250-224">次の 2 つの例では、文字列以外で型指定された単一値の拡張プロパティを持つメッセージを取得する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="8f250-224">The next 2 examples show how to get messages that have non-string typed single-value extended properties.</span></span> <span data-ttu-id="8f250-225">読みやすくするため、必要な URL エンコードは含まれていません。</span><span class="sxs-lookup"><span data-stu-id="8f250-225">For ease of reading, they do not include the necessary URL encoding.</span></span>

<span data-ttu-id="8f250-226">次の例は、以下のような拡張プロパティを検索するフィルターを示しています。</span><span class="sxs-lookup"><span data-stu-id="8f250-226">The following example shows a filter that looks for the extended property that has:</span></span>

- <span data-ttu-id="8f250-227">その **id** は文字列 `CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid` と一致します。</span><span class="sxs-lookup"><span data-stu-id="8f250-227">Its **id** matching the string `CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid`.</span></span>

- <span data-ttu-id="8f250-228">その **value** は GUID `b9cf8971-7d55-4b73-9ffa-a584611b600b` です。</span><span class="sxs-lookup"><span data-stu-id="8f250-228">Its **value** being the GUID `b9cf8971-7d55-4b73-9ffa-a584611b600b`.</span></span> <span data-ttu-id="8f250-229">プロパティ値を GUID と比較するには、`ep/value` を `Edm.Guid` にキャストします。</span><span class="sxs-lookup"><span data-stu-id="8f250-229">To compare the property value with a GUID, cast `ep/value` to `Edm.Guid`.</span></span>


<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=singleValueExtendedProperties/any(ep:ep/id eq 'CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid' and cast(ep/value, Edm.Guid) eq (b9cf8971-7d55-4b73-9ffa-a584611b600b))
```

<span data-ttu-id="8f250-230">次の例は、以下のような拡張プロパティを検索するフィルターを示しています。</span><span class="sxs-lookup"><span data-stu-id="8f250-230">The next example shows a filter that looks for the extended property that has:</span></span>

- <span data-ttu-id="8f250-231">その **id** は文字列 `Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete` と一致します。</span><span class="sxs-lookup"><span data-stu-id="8f250-231">Its **id** matching the string `Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete`.</span></span>

- <span data-ttu-id="8f250-232">その **value** は整数 12 と等しくなります。</span><span class="sxs-lookup"><span data-stu-id="8f250-232">Its **value** equal to the integer 12.</span></span> <span data-ttu-id="8f250-233">プロパティ値を整数と比較するには、`ep/value` を `Edm.Int32` にキャストします。</span><span class="sxs-lookup"><span data-stu-id="8f250-233">To compare the property value with an integer, cast `ep/value` to `Edm.Int32`.</span></span>


<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=singleValueExtendedProperties/any(ep:ep/id eq 'Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete' and cast(ep/value, Edm.Int32) eq 12)
```


#### <a name="response-4"></a><span data-ttu-id="8f250-234">応答 4</span><span class="sxs-lookup"><span data-stu-id="8f250-234">Response 4</span></span>

<span data-ttu-id="8f250-235">前の 2 つの例では、正常な応答が `HTTP 200 OK` 応答コードによって示され、応答の本文には、対応するフィルターに一致する拡張プロパティを持つメッセージのすべてのプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="8f250-235">For each of the preceding 2 examples, a successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the corresponding filter.</span></span> <span data-ttu-id="8f250-236">応答本文は、[メッセージのコレクションの取得](../api/user_list_messages.md)からの応答に似ています。</span><span class="sxs-lookup"><span data-stu-id="8f250-236">The response body is similar to the response from [getting a message collection](../api/user_list_messages.md).</span></span> <span data-ttu-id="8f250-237">応答は、一致する拡張プロパティを含みません。</span><span class="sxs-lookup"><span data-stu-id="8f250-237">The response does not include the matching extended property.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get singleValueLegacyExtendedProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->