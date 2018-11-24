# <a name="get-multivaluelegacyextendedproperty"></a><span data-ttu-id="076ef-101">multiValueLegacyExtendedProperty を取得する</span><span class="sxs-lookup"><span data-stu-id="076ef-101">Get multiValueLegacyExtendedProperty</span></span>

<span data-ttu-id="076ef-102">`$expand` を使用して、複数値の拡張プロパティを含むリソース インスタンスを取得します。</span><span class="sxs-lookup"><span data-stu-id="076ef-102">Get a resource instance that contains a multi-value extended property by using `$expand`.</span></span>

<span data-ttu-id="076ef-103">クエリ パラメーター `$expand` を使用すると、指示された拡張プロパティで展開された特定のインスタンスを取得できます。</span><span class="sxs-lookup"><span data-stu-id="076ef-103">Using the query parameter `$expand` allows you to get the specified instance expanded with the indicated extended property.</span></span> <span data-ttu-id="076ef-104">これは、現時点で、拡張プロパティを表す [multiValueLegacyExtendedProperty](../resources/multiValueLegacyExtendedProperty.md) オブジェクトを取得する唯一の方法です。</span><span class="sxs-lookup"><span data-stu-id="076ef-104">This is currently the only way to get the [multiValueLegacyExtendedProperty](../resources/multiValueLegacyExtendedProperty.md) object that represents an extended property.</span></span>

<span data-ttu-id="076ef-105">次のユーザー リソースがサポートされます。</span><span class="sxs-lookup"><span data-stu-id="076ef-105">The following user resources are supported:</span></span>

- [<span data-ttu-id="076ef-106">calendar</span><span class="sxs-lookup"><span data-stu-id="076ef-106">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="076ef-107">contact</span><span class="sxs-lookup"><span data-stu-id="076ef-107">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="076ef-108">contactFolder</span><span class="sxs-lookup"><span data-stu-id="076ef-108">contactFolder</span></span>](../resources/contactfolder.md) 
- [<span data-ttu-id="076ef-109">イベント</span><span class="sxs-lookup"><span data-stu-id="076ef-109">event</span></span>](../resources/event.md)
- [<span data-ttu-id="076ef-110">mailFolder</span><span class="sxs-lookup"><span data-stu-id="076ef-110">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="076ef-111">message</span><span class="sxs-lookup"><span data-stu-id="076ef-111">message</span></span>](../resources/message.md) 

<span data-ttu-id="076ef-112">次のグループ リソースもサポートされます。</span><span class="sxs-lookup"><span data-stu-id="076ef-112">As well as the following group resources:</span></span>

