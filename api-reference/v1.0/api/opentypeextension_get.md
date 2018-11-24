# <a name="get-open-extension"></a><span data-ttu-id="7adde-101">オープン拡張機能を取得する</span><span class="sxs-lookup"><span data-stu-id="7adde-101">Get open extension</span></span>

<span data-ttu-id="7adde-102">名前または完全修飾名で識別されたオープン拡張機能 ([openTypeExtension](../resources/openTypeExtension.md) オブジェクト) を取得します。</span><span class="sxs-lookup"><span data-stu-id="7adde-102">Get an open extension ([openTypeExtension](../resources/openTypeExtension.md) object) identified by name or fully qualified name.</span></span>

<span data-ttu-id="7adde-103">次の表は、サポートされているリソース インスタンスからオープン拡張機能を取得できる 3 つのシナリオの一覧です。</span><span class="sxs-lookup"><span data-stu-id="7adde-103">The following table lists the three scenarios where you can get an open extension from a supported resource instance.</span></span>

|<span data-ttu-id="7adde-104">**GET シナリオ**</span><span class="sxs-lookup"><span data-stu-id="7adde-104">**GET scenario**</span></span>|<span data-ttu-id="7adde-105">**サポートされているリソース**</span><span class="sxs-lookup"><span data-stu-id="7adde-105">**Supported resources**</span></span>|<span data-ttu-id="7adde-106">**応答本文**</span><span class="sxs-lookup"><span data-stu-id="7adde-106">**Response body**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="7adde-107">既知のリソース インスタンスから特定の拡張機能を取得します。</span><span class="sxs-lookup"><span data-stu-id="7adde-107">Get a specific extension from a known resource instance.</span></span>| <span data-ttu-id="7adde-108">[デバイス](../resources/device.md)、[イベント](../resources/event.md)、[グループ](../resources/group.md)、[グループ イベント](../resources/event.md)、[グループの投稿](../resources/post.md)、[メッセージ](../resources/message.md)、[組織](../resources/organization.md)、[個人用連絡先](../resources/contact.md)、[ユーザー](../resources/user.md)</span><span class="sxs-lookup"><span data-stu-id="7adde-108">[Device](../resources/device.md), [event](../resources/event.md), [group](../resources/group.md), [group event](../resources/event.md), [group post](../resources/post.md), [message](../resources/message.md), [organization](../resources/organization.md), [personal contact](../resources/contact.md), [user](../resources/user.md)</span></span> | <span data-ttu-id="7adde-109">オープン拡張機能のみ。</span><span class="sxs-lookup"><span data-stu-id="7adde-109">Open extension only.</span></span>|
|<span data-ttu-id="7adde-110">特定の拡張機能で展開された既知のリソース インスタンスを取得します。</span><span class="sxs-lookup"><span data-stu-id="7adde-110">Get a known resource instance expanded with a specific extension.</span></span>|<span data-ttu-id="7adde-111">デバイス、イベント、グループ、グループ イベント、グループの投稿、メッセージ、組織、個人用連絡先、ユーザー</span><span class="sxs-lookup"><span data-stu-id="7adde-111">Device, event, group, group event, group post, message, organization, personal contact, user</span></span> |<span data-ttu-id="7adde-112">オープン拡張機能で展開されたリソース インスタンス。</span><span class="sxs-lookup"><span data-stu-id="7adde-112">A resource instance expanded with the open extension.</span></span>|
|<span data-ttu-id="7adde-113">特定の拡張機能でリソース インスタンスを検索し、展開します。</span><span class="sxs-lookup"><span data-stu-id="7adde-113">Find and expand resource instances with a specific extension.</span></span> |<span data-ttu-id="7adde-114">イベント、グループ イベント、グループの投稿、メッセージ、個人用連絡先</span><span class="sxs-lookup"><span data-stu-id="7adde-114">Event, group event, group post, message, personal contact</span></span>|<span data-ttu-id="7adde-115">オープン拡張機能で展開されたリソース インスタンス。</span><span class="sxs-lookup"><span data-stu-id="7adde-115">Resource instances expanded with the open extension.</span></span>|

## <a name="permissions"></a><span data-ttu-id="7adde-116">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7adde-116">Permissions</span></span>

