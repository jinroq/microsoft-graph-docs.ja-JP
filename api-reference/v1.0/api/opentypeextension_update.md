# <a name="update-open-extension"></a><span data-ttu-id="4cf7f-101">オープン拡張機能を更新する</span><span class="sxs-lookup"><span data-stu-id="4cf7f-101">Update open extension</span></span>

<span data-ttu-id="4cf7f-102">要求本文内のプロパティでオープン拡張機能 ([openTypeExtension](../resources/openTypeExtension.md) オブジェクト) を更新します。</span><span class="sxs-lookup"><span data-stu-id="4cf7f-102">Update an open extension ([openTypeExtension](../resources/openTypeExtension.md) object) with the properties in the request body:</span></span>

- <span data-ttu-id="4cf7f-103">要求本文内のプロパティが拡張情報内の既存のプロパティの名前と一致すると、拡張情報内のデータが更新されます。</span><span class="sxs-lookup"><span data-stu-id="4cf7f-103">If a property in the request body matches the name of an existing property in the extension, the data in the extension is updated.</span></span>
- <span data-ttu-id="4cf7f-104">一致しないと、このプロパティとそのデータは拡張情報に追加されます。</span><span class="sxs-lookup"><span data-stu-id="4cf7f-104">Otherwise that property and its data are added to the extension.</span></span> 

<span data-ttu-id="4cf7f-105">拡張機能内のデータは、プリミティブ型、またはプリミティブ型の配列にすることができます。</span><span class="sxs-lookup"><span data-stu-id="4cf7f-105">The data in an extension can be primitive types, or arrays of primitive types.</span></span>

## <a name="permissions"></a><span data-ttu-id="4cf7f-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4cf7f-106">Permissions</span></span>

<span data-ttu-id="4cf7f-p101">この API を呼び出すには、拡張機能が作成されたリソースに応じて、以下のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4cf7f-p101">One of the following permissions is required to call this API, depending on the resource that the extension was created in. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4cf7f-109">**サポートされているリソース**</span><span class="sxs-lookup"><span data-stu-id="4cf7f-109">**Supported resource**</span></span>|<span data-ttu-id="4cf7f-110">**アクセス許可**</span><span class="sxs-lookup"><span data-stu-id="4cf7f-110">**Permission**</span></span>|<span data-ttu-id="4cf7f-111">**サポートされているリソース**</span><span class="sxs-lookup"><span data-stu-id="4cf7f-111">**Supported resource**</span></span>|<span data-ttu-id="4cf7f-112">**アクセス許可**</span><span class="sxs-lookup"><span data-stu-id="4cf7f-112">**Permission**</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="4cf7f-113">デバイス</span><span class="sxs-lookup"><span data-stu-id="4cf7f-113">device</span></span>](../resources/device.md) | <span data-ttu-id="4cf7f-114">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4cf7f-114">Device.ReadWrite.All</span></span> | [<span data-ttu-id="4cf7f-115">イベント</span><span class="sxs-lookup"><span data-stu-id="4cf7f-115">event</span></span>](../resources/event.md) | <span data-ttu-id="4cf7f-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4cf7f-116">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="4cf7f-117">グループ</span><span class="sxs-lookup"><span data-stu-id="4cf7f-117">group</span></span>](../resources/group.md) | <span data-ttu-id="4cf7f-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4cf7f-118">Group.ReadWrite.All</span></span> | [<span data-ttu-id="4cf7f-119">グループ イベント</span><span class="sxs-lookup"><span data-stu-id="4cf7f-119">group event</span></span>](../resources/event.md) | <span data-ttu-id="4cf7f-120">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4cf7f-120">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="4cf7f-121">グループの投稿</span><span class="sxs-lookup"><span data-stu-id="4cf7f-121">group post</span></span>](../resources/post.md) | <span data-ttu-id="4cf7f-122">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4cf7f-122">Group.ReadWrite.All</span></span> | [<span data-ttu-id="4cf7f-123">メッセージ</span><span class="sxs-lookup"><span data-stu-id="4cf7f-123">message</span></span>](../resources/message.md) | <span data-ttu-id="4cf7f-124">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4cf7f-124">Mail.ReadWrite</span></span> |
| [<span data-ttu-id="4cf7f-125">組織</span><span class="sxs-lookup"><span data-stu-id="4cf7f-125">organization</span></span>](../resources/organization.md) | <span data-ttu-id="4cf7f-126">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4cf7f-126">Directory.AccessAsUser.All</span></span> | [<span data-ttu-id="4cf7f-127">個人用連絡先</span><span class="sxs-lookup"><span data-stu-id="4cf7f-127">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="4cf7f-128">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4cf7f-128">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="4cf7f-129">ユーザー</span><span class="sxs-lookup"><span data-stu-id="4cf7f-129">user</span></span>](../resources/user.md) | <span data-ttu-id="4cf7f-130">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4cf7f-130">Directory.AccessAsUser.All</span></span> | | |

