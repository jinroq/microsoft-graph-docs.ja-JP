# <a name="get-multivaluelegacyextendedproperty"></a><span data-ttu-id="f403a-101">multiValueLegacyExtendedProperty を取得する</span><span class="sxs-lookup"><span data-stu-id="f403a-101">Get multiValueLegacyExtendedProperty</span></span>

<span data-ttu-id="f403a-102">`$expand` を使用して、複数値の拡張プロパティを含むリソース インスタンスを取得します。</span><span class="sxs-lookup"><span data-stu-id="f403a-102">Get a resource instance that contains a multi-value extended property by using `$expand`.</span></span>

<span data-ttu-id="f403a-p101">クエリ パラメーター `$expand` を使用すると、指示された拡張プロパティで展開された特定のインスタンスを取得できます。これは、現時点で、拡張プロパティを表す [singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md) オブジェクトを取得する唯一の方法です。</span><span class="sxs-lookup"><span data-stu-id="f403a-p101">Using the query parameter `$expand` allows you to get the specified instance expanded with the indicated extended property. This is currently the only way to get the [singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md) object that represents an extended property.</span></span>

<span data-ttu-id="f403a-105">次のユーザー リソースがサポートされます。</span><span class="sxs-lookup"><span data-stu-id="f403a-105">The following user resources are supported:</span></span>

- [<span data-ttu-id="f403a-106">message</span><span class="sxs-lookup"><span data-stu-id="f403a-106">message</span></span>](../resources/message.md)
- [<span data-ttu-id="f403a-107">mailFolder</span><span class="sxs-lookup"><span data-stu-id="f403a-107">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="f403a-108">event</span><span class="sxs-lookup"><span data-stu-id="f403a-108">event</span></span>](../resources/event.md)
- [<span data-ttu-id="f403a-109">calendar</span><span class="sxs-lookup"><span data-stu-id="f403a-109">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="f403a-110">contact</span><span class="sxs-lookup"><span data-stu-id="f403a-110">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="f403a-111">contactFolder</span><span class="sxs-lookup"><span data-stu-id="f403a-111">contactFolder</span></span>](../resources/contactfolder.md) 

<span data-ttu-id="f403a-112">次のグループ リソースもサポートされます。</span><span class="sxs-lookup"><span data-stu-id="f403a-112">As well as the following group resources:</span></span>

