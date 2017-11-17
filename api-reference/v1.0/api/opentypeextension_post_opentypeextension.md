# <a name="create-open-extension"></a><span data-ttu-id="70e6c-101">オープン拡張機能を作成する</span><span class="sxs-lookup"><span data-stu-id="70e6c-101">Create open extension</span></span>

<span data-ttu-id="70e6c-102">オープン拡張機能 ([openTypeExtension](../resources/openTypeExtension.md) オブジェクト) を作成し、リソースの新規または既存のインスタンスのカスタム プロパティを追加します。</span><span class="sxs-lookup"><span data-stu-id="70e6c-102">Create an open extension ([openTypeExtension](../resources/openTypeExtension.md) object) and add custom properties in a new or existing instance of a resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="70e6c-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="70e6c-103">Permissions</span></span>

<span data-ttu-id="70e6c-p101">この API を呼び出すには、拡張機能を作成するリソースに応じて、以下のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="70e6c-p101">One of the following permissions is required to call this API, depending on the resource you're creating the extension in. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="70e6c-106">**サポートされているリソース**</span><span class="sxs-lookup"><span data-stu-id="70e6c-106">**Supported resource**</span></span>|<span data-ttu-id="70e6c-107">**アクセス許可**</span><span class="sxs-lookup"><span data-stu-id="70e6c-107">**Permission**</span></span>|<span data-ttu-id="70e6c-108">**サポートされているリソース**</span><span class="sxs-lookup"><span data-stu-id="70e6c-108">**Supported resource**</span></span>|<span data-ttu-id="70e6c-109">**アクセス許可**</span><span class="sxs-lookup"><span data-stu-id="70e6c-109">**Permission**</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="70e6c-110">デバイス</span><span class="sxs-lookup"><span data-stu-id="70e6c-110">device</span></span>](../resources/device.md) | <span data-ttu-id="70e6c-111">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70e6c-111">Device.ReadWrite.All</span></span> | [<span data-ttu-id="70e6c-112">イベント</span><span class="sxs-lookup"><span data-stu-id="70e6c-112">event</span></span>](../resources/event.md) | <span data-ttu-id="70e6c-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="70e6c-113">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="70e6c-114">グループ</span><span class="sxs-lookup"><span data-stu-id="70e6c-114">group</span></span>](../resources/group.md) | <span data-ttu-id="70e6c-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70e6c-115">Group.ReadWrite.All</span></span> | [<span data-ttu-id="70e6c-116">グループ イベント</span><span class="sxs-lookup"><span data-stu-id="70e6c-116">group event</span></span>](../resources/event.md) | <span data-ttu-id="70e6c-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70e6c-117">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="70e6c-118">グループの投稿</span><span class="sxs-lookup"><span data-stu-id="70e6c-118">group post</span></span>](../resources/post.md) | <span data-ttu-id="70e6c-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70e6c-119">Group.ReadWrite.All</span></span> | [<span data-ttu-id="70e6c-120">メッセージ</span><span class="sxs-lookup"><span data-stu-id="70e6c-120">message</span></span>](../resources/message.md) | <span data-ttu-id="70e6c-121">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="70e6c-121">Mail.ReadWrite</span></span> |
| [<span data-ttu-id="70e6c-122">組織</span><span class="sxs-lookup"><span data-stu-id="70e6c-122">organization</span></span>](../resources/organization.md) | <span data-ttu-id="70e6c-123">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="70e6c-123">Directory.AccessAsUser.All</span></span> | [<span data-ttu-id="70e6c-124">個人用連絡先</span><span class="sxs-lookup"><span data-stu-id="70e6c-124">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="70e6c-125">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="70e6c-125">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="70e6c-126">ユーザー</span><span class="sxs-lookup"><span data-stu-id="70e6c-126">user</span></span>](../resources/user.md) | <span data-ttu-id="70e6c-127">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="70e6c-127">Directory.AccessAsUser.All</span></span> | | |

## <a name="http-request"></a><span data-ttu-id="70e6c-128">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="70e6c-128">HTTP request</span></span>

### <a name="create-an-extension-in-a-new-resource-instance"></a><span data-ttu-id="70e6c-129">新規のリソース インスタンスに拡張機能を作成する</span><span class="sxs-lookup"><span data-stu-id="70e6c-129">Create an extension in a new resource instance</span></span>