## <a name="http-request"></a><span data-ttu-id="4cf7f-131">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4cf7f-131">HTTP request</span></span>
<span data-ttu-id="4cf7f-132">要求で、リソース インスタンスを識別し、そのインスタンスの **extensions** ナビゲーション プロパティを使用して拡張機能を識別し、その拡張インスタンスで `PATCH` を行います。</span><span class="sxs-lookup"><span data-stu-id="4cf7f-132">In the request, identify the resource instance, use the **extensions** navigation property of that instance to identify the extension, and do a `PATCH` on that extension instance.</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /devices/{Id}/extensions/{extensionId}
PATCH /users/{id|userPrincipalName}/events/{id}/extensions/{extensionId}
PATCH /groups/{id}/extensions/{extensionId}
PATCH /groups/{id}/events/{id}/extensions/{extensionId}
PATCH /groups/{id}/threads/{id}/posts/{id}/extensions/{extensionId}
PATCH /users/{id|userPrincipalName}/messages/{id}/extensions/{extensionId}
PATCH /organization/{Id}/extensions/{extensionId}
PATCH /users/{id|userPrincipalName}/contacts/{id}/extensions/{extensionId}
PATCH /users/{id|userPrincipalName}/extensions/{extensionId}
```

><span data-ttu-id="4cf7f-p102">**注:** 上記の構文は、含まれる拡張機能を更新するリソース インスタンスを特定する一般的な方法を示しています。こうしたリソース インスタンスを特定するために使用できる他の構文すべても、同様の方法でオープン拡張機能を更新できます。</span><span class="sxs-lookup"><span data-stu-id="4cf7f-p102">**Note:** The above syntax shows some common ways to identify a resource instance, in order to update an extension in it. All other syntax that allows you to identify these resource instances supports updating open extensions in them in a similar way.</span></span>

<span data-ttu-id="4cf7f-135">要求本文に、その拡張情報への変更や追加を行うための任意のカスタム データを含める方法については、[要求本文](#request-body)のセクションをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="4cf7f-135">See the [Request body](#request-body) section about including in the request body any custom data to change or add to that extension.</span></span>


## <a name="path-parameters"></a><span data-ttu-id="4cf7f-136">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="4cf7f-136">Path parameters</span></span>
|<span data-ttu-id="4cf7f-137">パラメーター</span><span class="sxs-lookup"><span data-stu-id="4cf7f-137">Parameter</span></span>|<span data-ttu-id="4cf7f-138">型</span><span class="sxs-lookup"><span data-stu-id="4cf7f-138">Type</span></span>|<span data-ttu-id="4cf7f-139">説明</span><span class="sxs-lookup"><span data-stu-id="4cf7f-139">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="4cf7f-140">ID</span><span class="sxs-lookup"><span data-stu-id="4cf7f-140">id</span></span>|<span data-ttu-id="4cf7f-141">文字列</span><span class="sxs-lookup"><span data-stu-id="4cf7f-141">string</span></span>|<span data-ttu-id="4cf7f-p103">対応するコレクションのインスタンスの一意識別子。必須。</span><span class="sxs-lookup"><span data-stu-id="4cf7f-p103">A unique identifier for an instance of the corresponding collection. Required.</span></span>|
|<span data-ttu-id="4cf7f-144">extensionId</span><span class="sxs-lookup"><span data-stu-id="4cf7f-144">extensionId</span></span>|<span data-ttu-id="4cf7f-145">文字列</span><span class="sxs-lookup"><span data-stu-id="4cf7f-145">string</span></span>|<span data-ttu-id="4cf7f-p104">これは、拡張情報の一意のテキスト識別子である拡張情報名、または拡張情報の種類と一意のテキスト識別子を連結した完全修飾名になります。完全修飾名は、拡張情報を作成したときに、`id` プロパティで返されます。必須。</span><span class="sxs-lookup"><span data-stu-id="4cf7f-p104">This can be an extension name which is a unique text identifier for an extension, or a fully qualified name which concatenates the extension type and unique text identifier. The fully qualified name is returned in the `id` property when you create the extension. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="4cf7f-149">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4cf7f-149">Request headers</span></span>
| <span data-ttu-id="4cf7f-150">名前</span><span class="sxs-lookup"><span data-stu-id="4cf7f-150">Name</span></span>       | <span data-ttu-id="4cf7f-151">値</span><span class="sxs-lookup"><span data-stu-id="4cf7f-151">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="4cf7f-152">承認</span><span class="sxs-lookup"><span data-stu-id="4cf7f-152">Authorization</span></span> | <span data-ttu-id="4cf7f-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4cf7f-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4cf7f-155">コンテンツ タイプ</span><span class="sxs-lookup"><span data-stu-id="4cf7f-155">Content-Type</span></span> | <span data-ttu-id="4cf7f-156">アプリケーション /json</span><span class="sxs-lookup"><span data-stu-id="4cf7f-156">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="4cf7f-157">要求本文</span><span class="sxs-lookup"><span data-stu-id="4cf7f-157">Request body</span></span>

<span data-ttu-id="4cf7f-p106">次に示す必須の名前/値のペアと、その拡張情報に変更を加えるデータまたは追加するデータとともに、[openTypeExtension](../resources/openTypeExtension.md) オブジェクトの JSON 本文を指定します。JSON ペイロード内のデータは、プリミティブ型か、プリミティブ型の配列にすることができます。</span><span class="sxs-lookup"><span data-stu-id="4cf7f-p106">Provide a JSON body of an [openTypeExtension](../resources/openTypeExtension.md) object, with the following required name-value pairs, and any custom data to change or add to that extension. The data in the JSON payload can be primitive types, or arrays of primitive types.</span></span>

| <span data-ttu-id="4cf7f-160">名前</span><span class="sxs-lookup"><span data-stu-id="4cf7f-160">Name</span></span>       | <span data-ttu-id="4cf7f-161">値</span><span class="sxs-lookup"><span data-stu-id="4cf7f-161">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="4cf7f-162">@odata.type</span><span class="sxs-lookup"><span data-stu-id="4cf7f-162">@odata.type</span></span> | <span data-ttu-id="4cf7f-163">Microsoft.Graph.OpenTypeExtension</span><span class="sxs-lookup"><span data-stu-id="4cf7f-163">Microsoft.Graph.OpenTypeExtension</span></span> |
| <span data-ttu-id="4cf7f-164">extensionName</span><span class="sxs-lookup"><span data-stu-id="4cf7f-164">extensionName</span></span> | <span data-ttu-id="4cf7f-165">%unique_string %</span><span class="sxs-lookup"><span data-stu-id="4cf7f-165">%unique_string%</span></span> |

## <a name="response"></a><span data-ttu-id="4cf7f-166">応答</span><span class="sxs-lookup"><span data-stu-id="4cf7f-166">Response</span></span>

<span data-ttu-id="4cf7f-167">成功した場合、このメソッドは `200 OK` 応答コードと、更新した [openTypeExtension](../resources/openTypeExtension.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4cf7f-167">If successful, this method returns a `200 OK` response code and the updated [openTypeExtension](../resources/openTypeExtension.md) object.</span></span>


## <a name="example"></a><span data-ttu-id="4cf7f-168">例</span><span class="sxs-lookup"><span data-stu-id="4cf7f-168">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="4cf7f-169">要求 1</span><span class="sxs-lookup"><span data-stu-id="4cf7f-169">Request 1</span></span>

<span data-ttu-id="4cf7f-p107">最初の例では、メッセージ内の拡張情報を更新する方法を示します。この拡張情報は、最初に次の JSON ペイロードで表されます。</span><span class="sxs-lookup"><span data-stu-id="4cf7f-p107">The first example shows how to update an extension in a message. The extension is initially represented by the following JSON payload:</span></span>

<!-- { "blockType": "ignored" } -->
```http
{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions
('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
    "extensionName": "Com.Contoso.Referral",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
    "companyName": "Wingtip Toys",
    "dealValue": 500050,
    "expirationDate": "2015-12-03T10:00:00Z"
}
```

<span data-ttu-id="4cf7f-172">拡張情報は、その名前で参照できます。</span><span class="sxs-lookup"><span data-stu-id="4cf7f-172">You can reference the extension by its name:</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Com.Contoso.Referral
```

<span data-ttu-id="4cf7f-173">また、拡張情報は、その完全修飾名でも参照できます。</span><span class="sxs-lookup"><span data-stu-id="4cf7f-173">Or you can reference the extension by its fully qualified name:</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral
```

<span data-ttu-id="4cf7f-174">要求の例と以下の要求本文を使用して、上記の拡張情報を次のように更新できます。</span><span class="sxs-lookup"><span data-stu-id="4cf7f-174">You can use either example request and the following request body to update the above extension by:</span></span>
- <span data-ttu-id="4cf7f-175">を `Wingtip Toys` から `Wingtip Toys (USA)` に変更する `Wingtip Toys (USA)`</span><span class="sxs-lookup"><span data-stu-id="4cf7f-175">Changing `companyName` from `Wingtip Toys` to `Wingtip Toys (USA)`</span></span>
- <span data-ttu-id="4cf7f-176">を `500050` から `500100` に変更する `500100`</span><span class="sxs-lookup"><span data-stu-id="4cf7f-176">Changing `dealValue` from `500050` to `500100`</span></span>
- <span data-ttu-id="4cf7f-177">新しいデータをカスタム プロパティ `updated` として追加する `updated`</span><span class="sxs-lookup"><span data-stu-id="4cf7f-177">Adding new data as the custom property `updated`</span></span>

<!-- { "blockType": "ignored" } -->
```http
{
    "@odata.type": "microsoft.graph.openTypeExtension",
    "extensionName": "Com.Contoso.Referral",
    "companyName": "Wingtip Toys (USA)",
    "dealValue": "500100",
    "expirationDate": "2015-12-03T10:00:00.000Z",
    "updated": "2015-10-29T11:00:00.000Z"
} 
```


#### <a name="response-1"></a><span data-ttu-id="4cf7f-178">応答 1</span><span class="sxs-lookup"><span data-stu-id="4cf7f-178">Response 1</span></span>

<span data-ttu-id="4cf7f-179">ここでは、拡張情報を参照するために使用する方法にかかわらず、同じになる応答を示します。</span><span class="sxs-lookup"><span data-stu-id="4cf7f-179">Here is the response which is the same regardless of the way used to reference the extension.</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions
('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
    "extensionName": "Com.Contoso.Referral",
    "companyName": "Wingtip Toys (USA)",
    "dealValue": 500100,
    "expirationDate": "2015-12-03T10:00:00Z",
    "updated": "2015-10-29T11:00:00.000Z"
}
```

****

#### <a name="request-2"></a><span data-ttu-id="4cf7f-180">要求 2</span><span class="sxs-lookup"><span data-stu-id="4cf7f-180">Request 2</span></span>

<span data-ttu-id="4cf7f-p108">2 番目の例では、グループ投稿に含まれる拡張情報を更新する方法を示します。この拡張情報は、次の JSON ペイロード (`2015-07-03T13:04:00Z` の値が `expirationDate`) で最初に表されます。</span><span class="sxs-lookup"><span data-stu-id="4cf7f-p108">The second example shows how to update an extension in a group post. The extension is initially represented by the following JSON payload, with an `expirationDate` value of `2015-07-03T13:04:00Z`:</span></span>

<!-- { "blockType": "ignored" } -->
```http
{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/threads('AAQkADJizZJpEWwqDHsEpV_KA%3D%3D')/posts('AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA%3D')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate",
    "extensionName": "Com.Contoso.Estimate",
    "companyName": "Contoso",
    "expirationDate": "2015-07-03T13:04:00Z",
    "DealValue": 1010100,
    "Strings@odata.type": "#Collection(String)",
    "topPicks": [
        "Employees only",
        "Add spouse or guest",
        "Add family"
    ]
}
```

<span data-ttu-id="4cf7f-183">次に、`expirationDate` を `2016-07-30T11:00:00Z` に変更する要求と要求本文を示します。</span><span class="sxs-lookup"><span data-stu-id="4cf7f-183">The following is the request and request body to change the `expirationDate` to `2016-07-30T11:00:00Z`:</span></span>

<!-- {
  "blockType": "ignored",
  "sampleKeys": ["Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate"],
  "name": "update_opentypeextension"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groups/37df2ff0-0de0-4c33-8aee-75289364aef6/threads/AAQkADJizZJpEWwqDHsEpV_KA==/posts/AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA=/extensions/Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate
Content-type: application/json

{
   "@odata.type": "Microsoft.OutlookServices.OpenTypeExtension",
   "extensionName": "Com.Contoso.Estimate",
   "companyName": "Contoso",
   "expirationDate": "2016-07-30T11:00:00.000Z",
   "DealValue": 1010100,
   "topPicks": [
       "Employees only",
       "Add spouse or guest",
       "Add family"
    ]
}
```

#### <a name="response-2"></a><span data-ttu-id="4cf7f-184">応答 2</span><span class="sxs-lookup"><span data-stu-id="4cf7f-184">Response 2</span></span>

<span data-ttu-id="4cf7f-185">ここでは、拡張情報内の更新された `expirationDate` を表示する 2 番目の例の応答を示します。</span><span class="sxs-lookup"><span data-stu-id="4cf7f-185">Here is the response of the second example which shows the updated `expirationDate` in the extension.</span></span>

<!-- {  
  "blockType": "ignored",  
  "truncated": true,  
  "@odata.type": "microsoft.graph.openTypeExtension"  
} --> 
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/threads('AAQkADJizZJpEWwqDHsEpV_KA%3D%3D')/posts('AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA%3D')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate",
    "extensionName": "Com.Contoso.Estimate",
    "companyName": "Contoso",
    "expirationDate": "2016-07-30T11:00:00Z",
    "DealValue": 1010100,
    "Strings@odata.type": "#Collection(String)",
    "topPicks": [
        "Employees only",
        "Add spouse or guest",
        "Add family"
    ]
}
```

<!-- This page was manually created. -->
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update opentypeextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
} -->