- <span data-ttu-id="f403a-113">グループ [event](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="f403a-113">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="f403a-114">グループ [calendar](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="f403a-114">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="f403a-115">グループ [post](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="f403a-115">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="f403a-116">オープン拡張機能または拡張プロパティを使用するのに適した状況と、拡張プロパティを指定する方法の詳細については、「[拡張プロパティの概要](../resources/extended-properties-overview.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f403a-116">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="f403a-117">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f403a-117">Permissions</span></span>
<span data-ttu-id="f403a-p102">この API を呼び出すには、取得するリソースに応じて、以下のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f403a-p102">One of the following permissions is required to call this API, depending on the resource you're getting. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

- <span data-ttu-id="f403a-120">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="f403a-120">Mail.Read</span></span>
- <span data-ttu-id="f403a-121">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f403a-121">Calendars.Read</span></span>
- <span data-ttu-id="f403a-122">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="f403a-122">Contacts.Read</span></span>
- <span data-ttu-id="f403a-123">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="f403a-123">Group.Read.All</span></span> 
 
## <a name="http-request"></a><span data-ttu-id="f403a-124">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f403a-124">HTTP request</span></span>

<span data-ttu-id="f403a-p103">**id** プロパティに対するフィルターと一致する拡張プロパティで展開された、リソース インスタンスを取得します。フィルター文字列内のスペース文字に [URL エンコード](http://www.w3schools.com/tags/ref_urlencode.asp)を適用していることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="f403a-p103">Get a resource instance expanded with the extended property which matches a filter on the **id** property. Make sure you apply [URL encoding](http://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the filter string.</span></span>

<span data-ttu-id="f403a-127">**message** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="f403a-127">Get a **message** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="f403a-128">**mailFolder** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="f403a-128">Get a **mailFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="f403a-129">**event** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="f403a-129">Get an **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="f403a-130">**calendar** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="f403a-130">Get a **calendar** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="f403a-131">**contact** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="f403a-131">Get a **contact** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="f403a-132">**contactFolder** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="f403a-132">Get a **contactFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="f403a-133">グループ **event** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="f403a-133">Get a group **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="f403a-134">グループ **post** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="f403a-134">Get a group **post** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

## <a name="parameters"></a><span data-ttu-id="f403a-135">パラメーター</span><span class="sxs-lookup"><span data-stu-id="f403a-135">Parameters</span></span>
|<span data-ttu-id="f403a-136">**パラメーター**</span><span class="sxs-lookup"><span data-stu-id="f403a-136">**Parameter**</span></span>|<span data-ttu-id="f403a-137">**型**</span><span class="sxs-lookup"><span data-stu-id="f403a-137">**Type**</span></span>|<span data-ttu-id="f403a-138">**説明**</span><span class="sxs-lookup"><span data-stu-id="f403a-138">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="f403a-139">_URL parameters_</span><span class="sxs-lookup"><span data-stu-id="f403a-139">_URL parameters_</span></span>|
|<span data-ttu-id="f403a-140">id_value</span><span class="sxs-lookup"><span data-stu-id="f403a-140">id_value</span></span>|<span data-ttu-id="f403a-141">String</span><span class="sxs-lookup"><span data-stu-id="f403a-141">String</span></span>|<span data-ttu-id="f403a-p104">照合する拡張プロパティの ID。サポートされている形式のいずれかに従う必要があります。詳しくは、「[Outlook の拡張プロパティの概要](../resources/extended-properties-overview.md)」を参照してください。必須。</span><span class="sxs-lookup"><span data-stu-id="f403a-p104">The ID of the extended property to match. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="f403a-146">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f403a-146">Request headers</span></span>
| <span data-ttu-id="f403a-147">名前</span><span class="sxs-lookup"><span data-stu-id="f403a-147">Name</span></span>      |<span data-ttu-id="f403a-148">説明</span><span class="sxs-lookup"><span data-stu-id="f403a-148">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f403a-149">Authorization</span><span class="sxs-lookup"><span data-stu-id="f403a-149">Authorization</span></span>  | <span data-ttu-id="f403a-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f403a-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f403a-152">要求本文</span><span class="sxs-lookup"><span data-stu-id="f403a-152">Request body</span></span>
<span data-ttu-id="f403a-153">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f403a-153">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f403a-154">応答</span><span class="sxs-lookup"><span data-stu-id="f403a-154">Response</span></span>

<span data-ttu-id="f403a-155">成功した場合、このメソッドは `200 OK` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="f403a-155">If successful, this method returns a `200 OK` response code.</span></span> 

<span data-ttu-id="f403a-156">応答本文には、一致する [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) オブジェクトで展開された、要求したリソース インスタンスで表されるオブジェクトが含まれます。</span><span class="sxs-lookup"><span data-stu-id="f403a-156">The response body includes an object representing the requested resource instance, expanded with the matching [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object.</span></span>

## <a name="example"></a><span data-ttu-id="f403a-157">例</span><span class="sxs-lookup"><span data-stu-id="f403a-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f403a-158">要求</span><span class="sxs-lookup"><span data-stu-id="f403a-158">Request</span></span>
<span data-ttu-id="f403a-p106">この例では、複数値の拡張プロパティを含めることで指定されたイベントを取得して展開します。フィルターは、**id** が文字列 `StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation` と一致する拡張プロパティを返します (ここでは、読みやすくするため URL エンコードを削除しています)。</span><span class="sxs-lookup"><span data-stu-id="f403a-p106">This example gets and expands the specified event by including a multi-value extended property. The filter returns the extended property that has its **id** matching the string `StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation` (with URL encoding removed here for ease of reading).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/events('AAMkAGE1M2_bs88AACbuFiiAAA=')?$expand=multiValueExtendedProperties($filter=id%20eq%20'StringArray%20{66f5a359-4659-4830-9070-00050ec6ac6e}%20Name%20Recreation')
```
##### <a name="response"></a><span data-ttu-id="f403a-161">応答</span><span class="sxs-lookup"><span data-stu-id="f403a-161">Response</span></span>

<span data-ttu-id="f403a-162">応答本文には、指定されたイベントのすべてのプロパティと、フィルターから返される拡張プロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="f403a-162">The response body includes all the properties of the specified event and extended property returned from the filter.</span></span>

<span data-ttu-id="f403a-p107">注:簡潔にするために、ここに示す**イベント** オブジェクトは切り詰められています。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f403a-p107">Note: The **event** object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/events/$entity",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfcd489-628b-40d7-b48b-57002df800e5@1717622f-1d94-4d0c-9d74-709fad664b77')/events('AAMkAGE1M2_bs88AACbuFiiAAA=')",
    "@odata.etag": "W/\"mODEKWhc/Um6lA3uPm7PPAAAm8k15A==\"",
    "id": "AAMkAGE1M2_bs88AACbuFiiAAA=",
    "start": {
        "dateTime": "2015-11-26T17:00:00.0000000",
        "timeZone": "UTC"
    },
    "end": {
        "dateTime": "2015-11-30T05:00:00.0000000",
        "timeZone": "UTC"
    },
    "organizer": {
        "emailAddress": {
            "name": "Christine Irwin",
            "address": "christine@contoso.com"
        }
    },
    "multiValueExtendedProperties@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/events('AAMkAGE1M2_bs88AACbuFiiAAA%3D')/multiValueExtendedProperties",
    "multiValueExtendedProperties": [
        {
            "id": "StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation",
            "value": [
                "Food",
                "Hiking",
                "Swimming"
            ]
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get multiValueLegacyExtendedProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->