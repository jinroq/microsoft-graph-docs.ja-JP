# <a name="create-open-extension"></a><span data-ttu-id="6c17e-101">オープン拡張機能を作成する</span><span class="sxs-lookup"><span data-stu-id="6c17e-101">Create open extension</span></span>

<span data-ttu-id="6c17e-102">オープン拡張機能 ([openTypeExtension](../resources/openTypeExtension.md) オブジェクト) を作成し、リソースの新規または既存のインスタンスのカスタム プロパティを追加します。</span><span class="sxs-lookup"><span data-stu-id="6c17e-102">Create an open extension ([openTypeExtension](../resources/openTypeExtension.md) object) and add custom properties in a new or existing instance of a resource.</span></span>

> <span data-ttu-id="6c17e-103">**注:** Outlook のリソースでオープン拡張機能を作成している場合は、「[openTypeExtension リソースの種類](../resources/opentypeextension.md#outlook-specific-considerations)」の 「**Outlook に固有の考慮事項**」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6c17e-103">**Note:** If you're creating open extensions on Outlook resources, see **Outlook-specific considerations** in [openTypeExtension resource type](../resources/opentypeextension.md#outlook-specific-considerations).</span></span>

## <a name="permissions"></a><span data-ttu-id="6c17e-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6c17e-104">Permissions</span></span>

<span data-ttu-id="6c17e-p101">この API を呼び出すには、拡張機能を作成するリソースに応じて、以下のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6c17e-p101">One of the following permissions is required to call this API, depending on the resource you're creating the extension in. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6c17e-107">**サポートされているリソース**</span><span class="sxs-lookup"><span data-stu-id="6c17e-107">**Supported resource**</span></span>|<span data-ttu-id="6c17e-108">**アクセス許可**</span><span class="sxs-lookup"><span data-stu-id="6c17e-108">**Permission**</span></span>|<span data-ttu-id="6c17e-109">**サポートされているリソース**</span><span class="sxs-lookup"><span data-stu-id="6c17e-109">**Supported resource**</span></span>|<span data-ttu-id="6c17e-110">**アクセス許可**</span><span class="sxs-lookup"><span data-stu-id="6c17e-110">**Permission**</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="6c17e-111">デバイス</span><span class="sxs-lookup"><span data-stu-id="6c17e-111">device</span></span>](../resources/device.md) | <span data-ttu-id="6c17e-112">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c17e-112">Device.ReadWrite.All</span></span> | [<span data-ttu-id="6c17e-113">イベント</span><span class="sxs-lookup"><span data-stu-id="6c17e-113">event</span></span>](../resources/event.md) | <span data-ttu-id="6c17e-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6c17e-114">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="6c17e-115">グループ</span><span class="sxs-lookup"><span data-stu-id="6c17e-115">group</span></span>](../resources/group.md) | <span data-ttu-id="6c17e-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c17e-116">Group.ReadWrite.All</span></span> | [<span data-ttu-id="6c17e-117">グループ イベント</span><span class="sxs-lookup"><span data-stu-id="6c17e-117">group event</span></span>](../resources/event.md) | <span data-ttu-id="6c17e-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c17e-118">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="6c17e-119">グループの投稿</span><span class="sxs-lookup"><span data-stu-id="6c17e-119">group post</span></span>](../resources/post.md) | <span data-ttu-id="6c17e-120">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c17e-120">Group.ReadWrite.All</span></span> | [<span data-ttu-id="6c17e-121">メッセージ</span><span class="sxs-lookup"><span data-stu-id="6c17e-121">message</span></span>](../resources/message.md) | <span data-ttu-id="6c17e-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6c17e-122">Mail.ReadWrite</span></span> |
| [<span data-ttu-id="6c17e-123">組織</span><span class="sxs-lookup"><span data-stu-id="6c17e-123">organization</span></span>](../resources/organization.md) | <span data-ttu-id="6c17e-124">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6c17e-124">Directory.AccessAsUser.All</span></span> | [<span data-ttu-id="6c17e-125">個人用連絡先</span><span class="sxs-lookup"><span data-stu-id="6c17e-125">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="6c17e-126">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6c17e-126">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="6c17e-127">ユーザー</span><span class="sxs-lookup"><span data-stu-id="6c17e-127">user</span></span>](../resources/user.md) | <span data-ttu-id="6c17e-128">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6c17e-128">Directory.AccessAsUser.All</span></span> | | |