<span data-ttu-id="70e6c-130">インスタンスを作成するのと同じ REST 要求を使用します。</span><span class="sxs-lookup"><span data-stu-id="70e6c-130">Use the same REST request as creating the instance.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/events
POST /users/{id|userPrincipalName}/messages
POST /groups/{id}/events
POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /users/{id|userPrincipalName}/contacts
```

><span data-ttu-id="70e6c-p102">**注:**上記の構文は、サポートされているリソース インスタンスを作成する一般的な方法を示しています。こうしたリソース インスタンスを作成するために使用できる他の POST 構文すべても、同様の方法でオープン拡張機能を作成できます。</span><span class="sxs-lookup"><span data-stu-id="70e6c-p102">**Note:** The above syntax shows some common ways to create the supported resource instances. All other POST syntax that allows you to create these resource instances supports creating open extensions in them in a similar way.</span></span>

<span data-ttu-id="70e6c-133">要求本文に、新規のリソース インスタンスのプロパティおよび_拡張機能_を含める方法については、[要求本文](#request-body)のセクションをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="70e6c-133">See the [Request body](#request-body) section about including the properties of the new resource instance _and the extension_ in the request body.</span></span>

### <a name="create-an-extension-in-an-existing-resource-instance"></a><span data-ttu-id="70e6c-134">既存のリソース インスタンスに拡張機能を作成する</span><span class="sxs-lookup"><span data-stu-id="70e6c-134">Create an extension in an existing resource instance</span></span>

<span data-ttu-id="70e6c-135">要求でリソース インスタンスを識別し、**extensions** ナビゲーション プロパティで `POST` を行います。</span><span class="sxs-lookup"><span data-stu-id="70e6c-135">Identify the resource instance in the request and do a `POST` to the **extensions** navigation property.</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /devices/{id}/extensions
POST /users/{id|userPrincipalName}/events/{id}/extensions
POST /groups/{id}/extensions
POST /groups/{id}/events/{id}/extensions
POST /groups/{id}/threads/{id}/posts/{id}/extensions
POST /users/{id|userPrincipalName}/messages/{id}/extensions
POST /organization/{id}/extensions
POST /users/{id|userPrincipalName}/contacts/{id}/extensions
POST /users/{id|userPrincipalName}/extensions
```

><span data-ttu-id="70e6c-p103">**注:**上記の構文は、拡張機能をその中に作成するリソース インスタンスを特定する一般的な方法を示しています。こうしたリソース インスタンスを特定するために使用できる他の構文すべても、同様の方法でオープン拡張機能を作成できます。</span><span class="sxs-lookup"><span data-stu-id="70e6c-p103">**Note:** The above syntax shows some common ways to identify a resource instance, in order to create an extension in it. All other syntax that allows you to identify these resource instances supports creating open extensions in them in a similar way.</span></span>

