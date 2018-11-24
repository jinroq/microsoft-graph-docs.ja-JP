# <a name="create-multi-value-extended-property"></a><span data-ttu-id="fdfd7-101">複数値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="fdfd7-101">Create multi-value extended property</span></span>

<span data-ttu-id="fdfd7-102">リソースの新規または既存のインスタンスに、1 つ以上の複数値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="fdfd7-102">Create one or more multi-value extended properties in a new or existing instance of a resource.</span></span> 

<span data-ttu-id="fdfd7-103">次のユーザー リソースがサポートされます。</span><span class="sxs-lookup"><span data-stu-id="fdfd7-103">The following user resources are supported:</span></span>

- [<span data-ttu-id="fdfd7-104">calendar</span><span class="sxs-lookup"><span data-stu-id="fdfd7-104">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="fdfd7-105">contact</span><span class="sxs-lookup"><span data-stu-id="fdfd7-105">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="fdfd7-106">contactFolder</span><span class="sxs-lookup"><span data-stu-id="fdfd7-106">contactFolder</span></span>](../resources/contactfolder.md) 
- [<span data-ttu-id="fdfd7-107">イベント</span><span class="sxs-lookup"><span data-stu-id="fdfd7-107">event</span></span>](../resources/event.md)
- [<span data-ttu-id="fdfd7-108">mailFolder</span><span class="sxs-lookup"><span data-stu-id="fdfd7-108">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="fdfd7-109">message</span><span class="sxs-lookup"><span data-stu-id="fdfd7-109">message</span></span>](../resources/message.md)

<span data-ttu-id="fdfd7-110">次のグループ リソースもサポートされます。</span><span class="sxs-lookup"><span data-stu-id="fdfd7-110">As well as the following group resources:</span></span>