## <a name="http-request"></a><span data-ttu-id="6c17e-129">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6c17e-129">HTTP request</span></span>

### <a name="create-an-extension-in-a-new-resource-instance"></a><span data-ttu-id="6c17e-130">新規のリソース インスタンスに拡張機能を作成する</span><span class="sxs-lookup"><span data-stu-id="6c17e-130">Create an extension in a new resource instance</span></span>

<span data-ttu-id="6c17e-131">インスタンスの作成に使用するのと同じ REST 要求を使用します。</span><span class="sxs-lookup"><span data-stu-id="6c17e-131">Use the same REST request that you use to create the instance.</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/events
POST /users/{id|userPrincipalName}/messages
POST /groups/{id}/events
POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /users/{id|userPrincipalName}/contacts
```

><span data-ttu-id="6c17e-132">**注:** この構文は、サポートされているリソース インスタンスを作成する一般的な方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="6c17e-132">**Note:** This syntax shows some common ways to create the supported resource instances.</span></span> <span data-ttu-id="6c17e-133">これらのリソース インスタンスの作成を許可するその他すべての POST 構文で、同様の方法でのオープン拡張機能の作成をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="6c17e-133">Note: The above syntax shows some common ways to create the supported resource instances. All other POST syntax that allows you to create these resource instances supports creating open extensions in them in a similar way.</span></span>

<span data-ttu-id="6c17e-134">要求本文に、新規のリソース インスタンスのプロパティ_および拡張機能_を含める方法については、[[要求本文](#request-body)] セクションを参照してください。</span><span class="sxs-lookup"><span data-stu-id="6c17e-134">See the [Request body](#request-body) section about including the properties of the new resource instance _and the extension_ in the request body.</span></span>

### <a name="create-an-extension-in-an-existing-resource-instance"></a><span data-ttu-id="6c17e-135">既存のリソース インスタンスに拡張機能を作成する</span><span class="sxs-lookup"><span data-stu-id="6c17e-135">Create an extension in an existing resource instance</span></span>

<span data-ttu-id="6c17e-136">要求でリソース インスタンスを識別し、**extensions** ナビゲーション プロパティで `POST` を行います。</span><span class="sxs-lookup"><span data-stu-id="6c17e-136">Identify the resource instance in the request and do a `POST` to the **extensions** navigation property.</span></span>

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

><span data-ttu-id="6c17e-137">**注:** この構文は、リソースのインスタンスを識別する一般的な方法を示しています。このリソース インスタンスで拡張機能を作成するためです。</span><span class="sxs-lookup"><span data-stu-id="6c17e-137">**Note:** The above syntax shows some common ways to identify a resource instance, in order to create an extension in it. All other syntax that allows you to identify these resource instances supports creating open extensions in them in a similar way.</span></span> <span data-ttu-id="6c17e-138">これらのリソース インスタンスの識別を許可するその他すべての構文は、同様の方法でのオープン拡張機能の作成をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="6c17e-138">Note: The above syntax shows some common ways to create the supported resource instances. All other POST syntax that allows you to create these resource instances supports creating open extensions in them in a similar way.</span></span>

<span data-ttu-id="6c17e-139">要求本文に_拡張機能_を含める方法については、[[要求本文](#request-body)] セクションを参照してください。</span><span class="sxs-lookup"><span data-stu-id="6c17e-139">See the [Request body](#request-body) section about including _the extension_ in the request body.</span></span>

## <a name="path-parameters"></a><span data-ttu-id="6c17e-140">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="6c17e-140">Path parameters</span></span>
|<span data-ttu-id="6c17e-141">パラメーター</span><span class="sxs-lookup"><span data-stu-id="6c17e-141">Parameter</span></span>|<span data-ttu-id="6c17e-142">型</span><span class="sxs-lookup"><span data-stu-id="6c17e-142">Type</span></span>|<span data-ttu-id="6c17e-143">説明</span><span class="sxs-lookup"><span data-stu-id="6c17e-143">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="6c17e-144">ID</span><span class="sxs-lookup"><span data-stu-id="6c17e-144">id</span></span>|<span data-ttu-id="6c17e-145">string</span><span class="sxs-lookup"><span data-stu-id="6c17e-145">string</span></span>|<span data-ttu-id="6c17e-p104">該当するコレクション内のオブジェクトの一意識別子。必須。</span><span class="sxs-lookup"><span data-stu-id="6c17e-p104">A unique identifier for an object in the corresponding collection. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="6c17e-148">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6c17e-148">Request headers</span></span>

| <span data-ttu-id="6c17e-149">名前</span><span class="sxs-lookup"><span data-stu-id="6c17e-149">Name</span></span>       | <span data-ttu-id="6c17e-150">値</span><span class="sxs-lookup"><span data-stu-id="6c17e-150">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="6c17e-151">承認</span><span class="sxs-lookup"><span data-stu-id="6c17e-151">Authorization</span></span> | <span data-ttu-id="6c17e-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6c17e-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6c17e-154">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6c17e-154">Content-Type</span></span> | <span data-ttu-id="6c17e-155">アプリケーション /json</span><span class="sxs-lookup"><span data-stu-id="6c17e-155">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="6c17e-156">要求本文</span><span class="sxs-lookup"><span data-stu-id="6c17e-156">Request body</span></span>

<span data-ttu-id="6c17e-p106">[openTypeExtension](../resources/openTypeExtension.md) の JSON 本文を、次の必須の名前と値の組や、その他のカスタム データとともに指定します。JSON ペイロード内のデータは、プリミティブ型か、プリミティブ型の配列にすることができます。</span><span class="sxs-lookup"><span data-stu-id="6c17e-p106">Provide a JSON body of an [openTypeExtension](../resources/openTypeExtension.md), with the following required name-value pairs, and any additional custom data. The data in the JSON payload can be primitive types, or arrays of primitive types.</span></span>

| <span data-ttu-id="6c17e-159">名前</span><span class="sxs-lookup"><span data-stu-id="6c17e-159">Name</span></span>       | <span data-ttu-id="6c17e-160">値</span><span class="sxs-lookup"><span data-stu-id="6c17e-160">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="6c17e-161">@odata.type</span><span class="sxs-lookup"><span data-stu-id="6c17e-161">@odata.type</span></span> | <span data-ttu-id="6c17e-162">Microsoft.Graph.OpenTypeExtension</span><span class="sxs-lookup"><span data-stu-id="6c17e-162">Microsoft.Graph.OpenTypeExtension</span></span> |
| <span data-ttu-id="6c17e-163">extensionName</span><span class="sxs-lookup"><span data-stu-id="6c17e-163">extensionName</span></span> | <span data-ttu-id="6c17e-164">%unique_string %</span><span class="sxs-lookup"><span data-stu-id="6c17e-164">%unique_string%</span></span> |

<span data-ttu-id="6c17e-165">_新しい_リソース インスタンスに拡張機能を作成するときは、新しい **openTypeExtension** オブジェクトに加えて、関連するプロパティの JSON 表現を指定して、このようなリソース インスタンスを作成します。</span><span class="sxs-lookup"><span data-stu-id="6c17e-165">When creating an extension in a _new_ resource instance, in addition to the new **openTypeExtension** object, provide a JSON representation of the relevant properties to create such a resource instance.</span></span>

## <a name="response"></a><span data-ttu-id="6c17e-166">応答</span><span class="sxs-lookup"><span data-stu-id="6c17e-166">Response</span></span>

### <a name="response-code"></a><span data-ttu-id="6c17e-167">応答コード</span><span class="sxs-lookup"><span data-stu-id="6c17e-167">Response code</span></span>

<span data-ttu-id="6c17e-168">操作によって、応答コードは `201 Created` または `202 Accepted` になります。</span><span class="sxs-lookup"><span data-stu-id="6c17e-168">Depending on the operation, the response code can be `201 Created` or `202 Accepted`.</span></span>

<span data-ttu-id="6c17e-169">リソース インスタンスの作成に使用するのと同じ操作で拡張機能を作成する場合は、その操作により、拡張機能なしでリソース インスタンスを作成するための操作を行う場合に返されるのと同じ応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="6c17e-169">When you create an extension using the same operation that you use to create a resource instance, the operation returns the same response code that it returns when you use the operation to create the resource instance without the extension.</span></span>
<span data-ttu-id="6c17e-170">[上記](#create-an-extension-in-a-new-resource-instance) で一覧表示されているとおり、インスタンスの作成に関する、対応するトピックスを参照してください。</span><span class="sxs-lookup"><span data-stu-id="6c17e-170">Refer to the corresponding topics for creating the instance, as listed [above](#create-an-extension-in-a-new-resource-instance).</span></span>

### <a name="response-body"></a><span data-ttu-id="6c17e-171">応答本文</span><span class="sxs-lookup"><span data-stu-id="6c17e-171">Response body</span></span>

| <span data-ttu-id="6c17e-172">シナリオ</span><span class="sxs-lookup"><span data-stu-id="6c17e-172">Scenario</span></span>       | <span data-ttu-id="6c17e-173">リソース</span><span class="sxs-lookup"><span data-stu-id="6c17e-173">Resource</span></span>  | <span data-ttu-id="6c17e-174">応答本文</span><span class="sxs-lookup"><span data-stu-id="6c17e-174">Response body</span></span> |
|:---------------|:----------|:--------------|
| <span data-ttu-id="6c17e-175">_新しい_リソース インスタンスを明示的に作成しながら、拡張機能を作成する</span><span class="sxs-lookup"><span data-stu-id="6c17e-175">Creating an extension while explicitly creating a _new_ resource instance</span></span> | <span data-ttu-id="6c17e-176">[連絡先](../resources/contact.md)、[イベント](../resources/event.md)、[メッセージ](../resources/message.md)</span><span class="sxs-lookup"><span data-stu-id="6c17e-176">[contact](../resources/contact.md), [event](../resources/event.md), [message](../resources/message.md)</span></span> | <span data-ttu-id="6c17e-177">[openTypeExtension](../resources/openTypeExtension.md) オブジェクトで展開した新しいインスタンスを含みます。</span><span class="sxs-lookup"><span data-stu-id="6c17e-177">Includes the new instance expanded with the [openTypeExtension](../resources/openTypeExtension.md) object.</span></span> |
| <span data-ttu-id="6c17e-178">新しいリソース インスタンスを暗示的に作成しながら、拡張機能を作成する</span><span class="sxs-lookup"><span data-stu-id="6c17e-178">Creating an extension while implicitly creating a resource instance</span></span> | [<span data-ttu-id="6c17e-179">post</span><span class="sxs-lookup"><span data-stu-id="6c17e-179">post</span></span>](../resources/post.md) | <span data-ttu-id="6c17e-180">応答には、応答コードだけが含まれ、応答本体は含まれません。</span><span class="sxs-lookup"><span data-stu-id="6c17e-180">The response includes only a response code but not a response body.</span></span> |
| <span data-ttu-id="6c17e-181">_既存_のリソース インスタンスに拡張機能を作成する</span><span class="sxs-lookup"><span data-stu-id="6c17e-181">Creating an extension in an _existing_ resource instance</span></span> | <span data-ttu-id="6c17e-182">サポートされているすべてのリソース</span><span class="sxs-lookup"><span data-stu-id="6c17e-182">All supported resources</span></span> | <span data-ttu-id="6c17e-183">**openTypeExtension** オブジェクトが含まれます。</span><span class="sxs-lookup"><span data-stu-id="6c17e-183">Includes the **openTypeExtension** object.</span></span> |

## <a name="example"></a><span data-ttu-id="6c17e-184">例</span><span class="sxs-lookup"><span data-stu-id="6c17e-184">Example</span></span>

### <a name="request-1"></a><span data-ttu-id="6c17e-185">要求 1</span><span class="sxs-lookup"><span data-stu-id="6c17e-185">Request 1</span></span>

<span data-ttu-id="6c17e-p108">最初の例では、同一の呼び出しでメッセージと拡張情報を作成します。要求本文には、次のものが含まれます。</span><span class="sxs-lookup"><span data-stu-id="6c17e-p108">The first example creates a message and an extension in the same call. The request body includes the following:</span></span>

- <span data-ttu-id="6c17e-188">新しいメッセージ固有の **subject**、**body**、**toRecipients** プロパティ。</span><span class="sxs-lookup"><span data-stu-id="6c17e-188">The **subject**, **body**, and **toRecipients** properties typical of a new message.</span></span>
- <span data-ttu-id="6c17e-189">拡張情報に関する次のもの。</span><span class="sxs-lookup"><span data-stu-id="6c17e-189">And for the extension:</span></span>

  - <span data-ttu-id="6c17e-190">型 `microsoft.graph.openTypeExtension`。</span><span class="sxs-lookup"><span data-stu-id="6c17e-190">The type `microsoft.graph.openTypeExtension`.</span></span>
  - <span data-ttu-id="6c17e-191">拡張情報名 "Com.Contoso.Referral" 。</span><span class="sxs-lookup"><span data-stu-id="6c17e-191">The extension name "Com.Contoso.Referral".</span></span>
  - <span data-ttu-id="6c17e-192">JSON ペイロードに 3 つのカスタム プロパティとして格納される追加のデータ: `companyName`、`expirationDate`、`dealValue`。</span><span class="sxs-lookup"><span data-stu-id="6c17e-192">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `expirationDate`, and `dealValue`.</span></span>

<!-- {
  "blockType": "ignored",
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
      "@odata.type": "microsoft.graph.openTypeExtension",
      "extensionName": "Com.Contoso.Referral",
      "companyName": "Wingtip Toys",
      "expirationDate": "2015-12-30T11:00:00.000Z",
      "dealValue": 10000
    }
  ]
}
```