<span data-ttu-id="70e6c-138">要求本文に_拡張機能_を含める方法については、[要求本文](#request-body)のセクションをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="70e6c-138">See the [Request body](#request-body) section about including _the extension_ in the request body.</span></span>

## <a name="parameters"></a><span data-ttu-id="70e6c-139">パラメーター</span><span class="sxs-lookup"><span data-stu-id="70e6c-139">Parameters</span></span>
|<span data-ttu-id="70e6c-140">**パラメーター**</span><span class="sxs-lookup"><span data-stu-id="70e6c-140">**Parameter**</span></span>|<span data-ttu-id="70e6c-141">**型**</span><span class="sxs-lookup"><span data-stu-id="70e6c-141">**Type**</span></span>|<span data-ttu-id="70e6c-142">**説明**</span><span class="sxs-lookup"><span data-stu-id="70e6c-142">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="70e6c-143">_URL parameters_</span><span class="sxs-lookup"><span data-stu-id="70e6c-143">_URL parameters_</span></span>|
|<span data-ttu-id="70e6c-144">id</span><span class="sxs-lookup"><span data-stu-id="70e6c-144">id</span></span>|<span data-ttu-id="70e6c-145">string</span><span class="sxs-lookup"><span data-stu-id="70e6c-145">string</span></span>|<span data-ttu-id="70e6c-p104">該当するコレクション内のオブジェクトの一意識別子。必須。</span><span class="sxs-lookup"><span data-stu-id="70e6c-p104">A unique identifier for an object in the corresponding collection. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="70e6c-148">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="70e6c-148">Request headers</span></span>
| <span data-ttu-id="70e6c-149">名前</span><span class="sxs-lookup"><span data-stu-id="70e6c-149">Name</span></span>       | <span data-ttu-id="70e6c-150">値</span><span class="sxs-lookup"><span data-stu-id="70e6c-150">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="70e6c-151">Authorization</span><span class="sxs-lookup"><span data-stu-id="70e6c-151">Authorization</span></span> | <span data-ttu-id="70e6c-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="70e6c-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="70e6c-154">Content-Type</span><span class="sxs-lookup"><span data-stu-id="70e6c-154">Content-Type</span></span> | <span data-ttu-id="70e6c-155">application/json</span><span class="sxs-lookup"><span data-stu-id="70e6c-155">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="70e6c-156">要求本文</span><span class="sxs-lookup"><span data-stu-id="70e6c-156">Request body</span></span>

<span data-ttu-id="70e6c-p106">[openTypeExtension](../resources/openTypeExtension.md) の JSON 本文を、次の必須の名前と値の組や、その他のカスタム データとともに指定します。JSON ペイロード内のデータは、プリミティブ型か、プリミティブ型の配列にすることができます。</span><span class="sxs-lookup"><span data-stu-id="70e6c-p106">Provide a JSON body of an [openTypeExtension](../resources/openTypeExtension.md), with the following required name-value pairs, and any additional custom data. The data in the JSON payload can be primitive types, or arrays of primitive types.</span></span>

| <span data-ttu-id="70e6c-159">名前</span><span class="sxs-lookup"><span data-stu-id="70e6c-159">Name</span></span>       | <span data-ttu-id="70e6c-160">値</span><span class="sxs-lookup"><span data-stu-id="70e6c-160">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="70e6c-161">@odata.type</span><span class="sxs-lookup"><span data-stu-id="70e6c-161">@odata.type</span></span> | <span data-ttu-id="70e6c-162">Microsoft.Graph.OpenTypeExtension</span><span class="sxs-lookup"><span data-stu-id="70e6c-162">Microsoft.Graph.OpenTypeExtension</span></span> |
| <span data-ttu-id="70e6c-163">extensionName</span><span class="sxs-lookup"><span data-stu-id="70e6c-163">extensionName</span></span> | <span data-ttu-id="70e6c-164">%unique_string%</span><span class="sxs-lookup"><span data-stu-id="70e6c-164">%unique_string%</span></span> |

<span data-ttu-id="70e6c-165">_新しい_リソース インスタンスに拡張機能を作成するときは、新しい **openTypeExtension** オブジェクトに加えて、関連するプロパティの JSON 表現を指定して、このようなリソース インスタンスを作成します。</span><span class="sxs-lookup"><span data-stu-id="70e6c-165">When creating an extension in a _new_ resource instance, in addition to the new **openTypeExtension** object, provide a JSON representation of the relevant properties to create such a resource instance.</span></span>

## <a name="response"></a><span data-ttu-id="70e6c-166">応答</span><span class="sxs-lookup"><span data-stu-id="70e6c-166">Response</span></span>

#### <a name="response-code"></a><span data-ttu-id="70e6c-167">応答コード</span><span class="sxs-lookup"><span data-stu-id="70e6c-167">Response code</span></span>
<span data-ttu-id="70e6c-168">応答コードは、操作によって `201 Created` または `202 Accepted` になります。</span><span class="sxs-lookup"><span data-stu-id="70e6c-168">Depending on the operation, the response code can be `201 Created` or `202 Accepted`.</span></span>

<span data-ttu-id="70e6c-p107">リソース インスタンスを作成するのと同じ操作で拡張機能を作成するとき、成功した操作は、拡張機能を作成せずにリソース インスタンスのみを作成する操作を使用したときと同じ応答コードを返します。それぞれ対応するインスタンスの作成については[上記](#create-an-extension-in-a-new-resource-instance)のトピックをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="70e6c-p107">When creating an extension in the same operation as creating a resource instance, a successful operation returns the same response code as when the operation is used to create only the resource instance without the extension. Refer to the corresponding topics for creating the instance, as listed [above](#create-an-extension-in-a-new-resource-instance).</span></span>

#### <a name="response-body"></a><span data-ttu-id="70e6c-171">応答本文</span><span class="sxs-lookup"><span data-stu-id="70e6c-171">Response body</span></span>
| <span data-ttu-id="70e6c-172">シナリオ</span><span class="sxs-lookup"><span data-stu-id="70e6c-172">Scenario</span></span>       | <span data-ttu-id="70e6c-173">リソース</span><span class="sxs-lookup"><span data-stu-id="70e6c-173">Resource</span></span>  | <span data-ttu-id="70e6c-174">応答本文</span><span class="sxs-lookup"><span data-stu-id="70e6c-174">Response body</span></span> |
|:---------------|:----------|:--------------|
| <span data-ttu-id="70e6c-175">_新しい_リソース インスタンスを明示的に作成しながら、拡張機能を作成する</span><span class="sxs-lookup"><span data-stu-id="70e6c-175">Creating an extension while explicitly creating a _new_ resource instance</span></span> | [<span data-ttu-id="70e6c-176">連絡先](../resources/contact.md)、[イベント](../resources/event.md)、[メッセージ</span><span class="sxs-lookup"><span data-stu-id="70e6c-176">contact](../resources/contact.md), [event](../resources/event.md), [message</span></span>](../resources/message.md) | <span data-ttu-id="70e6c-177">[openTypeExtension](../resources/openTypeExtension.md) オブジェクトで展開した新しいインスタンスを含みます。</span><span class="sxs-lookup"><span data-stu-id="70e6c-177">Includes the new instance expanded with the [openTypeExtension](../resources/openTypeExtension.md) object.</span></span> |
| <span data-ttu-id="70e6c-178">新しいリソース インスタンスを暗示的に作成しながら、拡張機能を作成する</span><span class="sxs-lookup"><span data-stu-id="70e6c-178">Creating an extension while implicitly creating a resource instance</span></span> | [<span data-ttu-id="70e6c-179">post</span><span class="sxs-lookup"><span data-stu-id="70e6c-179">post</span></span>](../resources/post.md) | <span data-ttu-id="70e6c-180">応答には、応答コードだけが含まれ、応答本体は含まれません。</span><span class="sxs-lookup"><span data-stu-id="70e6c-180">The response includes only a response code but not a response body.</span></span> |
| <span data-ttu-id="70e6c-181">_既存_のリソース インスタンスに拡張機能を作成する</span><span class="sxs-lookup"><span data-stu-id="70e6c-181">Creating an extension in an _existing_ resource instance</span></span> | <span data-ttu-id="70e6c-182">サポートされているすべてのリソース</span><span class="sxs-lookup"><span data-stu-id="70e6c-182">All supported resources</span></span> | <span data-ttu-id="70e6c-183">**openTypeExtension** オブジェクトが含まれます。</span><span class="sxs-lookup"><span data-stu-id="70e6c-183">Includes the **openTypeExtension** object.</span></span> |

## <a name="example"></a><span data-ttu-id="70e6c-184">例</span><span class="sxs-lookup"><span data-stu-id="70e6c-184">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="70e6c-185">要求 1</span><span class="sxs-lookup"><span data-stu-id="70e6c-185">Request 1</span></span>

<span data-ttu-id="70e6c-p108">最初の例では、同一の呼び出しでメッセージと拡張情報を作成します。要求本文には、次のものが含まれます。</span><span class="sxs-lookup"><span data-stu-id="70e6c-p108">The first example creates a message and an extension in the same call. The request body includes the following:</span></span>

- <span data-ttu-id="70e6c-188">新しいメッセージ固有の **subject**、**body**、**toRecipients** プロパティ。</span><span class="sxs-lookup"><span data-stu-id="70e6c-188">The **subject**, **body**, and **toRecipients** properties typical of a new message.</span></span> 
- <span data-ttu-id="70e6c-189">拡張情報に関する次のもの。</span><span class="sxs-lookup"><span data-stu-id="70e6c-189">And for the extension:</span></span>

  - <span data-ttu-id="70e6c-190">型 `Microsoft.Graph.OpenTypeExtension`。</span><span class="sxs-lookup"><span data-stu-id="70e6c-190">The type `Microsoft.Graph.OpenTypeExtension`.</span></span> 
  - <span data-ttu-id="70e6c-191">拡張情報名 "Com.Contoso.Referral"。</span><span class="sxs-lookup"><span data-stu-id="70e6c-191">The extension name "Com.Contoso.Referral".</span></span> 
  - <span data-ttu-id="70e6c-192">JSON ペイロードに 3 つのカスタム プロパティとして格納される追加のデータ: `companyName`、`expirationDate`、`dealValue`。</span><span class="sxs-lookup"><span data-stu-id="70e6c-192">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `expirationDate`, and `dealValue`.</span></span>  

<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_1"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages

{
  "subject": "Annual review",
  "body": {
    "contentType": "HTML",
    "content": "You should be proud!"
  },
  "toRecipients": [
    {
      "emailAddress": {
        "address": "rufus@contoso.com"
      }
    }
  ],
  "extensions": [
    {
      "@odata.type": "Microsoft.Graph.OpenTypeExtension",
      "extensionName": "Com.Contoso.Referral",
      "companyName": "Wingtip Toys",
      "expirationDate": "2015-12-30T11:00:00.000Z",
      "dealValue": 10000
    }
  ]
}
```

##### <a name="response-1"></a><span data-ttu-id="70e6c-193">応答 1</span><span class="sxs-lookup"><span data-stu-id="70e6c-193">Response 1</span></span>

<span data-ttu-id="70e6c-p109">最初の例の応答を次に示します。応答本文には、新しいメッセージのプロパティと、新しい拡張情報に関する次のものが含まれています。</span><span class="sxs-lookup"><span data-stu-id="70e6c-p109">Here is the response for the first example. The response body includes properties of the new message, and the following for the new extension:</span></span>

- <span data-ttu-id="70e6c-196">**id** プロパティと `Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral` の完全修飾名。</span><span class="sxs-lookup"><span data-stu-id="70e6c-196">The **id** property with the fully qualified name of `Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral`.</span></span> 
- <span data-ttu-id="70e6c-197">要求で指定されている既定のプロパティ **extensionName**。</span><span class="sxs-lookup"><span data-stu-id="70e6c-197">The default property **extensionName** specified in the request.</span></span>
- <span data-ttu-id="70e6c-198">要求で指定されている、3 つのカスタム プロパティとして格納されるカスタム データ。</span><span class="sxs-lookup"><span data-stu-id="70e6c-198">The custom data specified in the request stored as 3 custom properties.</span></span>

<span data-ttu-id="70e6c-p110">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="70e6c-p110">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages/$entity",
  "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df800e5@1717f226-49d1-4d0c-9d74-709fad664b77')/messages
('AAMkAGEbs88AAB84uLuAAA=')",
  "@odata.etag": "W/\"CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AAB88LOj\"",
  "id": "AAMkAGEbs88AAB84uLuAAA=",
  "createdDateTime": "2015-10-30T03:03:43Z",
  "lastModifiedDateTime": "2015-10-30T03:03:43Z",
  "changeKey": "CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AAB88LOj",
  "categories": [ ],
  "receivedDateTime": "2015-10-30T03:03:43Z",
  "sentDateTime": "2015-10-30T03:03:43Z",
  "hasAttachments": false,
  "subject": "Annual review",
  "body": {
    "contentType": "HTML",
    "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r
\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nYou should be proud!\r\n</body>\r
\n</html>\r\n"
  },
  "bodyPreview": "You should be proud!",
  "importance": "Normal",
  "parentFolderId": "AQMkAGEwAAAIBDwAAAA==",
  "sender": null,
  "from": null,
  "toRecipients": [
    {
      "emailAddress": {
        "address": "rufus@contoso.com",
        "name": "John Doe"
      }
    }
  ],
  "ccRecipients": [ ],
  "bccRecipients": [ ],
  "replyTo": [ ],
  "conversationId": "AAQkAGEFGugh3SVdMzzc=",
  "isDeliveryReceiptRequested": false,
  "isReadReceiptRequested": false,
  "isRead": true,
  "isDraft": true,
  "webLink": "https://outlook.office.com/owa/?
ItemID=AAMkAGEbs88AAB84uLuAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
  "inferenceClassification": "Focused",
  "extensions@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages
('AAMkAGEbs88AAB84uLuAAA%3D')/extensions",
  "extensions": [
    {
      "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
      "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df800e5@1717f226-49d1-4d0c-9d74-709fad664b77')/messages
('AAMkAGEbs88AAB84uLuAAA=')/extensions('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
      "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
      "extensionName": "Com.Contoso.Referral",
      "companyName": "Wingtip Toys",
      "expirationDate": "2015-12-30T11:00:00.000Z",
      "dealValue": 10000
    }
  ]
}
```


****

##### <a name="request-2"></a><span data-ttu-id="70e6c-201">要求 2</span><span class="sxs-lookup"><span data-stu-id="70e6c-201">Request 2</span></span>

<span data-ttu-id="70e6c-p111">2 番目の例では、指定されたメッセージに拡張情報を作成します。要求本文には、拡張情報に関する次のものが含まれます。</span><span class="sxs-lookup"><span data-stu-id="70e6c-p111">The second example creates an extension in the specified message. The request body includes the following for the extension:</span></span>

- <span data-ttu-id="70e6c-204">型 `Microsoft.Graph.OpenTypeExtension`。</span><span class="sxs-lookup"><span data-stu-id="70e6c-204">The type `Microsoft.Graph.OpenTypeExtension`.</span></span> 
- <span data-ttu-id="70e6c-205">拡張情報名 "Com.Contoso.Referral"。</span><span class="sxs-lookup"><span data-stu-id="70e6c-205">The extension name "Com.Contoso.Referral".</span></span>
- <span data-ttu-id="70e6c-206">JSON ペイロードに 3 つのカスタム プロパティとして格納される追加のデータ: `companyName`、`dealValue`、`expirationDate`。</span><span class="sxs-lookup"><span data-stu-id="70e6c-206">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `dealValue`, and `expirationDate`.</span></span>  

<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_2"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions

{ 
  "@odata.type" : "Microsoft.Graph.OpenTypeExtension", 
  "extensionName" : "Com.Contoso.Referral", 
  "companyName" : "Wingtip Toys", 
  "dealValue" : 500050, 
  "expirationDate" : "2015-12-03T10:00:00.000Z" 
} 
```

##### <a name="response-2"></a><span data-ttu-id="70e6c-207">応答 2</span><span class="sxs-lookup"><span data-stu-id="70e6c-207">Response 2</span></span>

<span data-ttu-id="70e6c-p112">2 番目の例の応答を次に示します。応答本文には、新しい拡張情報に関する次のものが含まれています。</span><span class="sxs-lookup"><span data-stu-id="70e6c-p112">Here is the response for the second example. The response body includes the following for the new extension:</span></span>

- <span data-ttu-id="70e6c-210">既定のプロパティ **extensionName**。</span><span class="sxs-lookup"><span data-stu-id="70e6c-210">The default property **extensionName**.</span></span>
- <span data-ttu-id="70e6c-211">**id** プロパティと `Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral` の完全修飾名。</span><span class="sxs-lookup"><span data-stu-id="70e6c-211">The **id** property with the fully qualified name of `Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral`.</span></span> 
- <span data-ttu-id="70e6c-212">格納されるカスタム データ。</span><span class="sxs-lookup"><span data-stu-id="70e6c-212">The custom data to be stored.</span></span>  

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.opentypeextension"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions/$entity",
    "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions
('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
    "extensionName": "Com.Contoso.Referral",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
    "companyName": "Wingtip Toys",
    "dealValue": 500050,
    "expirationDate": "2015-12-03T10:00:00.000Z"
}
```

****

##### <a name="request-3"></a><span data-ttu-id="70e6c-213">要求 3</span><span class="sxs-lookup"><span data-stu-id="70e6c-213">Request 3</span></span>

<span data-ttu-id="70e6c-p113">3 番目の例では、指定されたグループ イベントに拡張情報を作成します。要求本文には、拡張情報に関する次のものが含まれます。</span><span class="sxs-lookup"><span data-stu-id="70e6c-p113">The third example creates an extension in the specified group event. The request body includes the following for the extension:</span></span>

- <span data-ttu-id="70e6c-216">型 `Microsoft.Graph.OpenTypeExtension`。</span><span class="sxs-lookup"><span data-stu-id="70e6c-216">The type `Microsoft.Graph.OpenTypeExtension`.</span></span> 
- <span data-ttu-id="70e6c-217">拡張情報名 "Com.Contoso.Deal"。</span><span class="sxs-lookup"><span data-stu-id="70e6c-217">The extension name "Com.Contoso.Deal".</span></span>
- <span data-ttu-id="70e6c-218">JSON ペイロードに 3 つのカスタム プロパティとして格納される追加のデータ: `companyName`、`dealValue`、`expirationDate`。</span><span class="sxs-lookup"><span data-stu-id="70e6c-218">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `dealValue`, and `expirationDate`.</span></span>  

<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_3"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups('f5480dfd-7d77-4d0b-ba2e-3391953cc74a')/events('AAMkADVl17IsAAA=')/extensions 

{
  "@odata.type" : "Microsoft.Graph.OpenTypeExtension",
  "extensionName" : "Com.Contoso.Deal",
  "companyName" : "Alpine Skis",
  "dealValue" : 1010100,
  "expirationDate" : "2015-07-03T13:04:00.000Z"
}
```

##### <a name="response-3"></a><span data-ttu-id="70e6c-219">応答 3</span><span class="sxs-lookup"><span data-stu-id="70e6c-219">Response 3</span></span>

<span data-ttu-id="70e6c-220">3 番目の例の要求からの応答を次に示します。</span><span class="sxs-lookup"><span data-stu-id="70e6c-220">Here is the response from the third example request.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.opentypeextension"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('f5480dfd-7d77-4d0b-ba2e-3391953cc74a')/events('AAMkADVl7IsAAA%3D')/extensions/$entity",
    "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Deal",
    "extensionName": "Com.Contoso.Deal",
    "companyName": "Alpine Skis",
    "dealValue": 1010100,
    "expirationDate": "2015-07-03T13:04:00Z"
}
```

****

##### <a name="request-4"></a><span data-ttu-id="70e6c-221">要求 4</span><span class="sxs-lookup"><span data-stu-id="70e6c-221">Request 4</span></span>

<span data-ttu-id="70e6c-p114">4 番目の例では、既存のグループ投稿に対する **reply** アクション呼び出しと同じ呼び出しを使用して、新しいグループ投稿に拡張情報を作成します。**reply** アクションは、新しい投稿と、投稿に埋め込まれる新しい拡張情報を作成します。要求本文には **post** プロパティが含まれます。そのプロパティには新しい投稿の **body** が含まれ、さらに新しい拡張情報の次のデータが含まれます。</span><span class="sxs-lookup"><span data-stu-id="70e6c-p114">The fourth example creates an extension in a new group post, using the same **reply** action call to an existing group post. The **reply** action creates a new post, and a new extension embedded in the post. The request body includes a **post** property, which in turn contains the **body** of the new post, and the following data for the new extension:</span></span>

- <span data-ttu-id="70e6c-225">型 `Microsoft.Graph.OpenTypeExtension`。</span><span class="sxs-lookup"><span data-stu-id="70e6c-225">The type `Microsoft.Graph.OpenTypeExtension`.</span></span> 
- <span data-ttu-id="70e6c-226">拡張情報名 "Com.Contoso.HR"。</span><span class="sxs-lookup"><span data-stu-id="70e6c-226">The extension name "Com.Contoso.HR".</span></span>
- <span data-ttu-id="70e6c-227">JSON ペイロードに 3 つのカスタム プロパティとして格納される追加のデータ: `companyName`、`expirationDate`、文字列 `topPicks` の配列。</span><span class="sxs-lookup"><span data-stu-id="70e6c-227">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `expirationDate`, and the array of strings `topPicks`.</span></span>

<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_4"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/threads('AAQkADJizZJpEWwqDHsEpV_KA==')/posts('AAMkADJiUg96QZUkA-ICwMubAAC1heiSAAA=')/microsoft.graph.reply 

{
  "post": {
    "body": {
      "contentType": "html",
      "content": "<html><body><div><div><div><div>When and where? </div></div></div></div></body></html>"
    },
  "extensions": [
    {
      "@odata.type": "Microsoft.OutlookServices.OpenTypeExtension",
      "extensionName": "Com.Contoso.HR",
      "companyName": "Contoso",
      "expirationDate": "2015-07-03T13:04:00.000Z",
      "topPicks": [
        "Employees only",
        "Add spouse or guest",
        "Add family"
      ]
    }
  ]        
  }
}
```

##### <a name="response-4"></a><span data-ttu-id="70e6c-228">応答 4</span><span class="sxs-lookup"><span data-stu-id="70e6c-228">Response 4</span></span>

<span data-ttu-id="70e6c-p115">4 番目の例の応答を次に示します。新しいグループ投稿に正常に拡張情報を作成できた場合は、HTTP 202 応答コードのみが生成されます。</span><span class="sxs-lookup"><span data-stu-id="70e6c-p115">Here is the response from the fourth example. Successfully creating an extension in a new group post results in only the HTTP 202 response code.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
Content-type: text/plain
Content-Length: 0
```


****

##### <a name="request-5"></a><span data-ttu-id="70e6c-231">要求 5</span><span class="sxs-lookup"><span data-stu-id="70e6c-231">Request 5</span></span>

<span data-ttu-id="70e6c-p116">5 番目の例では、会話を作成するための同じ POST 操作を使用して、新しいグループ投稿に拡張情報を作成します。POST 操作は、新しい会話、スレッドと投稿、投稿に埋め込まれた新しい拡張情報を作成します。要求本文には、**Topic** プロパティと **Threads** プロパティや、新しい会話の子 **post** オブジェクトが含まれます。次いで、その **post** オブジェクトには、新しい投稿の **body** と、拡張情報の次のデータが含まれます。</span><span class="sxs-lookup"><span data-stu-id="70e6c-p116">The fifth example creates an extension in a new group post using the same POST operation to create a conversation. The POST operation creates a new conversation, thread and post, and a new extension embedded in the post. The request body includes the **Topic** and **Threads** properties, and a child **post** object for the new conversation. The **post** object in turn contains the **body** of the new post, and the following data for the extension:</span></span>

- <span data-ttu-id="70e6c-236">型 `Microsoft.Graph.OpenTypeExtension`。</span><span class="sxs-lookup"><span data-stu-id="70e6c-236">The type `Microsoft.Graph.OpenTypeExtension`.</span></span> 
- <span data-ttu-id="70e6c-237">拡張情報名 "Com.Contoso.HR"。</span><span class="sxs-lookup"><span data-stu-id="70e6c-237">The extension name "Com.Contoso.HR".</span></span>
- <span data-ttu-id="70e6c-238">JSON ペイロードに 3 つのカスタム プロパティとして格納される追加のデータ: `companyName`、`expirationDate`、文字列 `topPicks` の配列。</span><span class="sxs-lookup"><span data-stu-id="70e6c-238">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `expirationDate`, and the array of strings `topPicks`.</span></span>

<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_5"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/conversations

{
  "Topic": "Does anyone have a second?",
  "Threads": [
    {
      "Posts": [
        {
          "Body": {
            "ContentType": "HTML",
            "Content": "This is urgent!"
          },
          "Extensions": [
            {
              "@odata.type": "Microsoft.OutlookServices.OpenTypeExtension",
              "extensionName": "Com.Contoso.Benefits",
              "companyName": "Contoso",
              "expirationDate": "2016-08-03T11:00:00.000Z",
              "topPicks": [
                "Employees only",
                "Add spouse or guest",
                "Add family"
              ]  
            }  
          ] 
        } 
      ]  
    } 
  ]
}
```

##### <a name="response-5"></a><span data-ttu-id="70e6c-239">応答 5</span><span class="sxs-lookup"><span data-stu-id="70e6c-239">Response 5</span></span>

<span data-ttu-id="70e6c-p117">5 番目の例の応答を次に示します。この応答には、新しい会話とスレッド ID が含まれています。この新しいスレッドには、自動的に作成された投稿が含まれ、その投稿に新しい拡張情報が含まれます。</span><span class="sxs-lookup"><span data-stu-id="70e6c-p117">Here is the response from the fifth example which contains the new conversation and a thread ID. This new thread contains an automatically created post, which in turn contains the new extension.</span></span> 

<span data-ttu-id="70e6c-p118">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="70e6c-p118">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<span data-ttu-id="70e6c-p119">新しい拡張情報を取得するには、まずこのスレッド内の[すべての投稿を取得](../api/conversationthread_list_posts.md)します。投稿は最初は 1 つしかありません。その後、投稿 ID と拡張情報名 `Com.Contoso.Benefits` を適用して、[拡張情報を取得](../api/opentypeextension_get.md)します。</span><span class="sxs-lookup"><span data-stu-id="70e6c-p119">To get the new extension, first [get all the posts](../api/conversationthread_list_posts.md) in this thread, and initially there should be only one. Then apply the post ID and the extension name `Com.Contoso.Benefits` to [get the extension](../api/opentypeextension_get.md).</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/conversations/$entity",
    "id": "AAQkADJToRlbJ5Mg7TFM7H-j3Y=",
    "threads@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/conversations('AAQkADJToRlbJ5Mg7TFM7H-j3Y%3D')/threads",
    "threads": [
        {
            "id": "AAQkADJDtMUzsf_PdhAAswJOhGVsnkyDtMUzsf_Pdg=="
        }
    ]
}

```


<!-- This page was manually created. -->
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create extension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