- <span data-ttu-id="fdfd7-111">グループ [calendar](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="fdfd7-111">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="fdfd7-112">グループ [event](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="fdfd7-112">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="fdfd7-113">グループ [post](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="fdfd7-113">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="fdfd7-114">オープン拡張機能または拡張プロパティを使用するのに適した状況と、拡張プロパティを指定する方法の詳細については、「[拡張プロパティの概要](../resources/extended-properties-overview.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fdfd7-114">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="fdfd7-115">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="fdfd7-115">Permissions</span></span>
<span data-ttu-id="fdfd7-116">リソースに応じて、[拡張プロパティを作成するアクセス許可が委任された (アプリケーション) を要求を入力、次の表で指定されたアクセス許可は、この API を呼び出すために必要最低限。</span><span class="sxs-lookup"><span data-stu-id="fdfd7-116">Depending on the resource you're creating the extended property in and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="fdfd7-117">アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fdfd7-117">To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="fdfd7-118">サポートされているリソース</span><span class="sxs-lookup"><span data-stu-id="fdfd7-118">Supported resource</span></span> | <span data-ttu-id="fdfd7-119">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fdfd7-119">Delegated (work or school account)</span></span> | <span data-ttu-id="fdfd7-120">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fdfd7-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fdfd7-121">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fdfd7-121">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="fdfd7-122">calendar</span><span class="sxs-lookup"><span data-stu-id="fdfd7-122">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="fdfd7-123">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fdfd7-123">Calendars.ReadWrite</span></span> | <span data-ttu-id="fdfd7-124">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fdfd7-124">Calendars.ReadWrite</span></span> | <span data-ttu-id="fdfd7-125">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fdfd7-125">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="fdfd7-126">連絡先</span><span class="sxs-lookup"><span data-stu-id="fdfd7-126">contact</span></span>](../resources/contact.md) | <span data-ttu-id="fdfd7-127">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fdfd7-127">Contacts.ReadWrite</span></span> | <span data-ttu-id="fdfd7-128">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fdfd7-128">Contacts.ReadWrite</span></span> | <span data-ttu-id="fdfd7-129">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fdfd7-129">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="fdfd7-130">contactFolder</span><span class="sxs-lookup"><span data-stu-id="fdfd7-130">contactFolder</span></span>](../resources/contactfolder.md) | <span data-ttu-id="fdfd7-131">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fdfd7-131">Contacts.ReadWrite</span></span> | <span data-ttu-id="fdfd7-132">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fdfd7-132">Contacts.ReadWrite</span></span> | <span data-ttu-id="fdfd7-133">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fdfd7-133">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="fdfd7-134">イベント</span><span class="sxs-lookup"><span data-stu-id="fdfd7-134">event</span></span>](../resources/event.md) | <span data-ttu-id="fdfd7-135">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fdfd7-135">Calendars.ReadWrite</span></span> | <span data-ttu-id="fdfd7-136">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fdfd7-136">Calendars.ReadWrite</span></span> |  <span data-ttu-id="fdfd7-137">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fdfd7-137">Calendars.ReadWrite</span></span>|
| <span data-ttu-id="fdfd7-138">グループ [calendar](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="fdfd7-138">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="fdfd7-139">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdfd7-139">Group.ReadWrite.All</span></span> | <span data-ttu-id="fdfd7-140">使用不可</span><span class="sxs-lookup"><span data-stu-id="fdfd7-140">Not supported</span></span> | <span data-ttu-id="fdfd7-141">使用不可</span><span class="sxs-lookup"><span data-stu-id="fdfd7-141">Not supported</span></span> |
| <span data-ttu-id="fdfd7-142">グループ [event](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="fdfd7-142">group [event](../resources/event.md)</span></span> | <span data-ttu-id="fdfd7-143">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdfd7-143">Group.ReadWrite.All</span></span> | <span data-ttu-id="fdfd7-144">使用不可</span><span class="sxs-lookup"><span data-stu-id="fdfd7-144">Not supported</span></span> | <span data-ttu-id="fdfd7-145">使用不可</span><span class="sxs-lookup"><span data-stu-id="fdfd7-145">Not supported</span></span> |
| <span data-ttu-id="fdfd7-146">グループ [post](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="fdfd7-146">group [post](../resources/post.md)</span></span> | <span data-ttu-id="fdfd7-147">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdfd7-147">Group.ReadWrite.All</span></span> | <span data-ttu-id="fdfd7-148">使用不可</span><span class="sxs-lookup"><span data-stu-id="fdfd7-148">Not supported</span></span> | <span data-ttu-id="fdfd7-149">使用不可</span><span class="sxs-lookup"><span data-stu-id="fdfd7-149">Not supported</span></span> |
| [<span data-ttu-id="fdfd7-150">mailFolder</span><span class="sxs-lookup"><span data-stu-id="fdfd7-150">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="fdfd7-151">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fdfd7-151">Mail.ReadWrite</span></span> | <span data-ttu-id="fdfd7-152">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fdfd7-152">Mail.ReadWrite</span></span> | <span data-ttu-id="fdfd7-153">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fdfd7-153">Mail.ReadWrite</span></span> |
| [<span data-ttu-id="fdfd7-154">メッセージ</span><span class="sxs-lookup"><span data-stu-id="fdfd7-154">message</span></span>](../resources/message.md) | <span data-ttu-id="fdfd7-155">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fdfd7-155">Mail.ReadWrite</span></span> | <span data-ttu-id="fdfd7-156">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fdfd7-156">Mail.ReadWrite</span></span> | <span data-ttu-id="fdfd7-157">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fdfd7-157">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="fdfd7-158">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fdfd7-158">HTTP request</span></span>
<span data-ttu-id="fdfd7-159">新規または既存のリソースのインスタンスに、拡張プロパティを作成できます。</span><span class="sxs-lookup"><span data-stu-id="fdfd7-159">You can create extended properties in a new or existing resource instance.</span></span>

<span data-ttu-id="fdfd7-p102">1 つ以上の拡張プロパティを_新しい_リソースのインスタンスに作成するには、インスタンスの作成と同じ REST 要求を使用し、新しいリソース インスタンスのプロパティ_と拡張プロパティを_要求の本文に含めます。一部のリソースでは複数の作成方法がサポートされていますので、注意してください。これらのリソース インスタンスの作成に関して詳しくは、[メッセージ](../resources/message.md)、[mailFolder](../api/user_post_mailfolders.md)、[イベント](../api/user_post_events.md)、[予定表](../api/user_post_calendars.md)、[連絡先](../api/user_post_contacts.md)、[contactFolder](../api/user_post_contactfolders.md)、[グループ イベント](../api/group_post_events.md)、および [グループ投稿](../resources/post.md)作成の該当する各トピックをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="fdfd7-p102">To create one or more extended properties in a _new_ resource instance, use the same REST request as creating the instance, and include the properties of the new resource instance _and extended property_ in the request body. Note that some resources support creation in more than one way. For more information on creating these resource instances, see the corresponding topics for creating a [message](../resources/message.md), [mailFolder](../api/user_post_mailfolders.md), [event](../api/user_post_events.md), [calendar](../api/user_post_calendars.md), [contact](../api/user_post_contacts.md), [contactFolder](../api/user_post_contactfolders.md), [group event](../api/group_post_events.md), and [group post](../resources/post.md).</span></span> 
 
<span data-ttu-id="fdfd7-163">以下に要求の構文を示します。</span><span class="sxs-lookup"><span data-stu-id="fdfd7-163">The following is the syntax of the requests.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST /me/messages
POST /users/{id|userPrincipalName}/messages
POST /me/mailFolders/{id}/messages

POST /me/mailFolders
POST /users/{id|userPrincipalName}/mailFolders

POST /me/events
POST /users/{id|userPrincipalName}/events

POST /me/calendars
POST /users/{id|userPrincipalName}/calendars

POST /me/contacts
POST /users/{id|userPrincipalName}/contacts

POST /me/contactFolders
POST /users/{id|userPrincipalName}/contactFolders

POST /groups/{id}/events

POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/reply
POST /groups/{id}/threads/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/reply
POST /groups/{id}/threads
POST /groups/{id}/conversations
```

<span data-ttu-id="fdfd7-164">既存のリソースのインスタンスで 1 つ以上の拡張プロパティを作成するには、要求でインスタンスを指定し、要求本文に拡張プロパティを含めます。</span><span class="sxs-lookup"><span data-stu-id="fdfd7-164">To create one or more extended properties in an existing resource instance, specify the instance in the request, and include the extended property in the request body.</span></span>

<span data-ttu-id="fdfd7-165">**注** 既存のグループ投稿には拡張プロパティを作成できません。</span><span class="sxs-lookup"><span data-stu-id="fdfd7-165">**Note** You cannot create an extended property in an existing group post.</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id|userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}

PATCH /me/mailFolders/{id}
PATCH /users/{id|userPrincipalName}/mailFolders/{id}

PATCH /me/events/{id}
PATCH /users/{id|userPrincipalName}/events/{id}

PATCH /me/calendars/{id}
PATCH /users/{id|userPrincipalName}/calendars/{id}

PATCH /me/contacts/{id}
PATCH /users/{id|userPrincipalName}/contacts/{id}

PATCH /me/contactFolders/{id}
PATCH /users/{id|userPrincipalName}/contactFolders/{id}

PATCH /groups/{id}/events/{id}
```

## <a name="request-headers"></a><span data-ttu-id="fdfd7-166">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fdfd7-166">Request headers</span></span>
| <span data-ttu-id="fdfd7-167">名前</span><span class="sxs-lookup"><span data-stu-id="fdfd7-167">Name</span></span>       | <span data-ttu-id="fdfd7-168">値</span><span class="sxs-lookup"><span data-stu-id="fdfd7-168">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="fdfd7-169">Authorization</span><span class="sxs-lookup"><span data-stu-id="fdfd7-169">Authorization</span></span> | <span data-ttu-id="fdfd7-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="fdfd7-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fdfd7-172">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fdfd7-172">Content-Type</span></span> | <span data-ttu-id="fdfd7-173">application/json</span><span class="sxs-lookup"><span data-stu-id="fdfd7-173">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="fdfd7-174">要求本文</span><span class="sxs-lookup"><span data-stu-id="fdfd7-174">Request body</span></span>

<span data-ttu-id="fdfd7-175">リソース インスタンスの **multiValueExtendedProperties** コレクション プロパティに、各 [multiValueLegacyExtendedProperty](../resources/multiValueLegacyExtendedProperty.md) オブジェクトの JSON 本文を指定します。</span><span class="sxs-lookup"><span data-stu-id="fdfd7-175">Provide a JSON body of each [multiValueLegacyExtendedProperty](../resources/multiValueLegacyExtendedProperty.md) object in the **multiValueExtendedProperties** collection property of the resource instance.</span></span>

|<span data-ttu-id="fdfd7-176">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fdfd7-176">Property</span></span>|<span data-ttu-id="fdfd7-177">型</span><span class="sxs-lookup"><span data-stu-id="fdfd7-177">Type</span></span>|<span data-ttu-id="fdfd7-178">説明</span><span class="sxs-lookup"><span data-stu-id="fdfd7-178">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="fdfd7-179">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="fdfd7-179">multiValueExtendedProperties</span></span>|<span data-ttu-id="fdfd7-180">[multiValueLegacyExtendedProperty](../resources/multiValueLegacyExtendedProperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="fdfd7-180">[multiValueLegacyExtendedProperty](../resources/multiValueLegacyExtendedProperty.md) collection</span></span>| <span data-ttu-id="fdfd7-181">1 つ以上の複数値を持つ拡張プロパティの配列。</span><span class="sxs-lookup"><span data-stu-id="fdfd7-181">An array of one or more multi-valued extended properties.</span></span> |
|<span data-ttu-id="fdfd7-182">id</span><span class="sxs-lookup"><span data-stu-id="fdfd7-182">id</span></span>|<span data-ttu-id="fdfd7-183">String</span><span class="sxs-lookup"><span data-stu-id="fdfd7-183">String</span></span>|<span data-ttu-id="fdfd7-p104">**multiValueExtendedProperties** コレクションの各プロパティに対してこれを指定し、プロパティを特定します。サポートされている形式のいずれかに従う必要があります。詳しくは、[「Outlook の拡張プロパティの概要」](../resources/extended-properties-overview.md)をご覧ください。必須。</span><span class="sxs-lookup"><span data-stu-id="fdfd7-p104">For each property in the **multiValueExtendedProperties** collection, specify this to identify the property. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|
|<span data-ttu-id="fdfd7-188">value</span><span class="sxs-lookup"><span data-stu-id="fdfd7-188">value</span></span>|<span data-ttu-id="fdfd7-189">文字列</span><span class="sxs-lookup"><span data-stu-id="fdfd7-189">string</span></span>|<span data-ttu-id="fdfd7-p105">**multiValueExtendedProperties** コレクションの各プロパティに対し、プロパティの値を特定します。必須。</span><span class="sxs-lookup"><span data-stu-id="fdfd7-p105">For each property in the **multiValueExtendedProperties** collection, specify the property value. Required.</span></span>|

<span data-ttu-id="fdfd7-192">だけでなく、新しい**multiValueExtendedProperties**コレクションの_新しい_リソースのインスタンスで拡張プロパティを作成するときにそのリソースのインスタンスにも (つまり、[メッセージ](../resources/message.md)、 [mailFolder の JSON 表現を提供します。](../resources/mailfolder.md)、[イベント](../resources/event.md)などです。)。</span><span class="sxs-lookup"><span data-stu-id="fdfd7-192">When creating an extended property in a _new_ resource instance, in addition to the new **multiValueExtendedProperties** collection, provide a JSON representation of that resource instance as well (that is, a [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), etc.).</span></span>


## <a name="response"></a><span data-ttu-id="fdfd7-193">応答</span><span class="sxs-lookup"><span data-stu-id="fdfd7-193">Response</span></span>

#### <a name="response-code"></a><span data-ttu-id="fdfd7-194">応答コード</span><span class="sxs-lookup"><span data-stu-id="fdfd7-194">Response code</span></span>
<span data-ttu-id="fdfd7-195">新しいリソース インスタンスに拡張プロパティが正常に作成されると、`201 Created` が返されます。ただし新しいグループ投稿の場合は別で、使用するメソッドに応じて、`200 OK` または `202 Accepted` が返されます。</span><span class="sxs-lookup"><span data-stu-id="fdfd7-195">An operation successful in creating an extended property in a new resource instance returns `201 Created`, except in a new group post, depending on the method used, the operation can return `200 OK` or `202 Accepted`.</span></span>

<span data-ttu-id="fdfd7-196">既存のリソース インスタンスに拡張プロパティが正常に作成されると、`200 OK` が返されます。</span><span class="sxs-lookup"><span data-stu-id="fdfd7-196">In an existing resource instance, a successful create operation returns `200 OK`.</span></span> 


#### <a name="response-body"></a><span data-ttu-id="fdfd7-197">応答本文</span><span class="sxs-lookup"><span data-stu-id="fdfd7-197">Response body</span></span>

<span data-ttu-id="fdfd7-p106">[グループ投稿](../resources/post.md)以外のサポートされているリソースで拡張プロパティを作成する場合、応答には新規または既存のインスタンスだけが含まれ、新しい拡張プロパティは含まれません。新しく作成された拡張プロパティを表示するには、[拡張プロパティを使用して展開されているインスタンスを取得](../api/multivaluelegacyextendedproperty_get.md)します。</span><span class="sxs-lookup"><span data-stu-id="fdfd7-p106">When creating an extended property in a supported resource other than [group post](../resources/post.md), the response includes only the new or existing instance but not the new extended property. To see the newly created extended property, [get the instance expanded with the extended property](../api/multivaluelegacyextendedproperty_get.md).</span></span>

<span data-ttu-id="fdfd7-p107">_新しい_グループ投稿に拡張プロパティを作成する場合、応答には応答コードだけが含まれ、新しい投稿や拡張プロパティは含まれません。既存のグループ投稿には拡張プロパティを作成できません。</span><span class="sxs-lookup"><span data-stu-id="fdfd7-p107">When creating an extended property in a _new_ group post, the response includes only a response code but not the new post nor the extended property. You cannot create an extended property in an existing group post.</span></span>


## <a name="example"></a><span data-ttu-id="fdfd7-202">例</span><span class="sxs-lookup"><span data-stu-id="fdfd7-202">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="fdfd7-203">要求 1</span><span class="sxs-lookup"><span data-stu-id="fdfd7-203">Request 1</span></span>

<span data-ttu-id="fdfd7-p108">最初の例では、すべて同じ POST 操作の新しいイベントで複数値の拡張プロパティを作成します。新しいイベントに通常含まれるプロパティとは別に、要求の本文に 1 つの拡張プロパティを含む **multiValueExtendedProperties** コレクションが含まれます。要求本文には、その複数値の拡張プロパティに関する次のものが含まれています。</span><span class="sxs-lookup"><span data-stu-id="fdfd7-p108">The first example creates a multi-value extended property in a new event all in the same POST operation. Apart from the properties you'd normally include for a new event, the request body includes the **multiValueExtendedProperties** collection which contains one extended property. The request body includes the following for that multi-value extended property:</span></span>

- <span data-ttu-id="fdfd7-207">**id** 指定された GUID と名前 `Recreation` の文字列の配列としてプロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="fdfd7-207">**id** which specifies the property as an array of strings with the specified GUID and the name `Recreation`.</span></span> 
- <span data-ttu-id="fdfd7-208">**value** は、3 つの文字列値 `["Food", "Hiking", "Swimming"]` の配列として `Recreation` を指定します。</span><span class="sxs-lookup"><span data-stu-id="fdfd7-208">**value** which specifies `Recreation` as an array of 3 string values, `["Food", "Hiking", "Swimming"]`.</span></span>
 

<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/me/events
Content-Type: application/json

{
  "subject": "Family reunion",
  "body": {
    "contentType": "HTML",
    "content": "Let's get together this Thanksgiving!"
  },
  "start": {
      "dateTime": "2015-11-26T09:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2015-11-29T21:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "attendees": [
    {
      "emailAddress": {
        "address": "Terrie@contoso.com",
        "name": "Terrie Barrera"
      },
      "type": "Required"
    },
    {
      "emailAddress": {
        "address": "Lauren@contoso.com",
        "name": "Lauren Solis"
      },
      "type": "Required"
    }
  ],
  "multiValueExtendedProperties": [
     {
           "id":"StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation",
           "value": ["Food", "Hiking", "Swimming"]
     }
  ]
}
```

##### <a name="response-1"></a><span data-ttu-id="fdfd7-209">応答 1</span><span class="sxs-lookup"><span data-stu-id="fdfd7-209">Response 1</span></span>

<span data-ttu-id="fdfd7-p109">[イベントのみの作成](../api/user_post_events.md)からの応答と同様に、`HTTP 201 Created` 応答コードによって正常な応答が示され、応答の本文に新しいイベントが含まれます。応答には、新しく作成された拡張プロパティは含まれません。</span><span class="sxs-lookup"><span data-stu-id="fdfd7-p109">A successful response is indicated by an `HTTP 201 Created` response code, and includes the new event in the response body, similar to the response from [creating just an event](../api/user_post_events.md). The response does not include any newly created extended properties.</span></span>

<span data-ttu-id="fdfd7-212">新しく作成された拡張プロパティを表示するには、[拡張プロパティを使用して展開されているイベントを取得](../api/multivaluelegacyextendedproperty_get.md)します。</span><span class="sxs-lookup"><span data-stu-id="fdfd7-212">To see the newly created extended property, [get the event expanded with the extended property](../api/multivaluelegacyextendedproperty_get.md).</span></span>


****

##### <a name="request-2"></a><span data-ttu-id="fdfd7-213">要求 2</span><span class="sxs-lookup"><span data-stu-id="fdfd7-213">Request 2</span></span>

<span data-ttu-id="fdfd7-p110">2 番目の例では、指定したメッセージに対して 1 つの複数値の拡張プロパティを作成します。拡張プロパティは、**multiValueExtendedProperties** コレクションの唯一の要素です。要求本文には、拡張プロパティに関する次のものが含まれています。</span><span class="sxs-lookup"><span data-stu-id="fdfd7-p110">The second example creates one multi-value extended property for the specified message. That extended property is the only element in the **multiValueExtendedProperties** collection. The request body includes the following for the extended property:</span></span>

- <span data-ttu-id="fdfd7-217">**id** 指定された GUID と名前 `Palette` を使って、文字列の配列としてプロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="fdfd7-217">**id** specifies the property as an array of strings with the specified GUID and the name `Palette`.</span></span>
- <span data-ttu-id="fdfd7-218">**value** 3 つの文字列値 `["Green", "Aqua", "Blue"]` の配列として `Palette` を指定します。</span><span class="sxs-lookup"><span data-stu-id="fdfd7-218">**value** specifies `Palette` as an array of 3 string values, `["Green", "Aqua", "Blue"]`.</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/v1.0/me/messages('AAMkAGE1M2_as77AACHsLrBBBA=')

Content-Type: application/json

{
  "multiValueExtendedProperties": [
      {
         "id":"StringArray {66f5a359-4659-4830-9070-00049ec6ac6e} Name Palette",
         "value":["Green", "Aqua", "Blue"]
      }
    ]
}
```

##### <a name="response-2"></a><span data-ttu-id="fdfd7-219">応答 2</span><span class="sxs-lookup"><span data-stu-id="fdfd7-219">Response 2</span></span>

<span data-ttu-id="fdfd7-p111">[メッセージの更新](../api/message_update.md)からの応答と同様に、`HTTP 200 OK` 応答コードによって正常な応答が示され、応答の本文に指定したメッセージが含まれています。応答には、新しく作成された拡張プロパティは含まれません。</span><span class="sxs-lookup"><span data-stu-id="fdfd7-p111">A successful response is indicated by an `HTTP 200 OK` response code, and includes the specified message in the response body, similar to the response from [updating a message](../api/message_update.md). The response does not include the newly created extended property.</span></span>

<span data-ttu-id="fdfd7-222">新しく作成された拡張プロパティを表示するには、[拡張プロパティを使用して展開されているメッセージを取得](../api/multivaluelegacyextendedproperty_get.md)します。</span><span class="sxs-lookup"><span data-stu-id="fdfd7-222">To see the newly created extended property, [get the message expanded with the extended property](../api/multivaluelegacyextendedproperty_get.md).</span></span>


<!-- This page was manually created. -->
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create a single-value extended property",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->