### <a name="response-1"></a><span data-ttu-id="6c17e-193">応答 1</span><span class="sxs-lookup"><span data-stu-id="6c17e-193">Response 1</span></span>

<span data-ttu-id="6c17e-p109">最初の例の応答を次に示します。応答本文には、新しいメッセージのプロパティと、新しい拡張情報に関する次のものが含まれています。</span><span class="sxs-lookup"><span data-stu-id="6c17e-p109">Here is the response for the first example. The response body includes properties of the new message, and the following for the new extension:</span></span>

- <span data-ttu-id="6c17e-196">**id** プロパティと `Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral` の完全修飾名。</span><span class="sxs-lookup"><span data-stu-id="6c17e-196">The **id** property with the fully qualified name of `Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral`.</span></span>
- <span data-ttu-id="6c17e-197">要求で指定されている既定のプロパティ **extensionName**。</span><span class="sxs-lookup"><span data-stu-id="6c17e-197">The default property **extensionName** specified in the request.</span></span>
- <span data-ttu-id="6c17e-198">要求で指定されている、3 つのカスタム プロパティとして格納されるカスタム データ。</span><span class="sxs-lookup"><span data-stu-id="6c17e-198">The custom data specified in the request stored as 3 custom properties.</span></span>

<span data-ttu-id="6c17e-p110">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="6c17e-p110">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "@odata.type": "#microsoft.graph.openTypeExtension",
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