<span data-ttu-id="7adde-117">拡張機能とアクセス許可が含まれるリソースによって委任された (アプリケーション) の種類を要求、次の表で指定されたアクセス許可は、この API を呼び出すために必要最低限の特権。</span><span class="sxs-lookup"><span data-stu-id="7adde-117">Depending on the resource that contains the extension and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="7adde-118">アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7adde-118">To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="7adde-119">サポートされているリソース</span><span class="sxs-lookup"><span data-stu-id="7adde-119">Supported resource</span></span> | <span data-ttu-id="7adde-120">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7adde-120">Delegated (work or school account)</span></span> | <span data-ttu-id="7adde-121">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7adde-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7adde-122">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7adde-122">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="7adde-123">device</span><span class="sxs-lookup"><span data-stu-id="7adde-123">device</span></span>](../resources/device.md) | <span data-ttu-id="7adde-124">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="7adde-124">Directory.Read.All</span></span> | <span data-ttu-id="7adde-125">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="7adde-125">Not supported</span></span> | <span data-ttu-id="7adde-126">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7adde-126">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="7adde-127">イベント</span><span class="sxs-lookup"><span data-stu-id="7adde-127">event</span></span>](../resources/event.md) | <span data-ttu-id="7adde-128">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="7adde-128">Calendars.Read</span></span> | <span data-ttu-id="7adde-129">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="7adde-129">Calendars.Read</span></span> | <span data-ttu-id="7adde-130">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="7adde-130">Calendars.Read</span></span> |
| [<span data-ttu-id="7adde-131">group</span><span class="sxs-lookup"><span data-stu-id="7adde-131">group</span></span>](../resources/group.md) | <span data-ttu-id="7adde-132">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="7adde-132">Group.Read.All</span></span> | <span data-ttu-id="7adde-133">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="7adde-133">Not supported</span></span> | <span data-ttu-id="7adde-134">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="7adde-134">Group.Read.All</span></span> |
| [<span data-ttu-id="7adde-135">グループ イベント</span><span class="sxs-lookup"><span data-stu-id="7adde-135">group event</span></span>](../resources/event.md) | <span data-ttu-id="7adde-136">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="7adde-136">Group.Read.All</span></span> | <span data-ttu-id="7adde-137">使用不可</span><span class="sxs-lookup"><span data-stu-id="7adde-137">Not supported</span></span> | <span data-ttu-id="7adde-138">使用不可</span><span class="sxs-lookup"><span data-stu-id="7adde-138">Not supported</span></span> |
| [<span data-ttu-id="7adde-139">グループの投稿</span><span class="sxs-lookup"><span data-stu-id="7adde-139">group post</span></span>](../resources/post.md) | <span data-ttu-id="7adde-140">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="7adde-140">Group.Read.All</span></span> | <span data-ttu-id="7adde-141">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="7adde-141">Not supported</span></span> | <span data-ttu-id="7adde-142">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="7adde-142">Group.Read.All</span></span> |
| [<span data-ttu-id="7adde-143">message</span><span class="sxs-lookup"><span data-stu-id="7adde-143">message</span></span>](../resources/message.md) | <span data-ttu-id="7adde-144">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="7adde-144">Mail.Read</span></span> | <span data-ttu-id="7adde-145">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="7adde-145">Mail.Read</span></span> | <span data-ttu-id="7adde-146">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="7adde-146">Mail.Read</span></span> | 
| [<span data-ttu-id="7adde-147">organization</span><span class="sxs-lookup"><span data-stu-id="7adde-147">organization</span></span>](../resources/organization.md) | <span data-ttu-id="7adde-148">User.Read</span><span class="sxs-lookup"><span data-stu-id="7adde-148">User.Read</span></span> | <span data-ttu-id="7adde-149">使用不可</span><span class="sxs-lookup"><span data-stu-id="7adde-149">Not supported</span></span> | <span data-ttu-id="7adde-150">使用不可</span><span class="sxs-lookup"><span data-stu-id="7adde-150">Not supported</span></span> |
| [<span data-ttu-id="7adde-151">個人用連絡先</span><span class="sxs-lookup"><span data-stu-id="7adde-151">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="7adde-152">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="7adde-152">Contacts.Read</span></span> | <span data-ttu-id="7adde-153">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="7adde-153">Contacts.Read</span></span> | <span data-ttu-id="7adde-154">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="7adde-154">Contacts.Read</span></span> |
| [<span data-ttu-id="7adde-155">user</span><span class="sxs-lookup"><span data-stu-id="7adde-155">user</span></span>](../resources/user.md) | <span data-ttu-id="7adde-156">User.Read</span><span class="sxs-lookup"><span data-stu-id="7adde-156">User.Read</span></span> | <span data-ttu-id="7adde-157">User.Read</span><span class="sxs-lookup"><span data-stu-id="7adde-157">User.Read</span></span> | <span data-ttu-id="7adde-158">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="7adde-158">User.Read.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="7adde-159">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7adde-159">HTTP request</span></span>

<span data-ttu-id="7adde-160">このセクションでは、前述の 3 つの `GET` シナリオの構文について説明します。</span><span class="sxs-lookup"><span data-stu-id="7adde-160">This section lists the syntax for each of the three `GET` scenarios described above.</span></span>

### <a name="get-a-specific-extension-in-a-known-resource-instance"></a><span data-ttu-id="7adde-161">既知のリソース インスタンス内の特定の拡張機能を取得する</span><span class="sxs-lookup"><span data-stu-id="7adde-161">Get a specific extension in a known resource instance</span></span>

<span data-ttu-id="7adde-162">リソース インスタンスを取得するのと同じ REST 要求を使用し、そのインスタンスの **extensions** ナビゲーション プロパティを使用して拡張機能を識別します。</span><span class="sxs-lookup"><span data-stu-id="7adde-162">Use the same REST request as getting the resource instance, and identify the extension using the **extensions** navigation property of that instance.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /devices/{Id}/extensions/{extensionId}
GET /users/{Id|userPrincipalName}/events/{Id}/extensions/{extensionId}
GET /groups/{Id}/extensions/{extensionId}
GET /groups/{Id}/events/{Id}/extensions/{extensionId}
GET /groups/{Id}/threads/{Id}/posts/{Id}/extensions/{extensionId}
GET /users/{Id|userPrincipalName}/messages/{Id}/extensions/{extensionId}
GET /organization/{Id}/extensions/{extensionId}
GET /users/{Id|userPrincipalName}/contacts/{Id}/extensions/{extensionId}
GET /users/{Id|userPrincipalName}/extensions/{extensionId}
```


### <a name="get-a-known-resource-instance-expanded-with-a-matching-extension"></a><span data-ttu-id="7adde-163">一致する拡張機能で展開された既知のリソース インスタンスを取得する</span><span class="sxs-lookup"><span data-stu-id="7adde-163">Get a known resource instance expanded with a matching extension</span></span> 

<span data-ttu-id="7adde-p102">イベント、グループ イベント、グループの投稿、メッセージ、個人用連絡先のリソースの種類に関しては、リソース インスタンスを取得するのと同じ REST 要求を使用して、そのインスタンスの **id** プロパティのフィルターに一致する拡張機能を検索し、拡張機能でインスタンスを展開できます。応答には、リソース プロパティのほとんどが含まれています。</span><span class="sxs-lookup"><span data-stu-id="7adde-p102">For the event, group event, group post, message, personal contact resource types, you can use the same REST request as getting the resource instance, look for an extension that matches a filter on its **id** property, and expand the instance with the extension. The response includes most of the resource properties.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Id|userPrincipalName}/events/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /groups/{Id}/events/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /groups/{Id}/threads/{Id}/posts/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/messages/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/contacts/{Id}?$expand=extensions($filter=id eq '{extensionId}')
```


<span data-ttu-id="7adde-166">デバイス、グループ、組織、ユーザーのリソースの種類に関しては、リソース インスタンスから **id** プロパティやその他のプロパティを含めるために、`$select` パラメーターを使用する必要もあります。</span><span class="sxs-lookup"><span data-stu-id="7adde-166">For the device, group, organization, and user resource types, you must also use a `$select` parameter to include the **id** property and any other properties you want from the resource instance:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /devices/{Id}?$expand=extensions($filter=id eq '{extensionId}')&$select=id,{property_1},{property_n}
GET /groups/{Id}?$expand=extensions($filter=id eq '{extensionId}')&$select=id,{property_1},{property_n}
GET /organization/{Id}?$expand=extensions($filter=id eq '{extensionId}')&$select=id,{property_1},{property_n}
GET /users/{Id|userPrincipalName}?$expand=extensions($filter=id eq '{extensionId}')&$select=id,{property_1},{property_n}
```

### <a name="filter-for-resource-instances-expanded-with-a-matching-extension"></a><span data-ttu-id="7adde-167">一致する拡張機能で展開されたリソース インスタンスにフィルターをかける</span><span class="sxs-lookup"><span data-stu-id="7adde-167">Filter for resource instances expanded with a matching extension</span></span> 

<span data-ttu-id="7adde-168">サポートされているリソースのコレクションを取得するのと同じ REST 要求を使用して、対応する **id** プロパティの拡張機能を含むインスタンスのコレクションにフィルターをかけ、拡張機能でこれらのインスタンスを展開します。</span><span class="sxs-lookup"><span data-stu-id="7adde-168">Use the same REST request as getting a collection of the supported resource, filter the collection for instances that contain an extension with a matching **id** property, and expand these instances with the extension.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Id|userPrincipalName}/events?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
GET /groups/{Id}/events?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
GET /groups/{Id}/threads/{Id}/posts?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/messages?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/contacts?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
```

><span data-ttu-id="7adde-p103">**注:** 上記の構文は、拡張機能の取得元となるリソース インスタンスまたはコレクションを特定する一般的な方法を示しています。こうしたリソース インスタンスまたはコレクションを特定するために使用できる他の構文すべても、同様の方法でオープン拡張機能を取得できます。</span><span class="sxs-lookup"><span data-stu-id="7adde-p103">**Note:** The above syntax shows some common ways to identify a resource instance or collection, in order to get an extension from it. All other syntax that allows you to identify these resource instances or collections supports getting open extensions from them in a similar way.</span></span>

## <a name="path-parameters"></a><span data-ttu-id="7adde-171">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="7adde-171">Path parameters</span></span>
|<span data-ttu-id="7adde-172">パラメーター</span><span class="sxs-lookup"><span data-stu-id="7adde-172">Parameter</span></span>|<span data-ttu-id="7adde-173">型</span><span class="sxs-lookup"><span data-stu-id="7adde-173">Type</span></span>|<span data-ttu-id="7adde-174">説明</span><span class="sxs-lookup"><span data-stu-id="7adde-174">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="7adde-175">Id</span><span class="sxs-lookup"><span data-stu-id="7adde-175">Id</span></span>|<span data-ttu-id="7adde-176">文字列</span><span class="sxs-lookup"><span data-stu-id="7adde-176">string</span></span>|<span data-ttu-id="7adde-p104">メッセージ、イベント、連絡先などの対応するコレクションに含まれるオブジェクトの一意識別子を格納するプレースホルダー。必須。**openTypeExtension** の **id** プロパティと混同しないこと。</span><span class="sxs-lookup"><span data-stu-id="7adde-p104">Placeholder for a unique identifier for an object in the corresponding collection such as messages, events, contacts. Required. Not to be confused with the **id** property of an **openTypeExtension**.</span></span>|
|<span data-ttu-id="7adde-180">extensionId</span><span class="sxs-lookup"><span data-stu-id="7adde-180">extensionId</span></span>|<span data-ttu-id="7adde-181">文字列</span><span class="sxs-lookup"><span data-stu-id="7adde-181">string</span></span>|<span data-ttu-id="7adde-p105">拡張情報名を表すプレースホルダー。これは、拡張情報の一意のテキスト識別子であるか、拡張情報の種類と一意のテキスト識別子を連結した完全修飾名のいずれかです。完全修飾名は、拡張情報の作成時に **id** プロパティに入れて返されます。必須。</span><span class="sxs-lookup"><span data-stu-id="7adde-p105">Placeholder for an extension name which is a unique text identifier for an extension, or a fully qualified name which concatenates the extension type and unique text identifier. The fully qualified name is returned in the **id** property when you create the extension. Required.</span></span>|

## <a name="optional-query-parameters"></a><span data-ttu-id="7adde-185">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="7adde-185">Optional query parameters</span></span>

<span data-ttu-id="7adde-186">`$filter` 文字列内のスペース文字には必ず [URL エンコード](https://www.w3schools.com/tags/ref_urlencode.asp)を適用してください。</span><span class="sxs-lookup"><span data-stu-id="7adde-186">Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the `$filter` string.</span></span>

|<span data-ttu-id="7adde-187">名前</span><span class="sxs-lookup"><span data-stu-id="7adde-187">Name</span></span>|<span data-ttu-id="7adde-188">値</span><span class="sxs-lookup"><span data-stu-id="7adde-188">Value</span></span>|<span data-ttu-id="7adde-189">説明</span><span class="sxs-lookup"><span data-stu-id="7adde-189">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="7adde-190">$filter</span><span class="sxs-lookup"><span data-stu-id="7adde-190">$filter</span></span>|<span data-ttu-id="7adde-191">文字列</span><span class="sxs-lookup"><span data-stu-id="7adde-191">string</span></span>|<span data-ttu-id="7adde-192">**id** が `extensionId` パラメーターの値と一致する拡張情報を返します。</span><span class="sxs-lookup"><span data-stu-id="7adde-192">Returns an extension with its **id** matching the `extensionId` parameter value.</span></span>|
|<span data-ttu-id="7adde-193">$filter with **any** operator</span><span class="sxs-lookup"><span data-stu-id="7adde-193">$filter with **any** operator</span></span>|<span data-ttu-id="7adde-194">文字列</span><span class="sxs-lookup"><span data-stu-id="7adde-194">string</span></span>|<span data-ttu-id="7adde-195">**id** が `extensionId` パラメーターの値と一致する拡張情報を含むリソース コレクションのインスタンスを返します。</span><span class="sxs-lookup"><span data-stu-id="7adde-195">Returns instances of a resource collection that contain an extension with its **id** matching the `extensionId` parameter value.</span></span>|
|<span data-ttu-id="7adde-196">$expand</span><span class="sxs-lookup"><span data-stu-id="7adde-196">$expand</span></span>|<span data-ttu-id="7adde-197">文字列</span><span class="sxs-lookup"><span data-stu-id="7adde-197">string</span></span>|<span data-ttu-id="7adde-198">リソース インスタンスを展開して、拡張情報を組み込みます。</span><span class="sxs-lookup"><span data-stu-id="7adde-198">Expands a resource instance to include an extension.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="7adde-199">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7adde-199">Request headers</span></span>
| <span data-ttu-id="7adde-200">名前</span><span class="sxs-lookup"><span data-stu-id="7adde-200">Name</span></span>       | <span data-ttu-id="7adde-201">値</span><span class="sxs-lookup"><span data-stu-id="7adde-201">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="7adde-202">Authorization</span><span class="sxs-lookup"><span data-stu-id="7adde-202">Authorization</span></span> | <span data-ttu-id="7adde-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7adde-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7adde-205">要求本文</span><span class="sxs-lookup"><span data-stu-id="7adde-205">Request body</span></span>
<span data-ttu-id="7adde-206">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7adde-206">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7adde-207">応答</span><span class="sxs-lookup"><span data-stu-id="7adde-207">Response</span></span>

<span data-ttu-id="7adde-p107">成功した場合、このメソッドは応答本文で `200 OK` 応答コードと [openTypeExtension](../resources/opentypeextension.md) オブジェクトを返します。GET クエリに応じて、厳密な応答の本体は異なります。</span><span class="sxs-lookup"><span data-stu-id="7adde-p107">If successful, this method returns a `200 OK` response code and [openTypeExtension](../resources/opentypeextension.md) object in the response body. Depending on the GET query, the exact response body differs.</span></span>
## <a name="example"></a><span data-ttu-id="7adde-210">例</span><span class="sxs-lookup"><span data-stu-id="7adde-210">Example</span></span>

#### <a name="request-1"></a><span data-ttu-id="7adde-211">要求 1</span><span class="sxs-lookup"><span data-stu-id="7adde-211">Request 1</span></span>

<span data-ttu-id="7adde-p108">最初の例では、拡張情報を参照する 2 通りの方法を示し、指定されたメッセージ内の拡張情報を取得します。応答は、拡張情報を参照するために使用する方法に関係なく、同じです。</span><span class="sxs-lookup"><span data-stu-id="7adde-p108">The first example shows 2 ways of referencing an extension and gets the extension in the specified message. The response is the same regardless of the way used to reference the extension.</span></span>

<span data-ttu-id="7adde-214">最初は、名前で参照します。</span><span class="sxs-lookup"><span data-stu-id="7adde-214">First, by its name:</span></span> 

<!-- {
  "blockType": "request",
  "sampleKeys": ["Com.Contoso.Referral", "AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl==="],
  "name": "get_opentypeextension_1"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Com.Contoso.Referral
```

<span data-ttu-id="7adde-215">次に、ID (完全修飾名) で参照します。</span><span class="sxs-lookup"><span data-stu-id="7adde-215">Second, by its ID (fully qualified name):</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral
```

#### <a name="response-1"></a><span data-ttu-id="7adde-216">応答 1</span><span class="sxs-lookup"><span data-stu-id="7adde-216">Response 1</span></span>
<span data-ttu-id="7adde-217">最初の例の応答を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7adde-217">Here is the response for the first example.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.openTypeExtension"
} -->
```http
HTTP/1.1 200 OK
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
    "expirationDate": "2015-12-03T10:00:00Z"
}
```

****


#### <a name="request-2"></a><span data-ttu-id="7adde-218">要求 2</span><span class="sxs-lookup"><span data-stu-id="7adde-218">Request 2</span></span>

<span data-ttu-id="7adde-219">2 番目の例では、名前で拡張情報を参照し、指定されたグループ イベント内の拡張情報を取得します。</span><span class="sxs-lookup"><span data-stu-id="7adde-219">The second example references an extension by its name and gets the extension in the specified group event.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["Com.Contoso.Deal", "f5480dfd-7d77-4d0b-ba2e-3391953cc74a", "AAMkADVl17IsAAA="],
  "name": "get_opentypeextension_2"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/f5480dfd-7d77-4d0b-ba2e-3391953cc74a/events/AAMkADVl17IsAAA=/extensions/Com.Contoso.Deal/
```

#### <a name="response-2"></a><span data-ttu-id="7adde-220">応答 2</span><span class="sxs-lookup"><span data-stu-id="7adde-220">Response 2</span></span>

<span data-ttu-id="7adde-221">2 番目の例の応答を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7adde-221">Here is the response from the second example.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.openTypeExtension"
} -->
```http
HTTP/1.1 200 OK
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

#### <a name="request-3"></a><span data-ttu-id="7adde-222">要求 3</span><span class="sxs-lookup"><span data-stu-id="7adde-222">Request 3</span></span>

<span data-ttu-id="7adde-p109">3 番目の例では、指定されたメッセージを取得し、フィルターから返された拡張情報を組み込んで展開します。このフィルターは、**id** が完全修飾名と一致する拡張情報を返します。</span><span class="sxs-lookup"><span data-stu-id="7adde-p109">The third example gets and expands the specified message by including the extension returned from a filter. The filter returns the extension that has its **id** matching a fully qualified name.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl==="],
  "name": "get_opentypeextension_3"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===?$expand=extensions($filter=id%20eq%20'Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')
```


#### <a name="response-3"></a><span data-ttu-id="7adde-225">応答 3</span><span class="sxs-lookup"><span data-stu-id="7adde-225">Response 3</span></span>

<span data-ttu-id="7adde-p110">3 番目の例の応答を次に示します。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="7adde-p110">And here is the response from the third example. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')",
    "@odata.etag": "W/\"CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AABNsWMM\"",
    "id": "AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===",
    "changeKey": "CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AABNsWMM",
    "categories": [
    ],
    "createDateTime": "2015-06-19T02:03:31Z",
    "lastModifiedDateTime": "2015-08-13T02:28:00Z",
    "subject": "Attached is the requested info",
    "bodyPreview": "See the images attached.",
    "body": {
        "contentType": "HTML",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<style type=\"text/css\" style=\"display:none;\"><!-- P {margin-top:0;margin-bottom:0;} --></style>\r\n</head>\r\n<body dir=\"ltr\">\r\n<div id=\"divtagdefaultwrapper\" style=\"font-size:12pt;color:#000000;background-color:#FFFFFF;font-family:Calibri,Arial,Helvetica,sans-serif;\">\r\n<p>See the images attached. <br>\r\n</p>\r\n</div>\r\n</body>\r\n</html>\r\n"
    },
    "importance": "Normal",
    "hasAttachments": true,
    "parentFolderId": "AQMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===QAAAA==",
    "from": {
        "emailAddress": {
            "address": "desmond@contoso.com",
            "name": "Desmond Raley"
        }
    },
    "sender": {
        "emailAddress": {
            "address": "desmond@contoso.com",
            "name": "Desmond Raley"
        }
    },
    "toRecipients": [
        {
            "emailAddress": {
                "address": "wendy@contoso.com",
                "name": "Wendy Molina"
            }
        }
    ],
    "ccRecipients": [
    ],
    "bccRecipients": [
    ],
    "replyTo": [
    ],
    "conversationId": "AAQkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===mivdTmQ=",
    "receivedDateTime": "2015-06-19T02:05:04Z",
    "sentDateTime": "2015-06-19T02:04:59Z",
    "isDeliveryReceiptRequested": false,
    "isReadReceiptRequested": false,
    "isDraft": false,
    "isRead": true,
    "webLink": "https://outlook.office.com/owa/?ItemID=AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===%2FNJTqt5NqHlVnKVBwCY4MQpaFz9SbqUDe4%2Bbs88AAAAAAEJAACY4MQpaFz9SbqUDe4%2Bbs88AAApA4JMAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification": "Focused",
    "extensions@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('desmond40contoso.com')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions", 
    "extensions": [ 
      { 
        "@odata.type": "#microsoft.graph.openTypeExtension",
        "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
        "extensionName": "Com.Contoso.Referral",
        "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
        "companyName": "Wingtip Toys",
        "dealValue": 500050,
        "expirationDate": "2015-12-03T10:00:00Z"
      }
     ]
}
```

****

#### <a name="request-4"></a><span data-ttu-id="7adde-229">要求 4</span><span class="sxs-lookup"><span data-stu-id="7adde-229">Request 4</span></span>

<span data-ttu-id="7adde-230">4 番目の例では、完全修飾名で拡張情報を参照し、指定されたグループ投稿内の拡張情報を取得します。</span><span class="sxs-lookup"><span data-stu-id="7adde-230">The fourth example references an extension by its fully qualified name and gets the extension in the specified group post.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_opentypeextension_4"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/37df2ff0-0de0-4c33-8aee-75289364aef6/threads/AAQkADJizZJpEWwqDHsEpV_KA==/posts/AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA=/extensions/Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate
```

#### <a name="response-4"></a><span data-ttu-id="7adde-231">応答 4</span><span class="sxs-lookup"><span data-stu-id="7adde-231">Response 4</span></span>

<span data-ttu-id="7adde-232">4 番目の例の応答を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7adde-232">Here is the response from the fourth example.</span></span> 

<!-- {
  "blockType": "ignored",
  "truncated": false,
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
    "expirationDate": "2015-07-03T13:04:00Z",
    "Strings@odata.type": "#Collection(String)",
    "topPicks": [
        "Employees only",
        "Add spouse or guest",
        "Add family"
    ]
}
```


#### <a name="request-5"></a><span data-ttu-id="7adde-233">要求 5</span><span class="sxs-lookup"><span data-stu-id="7adde-233">Request 5</span></span>

<span data-ttu-id="7adde-p111">5 番目の例では、サインインしているユーザーのメールボックス内のすべてのメッセージを参照して、フィルターと一致する拡張情報が含まれているメッセージを検出し、拡張情報を組み込んでそれらのメッセージを展開します。このフィルターは、拡張情報名 `Com.Contoso.Referral` と一致する **id** プロパティを持つ拡張情報を返します。</span><span class="sxs-lookup"><span data-stu-id="7adde-p111">The fifth example looks at all messages in the signed-in user's mailbox to find those that contain an extension matching a filter, and expands them by including the extension. The filter returns extensions that has the **id** property matching the extension name `Com.Contoso.Referral`.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_opentypeextension_5"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=Extensions/any(f:f/id%20eq%20'Com.Contoso.Referral')&$expand=Extensions($filter=id%20eq%20'Com.Contoso.Referral')
```


####<a name="response-5"></a><span data-ttu-id="7adde-236">応答 5</span><span class="sxs-lookup"><span data-stu-id="7adde-236">Response 5</span></span>

<span data-ttu-id="7adde-237">5 番目の例のこの応答では、**id** が `Com.Contoso.Referral` である拡張情報が含まれているメッセージがユーザーのメールボックスに 1 つだけ存在します。</span><span class="sxs-lookup"><span data-stu-id="7adde-237">In this response for the fifth example, there is only one message in the user's mailbox that has an extension with its **id** equal to `Com.Contoso.Referral`.</span></span>

<span data-ttu-id="7adde-p112">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="7adde-p112">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages",
  "value": [
  {

    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')",
    "@odata.etag": "W/\"CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AABNsWMM\"",
    "id": "AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===",
    "changeKey": "CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AABNsWMM",
    "categories": [
    ],
    "createDateTime": "2015-06-19T02:03:31Z",
    "lastModifiedDateTime": "2015-08-13T02:28:00Z",
    "subject": "Attached is the requested info",
    "bodyPreview": "See the images attached.",
    "body": {
        "contentType": "HTML",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<style type=\"text/css\" style=\"display:none;\"><!-- P {margin-top:0;margin-bottom:0;} --></style>\r\n</head>\r\n<body dir=\"ltr\">\r\n<div id=\"divtagdefaultwrapper\" style=\"font-size:12pt;color:#000000;background-color:#FFFFFF;font-family:Calibri,Arial,Helvetica,sans-serif;\">\r\n<p>See the images attached. <br>\r\n</p>\r\n</div>\r\n</body>\r\n</html>\r\n"
    },
    "importance": "Normal",
    "hasAttachments": true,
    "parentFolderId": "AQMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===QAAAA==",
    "from": {
        "emailAddress": {
            "address": "desmond@contoso.com",
            "name": "Desmond Raley"
        }
    },
    "sender": {
        "emailAddress": {
            "address": "desmond@contoso.com",
            "name": "Desmond Raley"
        }
    },
    "toRecipients": [
        {
            "emailAddress": {
                "address": "wendy@contoso.com",
                "name": "Wendy Molina"
            }
        }
    ],
    "ccRecipients": [
    ],
    "bccRecipients": [
    ],
    "replyTo": [
    ],
    "conversationId": "AAQkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===mivdTmQ=",
    "receivedDateTime": "2015-06-19T02:05:04Z",
    "sentDateTime": "2015-06-19T02:04:59Z",
    "isDeliveryReceiptRequested": false,
    "isReadReceiptRequested": false,
    "isDraft": false,
    "isRead": true,
    "webLink": "https://outlook.office.com/owa/?ItemID=AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===%2FNJTqt5NqHlVnKVBwCY4MQpaFz9SbqUDe4%2Bbs88AAAAAAEJAACY4MQpaFz9SbqUDe4%2Bbs88AAApA4JMAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification": "Focused",
    "extensions@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('desmond40contoso.com')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions", 
    "extensions": [ 
      { 
        "@odata.type": "#microsoft.graph.openTypeExtension",
        "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
        "extensionName": "Com.Contoso.Referral",
        "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
        "companyName": "Wingtip Toys",
        "dealValue": 500050,
        "expirationDate": "2015-12-03T10:00:00Z"
      }
     ]
  }
  ]
}

```



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get openTypeExtension",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
      "Warning: /api-reference/v1.0/api/opentypeextension_get.md:
        Unable to map some markdown elements into schema.
            Unmapped methods:
        get_opentypeextension_1, get_opentypeextension_2, get_opentypeextension_3, get_opentypeextension_5
            Unmapped tables:
        Get open extension - Unknown, Permissions - AuthScopes, Path parameters - PathParameters, Optional query parameters - PathParameters, Request headers - HttpHeaders"
  ],
  "tocPath": ""
}-->