- <span data-ttu-id="076ef-113">グループ [calendar](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="076ef-113">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="076ef-114">グループ [event](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="076ef-114">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="076ef-115">グループ [post](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="076ef-115">group [post](../resources/post.md)</span></span>

<span data-ttu-id="076ef-116">オープン拡張機能または拡張プロパティを使用するのに適した状況と、拡張プロパティを指定する方法の詳細については、「[拡張プロパティの概要](../resources/extended-properties-overview.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="076ef-116">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="076ef-117">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="076ef-117">Permissions</span></span>
<span data-ttu-id="076ef-118">拡張プロパティを受信するリソースに応じて、アクセス許可が委任された (アプリケーション) を要求を入力する、次の表で指定されたアクセス許可は、この API を呼び出すために必要最低限。</span><span class="sxs-lookup"><span data-stu-id="076ef-118">Depending on the resource you're getting the extended property from and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="076ef-119">アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="076ef-119">To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="076ef-120">サポートされているリソース</span><span class="sxs-lookup"><span data-stu-id="076ef-120">Supported resource</span></span> | <span data-ttu-id="076ef-121">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="076ef-121">Delegated (work or school account)</span></span> | <span data-ttu-id="076ef-122">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="076ef-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="076ef-123">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="076ef-123">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="076ef-124">calendar</span><span class="sxs-lookup"><span data-stu-id="076ef-124">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="076ef-125">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="076ef-125">Calendars.Read</span></span> | <span data-ttu-id="076ef-126">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="076ef-126">Calendars.Read</span></span> | <span data-ttu-id="076ef-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="076ef-127">Calendars.Read</span></span> |
| [<span data-ttu-id="076ef-128">連絡先</span><span class="sxs-lookup"><span data-stu-id="076ef-128">contact</span></span>](../resources/contact.md) | <span data-ttu-id="076ef-129">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="076ef-129">Contacts.Read</span></span> | <span data-ttu-id="076ef-130">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="076ef-130">Contacts.Read</span></span> | <span data-ttu-id="076ef-131">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="076ef-131">Contacts.Read</span></span> |
| [<span data-ttu-id="076ef-132">contactFolder</span><span class="sxs-lookup"><span data-stu-id="076ef-132">contactFolder</span></span>](../resources/contactfolder.md) | <span data-ttu-id="076ef-133">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="076ef-133">Contacts.Read</span></span> | <span data-ttu-id="076ef-134">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="076ef-134">Contacts.Read</span></span> | <span data-ttu-id="076ef-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="076ef-135">Contacts.Read</span></span> |
| [<span data-ttu-id="076ef-136">イベント</span><span class="sxs-lookup"><span data-stu-id="076ef-136">event</span></span>](../resources/event.md) | <span data-ttu-id="076ef-137">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="076ef-137">Calendars.Read</span></span> | <span data-ttu-id="076ef-138">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="076ef-138">Calendars.Read</span></span> |  <span data-ttu-id="076ef-139">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="076ef-139">Calendars.Read</span></span>|
| <span data-ttu-id="076ef-140">グループ [calendar](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="076ef-140">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="076ef-141">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="076ef-141">Group.Read.All</span></span> | <span data-ttu-id="076ef-142">使用不可</span><span class="sxs-lookup"><span data-stu-id="076ef-142">Not supported</span></span> | <span data-ttu-id="076ef-143">使用不可</span><span class="sxs-lookup"><span data-stu-id="076ef-143">Not supported</span></span> |
| <span data-ttu-id="076ef-144">グループ [event](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="076ef-144">group [event](../resources/event.md)</span></span> | <span data-ttu-id="076ef-145">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="076ef-145">Group.Read.All</span></span> | <span data-ttu-id="076ef-146">使用不可</span><span class="sxs-lookup"><span data-stu-id="076ef-146">Not supported</span></span> | <span data-ttu-id="076ef-147">使用不可</span><span class="sxs-lookup"><span data-stu-id="076ef-147">Not supported</span></span> |
| <span data-ttu-id="076ef-148">グループ [post](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="076ef-148">group [post](../resources/post.md)</span></span> | <span data-ttu-id="076ef-149">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="076ef-149">Group.Read.All</span></span> | <span data-ttu-id="076ef-150">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="076ef-150">Not supported</span></span> | <span data-ttu-id="076ef-151">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="076ef-151">Group.Read.All</span></span> |
| [<span data-ttu-id="076ef-152">mailFolder</span><span class="sxs-lookup"><span data-stu-id="076ef-152">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="076ef-153">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="076ef-153">Mail.Read</span></span> | <span data-ttu-id="076ef-154">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="076ef-154">Mail.Read</span></span> | <span data-ttu-id="076ef-155">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="076ef-155">Mail.Read</span></span> |
| [<span data-ttu-id="076ef-156">message</span><span class="sxs-lookup"><span data-stu-id="076ef-156">message</span></span>](../resources/message.md) | <span data-ttu-id="076ef-157">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="076ef-157">Mail.Read</span></span> | <span data-ttu-id="076ef-158">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="076ef-158">Mail.Read</span></span> | <span data-ttu-id="076ef-159">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="076ef-159">Mail.Read</span></span> |
 
## <a name="http-request"></a><span data-ttu-id="076ef-160">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="076ef-160">HTTP request</span></span>

<span data-ttu-id="076ef-p103">**id** プロパティに対するフィルターと一致する拡張プロパティで展開された、リソース インスタンスを取得します。フィルター文字列内のスペース文字に [URL エンコード](https://www.w3schools.com/tags/ref_urlencode.asp)を適用していることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="076ef-p103">Get a resource instance expanded with the extended property which matches a filter on the **id** property. Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the filter string.</span></span>

<span data-ttu-id="076ef-163">**メッセージ**インスタンスを取得します。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="076ef-163">Get a **message** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="076ef-164">**MailFolder**のインスタンスを取得します。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="076ef-164">Get a **mailFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/mailFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="076ef-165">**イベント**インスタンスを取得します。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="076ef-165">Get an **event** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="076ef-166">**カレンダー**のインスタンスを取得します。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="076ef-166">Get a **calendar** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/calendars/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="076ef-167">**連絡**のインスタンスを取得します。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="076ef-167">Get a **contact** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="076ef-168">**ContactFolder**のインスタンスを取得します。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="076ef-168">Get a **contactFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/contactfolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="076ef-169">グループ**イベント**のインスタンスを取得します。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="076ef-169">Get a group **event** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="076ef-170">グループの**投稿**のインスタンスを取得します。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="076ef-170">Get a group **post** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

## <a name="path-parameters"></a><span data-ttu-id="076ef-171">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="076ef-171">Path parameters</span></span>
|<span data-ttu-id="076ef-172">パラメーター</span><span class="sxs-lookup"><span data-stu-id="076ef-172">Parameter</span></span>|<span data-ttu-id="076ef-173">型</span><span class="sxs-lookup"><span data-stu-id="076ef-173">Type</span></span>|<span data-ttu-id="076ef-174">説明</span><span class="sxs-lookup"><span data-stu-id="076ef-174">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="076ef-175">id_value</span><span class="sxs-lookup"><span data-stu-id="076ef-175">id_value</span></span>|<span data-ttu-id="076ef-176">String</span><span class="sxs-lookup"><span data-stu-id="076ef-176">String</span></span>|<span data-ttu-id="076ef-p104">照合する拡張プロパティの ID。サポートされている形式のいずれかに従う必要があります。詳しくは、「[Outlook の拡張プロパティの概要](../resources/extended-properties-overview.md)」を参照してください。必須。</span><span class="sxs-lookup"><span data-stu-id="076ef-p104">The ID of the extended property to match. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="076ef-181">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="076ef-181">Request headers</span></span>
| <span data-ttu-id="076ef-182">名前</span><span class="sxs-lookup"><span data-stu-id="076ef-182">Name</span></span>      |<span data-ttu-id="076ef-183">説明</span><span class="sxs-lookup"><span data-stu-id="076ef-183">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="076ef-184">Authorization</span><span class="sxs-lookup"><span data-stu-id="076ef-184">Authorization</span></span>  | <span data-ttu-id="076ef-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="076ef-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="076ef-187">要求本文</span><span class="sxs-lookup"><span data-stu-id="076ef-187">Request body</span></span>
<span data-ttu-id="076ef-188">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="076ef-188">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="076ef-189">応答</span><span class="sxs-lookup"><span data-stu-id="076ef-189">Response</span></span>

<span data-ttu-id="076ef-190">成功した場合、このメソッドは `200 OK` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="076ef-190">If successful, this method returns a `200 OK` response code.</span></span> 

<span data-ttu-id="076ef-191">応答本文には、一致する [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) オブジェクトで展開された、要求したリソース インスタンスで表されるオブジェクトが含まれます。</span><span class="sxs-lookup"><span data-stu-id="076ef-191">The response body includes an object representing the requested resource instance, expanded with the matching [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object.</span></span>

## <a name="example"></a><span data-ttu-id="076ef-192">例</span><span class="sxs-lookup"><span data-stu-id="076ef-192">Example</span></span>
##### <a name="request"></a><span data-ttu-id="076ef-193">要求</span><span class="sxs-lookup"><span data-stu-id="076ef-193">Request</span></span>
<span data-ttu-id="076ef-p106">この例では、複数値の拡張プロパティを含めることで指定されたイベントを取得して展開します。フィルターは、**id** が文字列 `StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation` と一致する拡張プロパティを返します (ここでは、読みやすくするため URL エンコードを削除しています)。</span><span class="sxs-lookup"><span data-stu-id="076ef-p106">This example gets and expands the specified event by including a multi-value extended property. The filter returns the extended property that has its **id** matching the string `StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation` (with URL encoding removed here for ease of reading).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/events('AAMkAGE1M2_bs88AACbuFiiAAA=')?$expand=multiValueExtendedProperties($filter=id%20eq%20'StringArray%20{66f5a359-4659-4830-9070-00050ec6ac6e}%20Name%20Recreation')
```
##### <a name="response"></a><span data-ttu-id="076ef-196">応答</span><span class="sxs-lookup"><span data-stu-id="076ef-196">Response</span></span>

<span data-ttu-id="076ef-197">応答本文には、指定されたイベントのすべてのプロパティと、フィルターから返される拡張プロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="076ef-197">The response body includes all the properties of the specified event and extended property returned from the filter.</span></span>

<span data-ttu-id="076ef-p107">注:簡潔にするために、ここに示す**イベント** オブジェクトは切り詰められています。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="076ef-p107">Note: The **event** object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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