### <a name="request-2"></a><span data-ttu-id="6c17e-201">要求 2</span><span class="sxs-lookup"><span data-stu-id="6c17e-201">Request 2</span></span>

<span data-ttu-id="6c17e-p111">2 番目の例では、指定されたメッセージに拡張情報を作成します。要求本文には、拡張情報に関する次のものが含まれます。</span><span class="sxs-lookup"><span data-stu-id="6c17e-p111">The second example creates an extension in the specified message. The request body includes the following for the extension:</span></span>

- <span data-ttu-id="6c17e-204">型 `microsoft.graph.openTypeExtension`。</span><span class="sxs-lookup"><span data-stu-id="6c17e-204">The type `microsoft.graph.openTypeExtension`.</span></span>
- <span data-ttu-id="6c17e-205">拡張情報名 "Com.Contoso.Referral" 。</span><span class="sxs-lookup"><span data-stu-id="6c17e-205">The extension name "Com.Contoso.Referral".</span></span>
- <span data-ttu-id="6c17e-206">JSON ペイロードに 3 つのカスタム プロパティとして格納される追加のデータ: `companyName`、`dealValue`、`expirationDate`。</span><span class="sxs-lookup"><span data-stu-id="6c17e-206">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `dealValue`, and `expirationDate`.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "post_opentypeextension_2"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions

{
  "@odata.type" : "microsoft.graph.openTypeExtension",
  "extensionName" : "Com.Contoso.Referral",
  "companyName" : "Wingtip Toys",
  "dealValue" : 500050,
  "expirationDate" : "2015-12-03T10:00:00.000Z"
}
```

### <a name="response-2"></a><span data-ttu-id="6c17e-207">応答 2</span><span class="sxs-lookup"><span data-stu-id="6c17e-207">Response 2</span></span>

<span data-ttu-id="6c17e-p112">2 番目の例の応答を次に示します。応答本文には、新しい拡張情報に関する次のものが含まれています。</span><span class="sxs-lookup"><span data-stu-id="6c17e-p112">Here is the response for the second example. The response body includes the following for the new extension:</span></span>

- <span data-ttu-id="6c17e-210">既定のプロパティ **extensionName**。</span><span class="sxs-lookup"><span data-stu-id="6c17e-210">The default property **extensionName**.</span></span>
- <span data-ttu-id="6c17e-211">**id** プロパティと `Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral` の完全修飾名。</span><span class="sxs-lookup"><span data-stu-id="6c17e-211">The **id** property with the fully qualified name of `Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral`.</span></span>
- <span data-ttu-id="6c17e-212">格納されるカスタム データ。</span><span class="sxs-lookup"><span data-stu-id="6c17e-212">The custom data to be stored.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.openTypeExtension"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
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

### <a name="request-3"></a><span data-ttu-id="6c17e-213">要求 3</span><span class="sxs-lookup"><span data-stu-id="6c17e-213">Request 3</span></span>

<span data-ttu-id="6c17e-p113">3 番目の例では、指定されたグループ イベントに拡張情報を作成します。要求本文には、拡張情報に関する次のものが含まれます。</span><span class="sxs-lookup"><span data-stu-id="6c17e-p113">The third example creates an extension in the specified group event. The request body includes the following for the extension:</span></span>

- <span data-ttu-id="6c17e-216">型 `microsoft.graph.openTypeExtension`。</span><span class="sxs-lookup"><span data-stu-id="6c17e-216">The type `microsoft.graph.openTypeExtension`.</span></span>
- <span data-ttu-id="6c17e-217">拡張情報名 "Com.Contoso.Deal"。</span><span class="sxs-lookup"><span data-stu-id="6c17e-217">The extension name "Com.Contoso.Deal".</span></span>
- <span data-ttu-id="6c17e-218">JSON ペイロードに 3 つのカスタム プロパティとして格納される追加のデータ: `companyName`、`dealValue`、`expirationDate`。</span><span class="sxs-lookup"><span data-stu-id="6c17e-218">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `dealValue`, and `expirationDate`.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "post_opentypeextension_3"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/f5480dfd-7d77-4d0b-ba2e-3391953cc74a/events/AAMkADVl17IsAAA=/extensions

{
  "@odata.type" : "microsoft.graph.openTypeExtension",
  "extensionName" : "Com.Contoso.Deal",
  "companyName" : "Alpine Skis",
  "dealValue" : 1010100,
  "expirationDate" : "2015-07-03T13:04:00.000Z"
}
```

### <a name="response-3"></a><span data-ttu-id="6c17e-219">応答 3</span><span class="sxs-lookup"><span data-stu-id="6c17e-219">Response 3</span></span>

<span data-ttu-id="6c17e-220">3 番目の例の要求からの応答を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6c17e-220">Here is the response from the third example request.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.openTypeExtension"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('f5480dfd-7d77-4d0b-ba2e-3391953cc74a')/events('AAMkADVl7IsAAA%3D')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Deal",
    "extensionName": "Com.Contoso.Deal",
    "companyName": "Alpine Skis",
    "dealValue": 1010100,
    "expirationDate": "2015-07-03T13:04:00Z"
}
```

****

### <a name="request-4"></a><span data-ttu-id="6c17e-221">要求 4</span><span class="sxs-lookup"><span data-stu-id="6c17e-221">Request 4</span></span>

<span data-ttu-id="6c17e-p114">4 番目の例では、既存のグループ投稿に対する **reply** アクション呼び出しと同じ呼び出しを使用して、新しいグループ投稿に拡張情報を作成します。**reply** アクションは、新しい投稿と、投稿に埋め込まれる新しい拡張情報を作成します。要求本文には **post** プロパティが含まれます。そのプロパティには新しい投稿の **body** が含まれ、さらに新しい拡張情報の次のデータが含まれます。</span><span class="sxs-lookup"><span data-stu-id="6c17e-p114">The fourth example creates an extension in a new group post, using the same **reply** action call to an existing group post. The **reply** action creates a new post, and a new extension embedded in the post. The request body includes a **post** property, which in turn contains the **body** of the new post, and the following data for the new extension:</span></span>

- <span data-ttu-id="6c17e-225">型 `microsoft.graph.openTypeExtension`。</span><span class="sxs-lookup"><span data-stu-id="6c17e-225">The type `microsoft.graph.openTypeExtension`.</span></span>
- <span data-ttu-id="6c17e-226">拡張情報名 "Com.Contoso.HR"。</span><span class="sxs-lookup"><span data-stu-id="6c17e-226">The extension name "Com.Contoso.HR".</span></span>
- <span data-ttu-id="6c17e-227">JSON ペイロードに 3 つのカスタム プロパティとして格納される追加のデータ: `companyName`、`expirationDate`、文字列 `topPicks` の配列。</span><span class="sxs-lookup"><span data-stu-id="6c17e-227">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `expirationDate`, and the array of strings `topPicks`.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "post_opentypeextension_4"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/37df2ff0-0de0-4c33-8aee-75289364aef6/threads/AAQkADJizZJpEWwqDHsEpV_KA==/posts/AAMkADJiUg96QZUkA-ICwMubAAC1heiSAAA=/reply

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

### <a name="response-4"></a><span data-ttu-id="6c17e-228">応答 4</span><span class="sxs-lookup"><span data-stu-id="6c17e-228">Response 4</span></span>

<span data-ttu-id="6c17e-p115">4 番目の例の応答を次に示します。新しいグループ投稿に正常に拡張情報を作成できた場合は、HTTP 202 応答コードのみが生成されます。</span><span class="sxs-lookup"><span data-stu-id="6c17e-p115">Here is the response from the fourth example. Successfully creating an extension in a new group post results in only the HTTP 202 response code.</span></span>

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

### <a name="request-5"></a><span data-ttu-id="6c17e-231">要求 5</span><span class="sxs-lookup"><span data-stu-id="6c17e-231">Request 5</span></span>

<span data-ttu-id="6c17e-p116">5 番目の例では、会話を作成するための同じ POST 操作を使用して、新しいグループ投稿に拡張情報を作成します。POST 操作は、新しい会話、スレッドと投稿、投稿に埋め込まれた新しい拡張情報を作成します。要求本文には、**Topic** プロパティと **Threads** プロパティや、新しい会話の子 **post** オブジェクトが含まれます。次いで、その **post** オブジェクトには、新しい投稿の **body** と、拡張情報の次のデータが含まれます。</span><span class="sxs-lookup"><span data-stu-id="6c17e-p116">The fifth example creates an extension in a new group post using the same POST operation to create a conversation. The POST operation creates a new conversation, thread and post, and a new extension embedded in the post. The request body includes the **Topic** and **Threads** properties, and a child **post** object for the new conversation. The **post** object in turn contains the **body** of the new post, and the following data for the extension:</span></span>

- <span data-ttu-id="6c17e-236">型 `microsoft.graph.openTypeExtension`。</span><span class="sxs-lookup"><span data-stu-id="6c17e-236">The type `microsoft.graph.openTypeExtension`.</span></span>
- <span data-ttu-id="6c17e-237">拡張情報名 "Com.Contoso.HR"。</span><span class="sxs-lookup"><span data-stu-id="6c17e-237">The extension name "Com.Contoso.HR".</span></span>
- <span data-ttu-id="6c17e-238">JSON ペイロードに 3 つのカスタム プロパティとして格納される追加のデータ: `companyName`、`expirationDate`、文字列 `topPicks` の配列。</span><span class="sxs-lookup"><span data-stu-id="6c17e-238">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `expirationDate`, and the array of strings `topPicks`.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "post_opentypeextension_5"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/37df2ff0-0de0-4c33-8aee-75289364aef6/conversations

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

### <a name="response-5"></a><span data-ttu-id="6c17e-239">応答 5</span><span class="sxs-lookup"><span data-stu-id="6c17e-239">Response 5</span></span>

<span data-ttu-id="6c17e-p117">5 番目の例の応答を次に示します。この応答には、新しい会話とスレッド ID が含まれています。この新しいスレッドには、自動的に作成された投稿が含まれ、その投稿に新しい拡張情報が含まれます。</span><span class="sxs-lookup"><span data-stu-id="6c17e-p117">Here is the response from the fifth example which contains the new conversation and a thread ID. This new thread contains an automatically created post, which in turn contains the new extension.</span></span>

<span data-ttu-id="6c17e-p118">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="6c17e-p118">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<span data-ttu-id="6c17e-p119">新しい拡張情報を取得するには、まずこのスレッド内の[すべての投稿を取得](../api/conversationthread_list_posts.md)します。投稿は最初は 1 つしかありません。その後、投稿 ID と拡張情報名 `Com.Contoso.Benefits` を適用して、[拡張情報を取得](../api/opentypeextension_get.md)します。</span><span class="sxs-lookup"><span data-stu-id="6c17e-p119">To get the new extension, first [get all the posts](../api/conversationthread_list_posts.md) in this thread, and initially there should be only one. Then apply the post ID and the extension name `Com.Contoso.Benefits` to [get the extension](../api/opentypeextension_get.md).</span></span>

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
