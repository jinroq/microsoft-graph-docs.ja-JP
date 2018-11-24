# <a name="create-single-value-extended-property"></a><span data-ttu-id="3f677-101">単一値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="3f677-101">Create single-value extended property</span></span>

<span data-ttu-id="3f677-102">リソースの新規または既存のインスタンスに、1 つ以上の単一値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="3f677-102">Create one or more single-value extended properties in a new or existing instance of a resource.</span></span> 

<span data-ttu-id="3f677-103">次のユーザー リソースがサポートされます。</span><span class="sxs-lookup"><span data-stu-id="3f677-103">The following user resources are supported:</span></span>

- [<span data-ttu-id="3f677-104">calendar</span><span class="sxs-lookup"><span data-stu-id="3f677-104">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="3f677-105">contact</span><span class="sxs-lookup"><span data-stu-id="3f677-105">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="3f677-106">contactFolder</span><span class="sxs-lookup"><span data-stu-id="3f677-106">contactFolder</span></span>](../resources/contactfolder.md) 
- [<span data-ttu-id="3f677-107">イベント</span><span class="sxs-lookup"><span data-stu-id="3f677-107">event</span></span>](../resources/event.md)
- [<span data-ttu-id="3f677-108">mailFolder</span><span class="sxs-lookup"><span data-stu-id="3f677-108">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="3f677-109">message</span><span class="sxs-lookup"><span data-stu-id="3f677-109">message</span></span>](../resources/message.md)

<span data-ttu-id="3f677-110">次のグループ リソースもサポートされます。</span><span class="sxs-lookup"><span data-stu-id="3f677-110">As well as the following group resources:</span></span>

- <span data-ttu-id="3f677-111">グループ [calendar](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="3f677-111">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="3f677-112">グループ [event](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="3f677-112">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="3f677-113">グループ [post](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="3f677-113">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="3f677-114">オープン拡張機能または拡張プロパティを使用するのに適した状況と、拡張プロパティを指定する方法の詳細については、「[拡張プロパティの概要](../resources/extended-properties-overview.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3f677-114">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="3f677-115">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3f677-115">Permissions</span></span>
<span data-ttu-id="3f677-116">リソースに応じて、[拡張プロパティを作成するアクセス許可が委任された (アプリケーション) を要求を入力、次の表で指定されたアクセス許可は、この API を呼び出すために必要最低限。</span><span class="sxs-lookup"><span data-stu-id="3f677-116">Depending on the resource you're creating the extended property in and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="3f677-117">アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3f677-117">To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="3f677-118">サポートされているリソース</span><span class="sxs-lookup"><span data-stu-id="3f677-118">Supported resource</span></span> | <span data-ttu-id="3f677-119">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3f677-119">Delegated (work or school account)</span></span> | <span data-ttu-id="3f677-120">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3f677-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3f677-121">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3f677-121">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="3f677-122">calendar</span><span class="sxs-lookup"><span data-stu-id="3f677-122">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="3f677-123">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3f677-123">Calendars.ReadWrite</span></span> | <span data-ttu-id="3f677-124">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3f677-124">Calendars.ReadWrite</span></span> | <span data-ttu-id="3f677-125">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3f677-125">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="3f677-126">連絡先</span><span class="sxs-lookup"><span data-stu-id="3f677-126">contact</span></span>](../resources/contact.md) | <span data-ttu-id="3f677-127">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3f677-127">Contacts.ReadWrite</span></span> | <span data-ttu-id="3f677-128">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3f677-128">Contacts.ReadWrite</span></span> | <span data-ttu-id="3f677-129">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3f677-129">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="3f677-130">contactFolder</span><span class="sxs-lookup"><span data-stu-id="3f677-130">contactFolder</span></span>](../resources/contactfolder.md) | <span data-ttu-id="3f677-131">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3f677-131">Contacts.ReadWrite</span></span> | <span data-ttu-id="3f677-132">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3f677-132">Contacts.ReadWrite</span></span> | <span data-ttu-id="3f677-133">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3f677-133">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="3f677-134">イベント</span><span class="sxs-lookup"><span data-stu-id="3f677-134">event</span></span>](../resources/event.md) | <span data-ttu-id="3f677-135">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3f677-135">Calendars.ReadWrite</span></span> | <span data-ttu-id="3f677-136">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3f677-136">Calendars.ReadWrite</span></span> |  <span data-ttu-id="3f677-137">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3f677-137">Calendars.ReadWrite</span></span>|
| <span data-ttu-id="3f677-138">グループ [calendar](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="3f677-138">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="3f677-139">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f677-139">Group.ReadWrite.All</span></span> | <span data-ttu-id="3f677-140">使用不可</span><span class="sxs-lookup"><span data-stu-id="3f677-140">Not supported</span></span> | <span data-ttu-id="3f677-141">使用不可</span><span class="sxs-lookup"><span data-stu-id="3f677-141">Not supported</span></span> |
| <span data-ttu-id="3f677-142">グループ [event](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="3f677-142">group [event](../resources/event.md)</span></span> | <span data-ttu-id="3f677-143">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f677-143">Group.ReadWrite.All</span></span> | <span data-ttu-id="3f677-144">使用不可</span><span class="sxs-lookup"><span data-stu-id="3f677-144">Not supported</span></span> | <span data-ttu-id="3f677-145">使用不可</span><span class="sxs-lookup"><span data-stu-id="3f677-145">Not supported</span></span> |
| <span data-ttu-id="3f677-146">グループ [post](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="3f677-146">group [post](../resources/post.md)</span></span> | <span data-ttu-id="3f677-147">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f677-147">Group.ReadWrite.All</span></span> | <span data-ttu-id="3f677-148">使用不可</span><span class="sxs-lookup"><span data-stu-id="3f677-148">Not supported</span></span> | <span data-ttu-id="3f677-149">使用不可</span><span class="sxs-lookup"><span data-stu-id="3f677-149">Not supported</span></span> |
| [<span data-ttu-id="3f677-150">mailFolder</span><span class="sxs-lookup"><span data-stu-id="3f677-150">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="3f677-151">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3f677-151">Mail.ReadWrite</span></span> | <span data-ttu-id="3f677-152">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3f677-152">Mail.ReadWrite</span></span> | <span data-ttu-id="3f677-153">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3f677-153">Mail.ReadWrite</span></span> |
| [<span data-ttu-id="3f677-154">メッセージ</span><span class="sxs-lookup"><span data-stu-id="3f677-154">message</span></span>](../resources/message.md) | <span data-ttu-id="3f677-155">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3f677-155">Mail.ReadWrite</span></span> | <span data-ttu-id="3f677-156">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3f677-156">Mail.ReadWrite</span></span> | <span data-ttu-id="3f677-157">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3f677-157">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="3f677-158">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3f677-158">HTTP request</span></span>
<span data-ttu-id="3f677-159">新規または既存のリソースのインスタンスに、拡張プロパティを作成できます。</span><span class="sxs-lookup"><span data-stu-id="3f677-159">You can create extended properties in a new or existing resource instance.</span></span>

<span data-ttu-id="3f677-p102">1 つ以上の拡張プロパティを_新しい_リソースのインスタンスに作成するには、インスタンスの作成と同じ REST 要求を使用し、新しいリソース インスタンスのプロパティ_と拡張プロパティを_要求の本文に含めます。一部のリソースでは複数の作成方法がサポートされていますので、注意してください。これらのリソース インスタンスの作成に関して詳しくは、[メッセージ](../resources/message.md)、[mailFolder](../api/user_post_mailfolders.md)、[イベント](../api/user_post_events.md)、[予定表](../api/user_post_calendars.md)、[連絡先](../api/user_post_contacts.md)、[contactFolder](../api/user_post_contactfolders.md)、[グループ イベント](../api/group_post_events.md)、および [グループ投稿](../resources/post.md)作成の該当する各トピックをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="3f677-p102">To create one or more extended properties in a _new_ resource instance, use the same REST request as creating the instance, and include the properties of the new resource instance _and extended property_ in the request body. Note that some resources support creation in more than one way. For more information on creating these resource instances, see the corresponding topics for creating a [message](../resources/message.md), [mailFolder](../api/user_post_mailfolders.md), [event](../api/user_post_events.md), [calendar](../api/user_post_calendars.md), [contact](../api/user_post_contacts.md), [contactFolder](../api/user_post_contactfolders.md), [group event](../api/group_post_events.md), and [group post](../resources/post.md).</span></span> 
 
<span data-ttu-id="3f677-163">以下に要求の構文を示します。</span><span class="sxs-lookup"><span data-stu-id="3f677-163">The following is the syntax of the requests.</span></span> 

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

<span data-ttu-id="3f677-164">既存のリソースのインスタンスで 1 つ以上の拡張プロパティを作成するには、要求でインスタンスを指定し、要求本文に拡張プロパティを含めます。</span><span class="sxs-lookup"><span data-stu-id="3f677-164">To create one or more extended properties in an existing resource instance, specify the instance in the request, and include the extended property in the request body.</span></span>

<span data-ttu-id="3f677-165">**注** 既存のグループ投稿には拡張プロパティを作成できません。</span><span class="sxs-lookup"><span data-stu-id="3f677-165">**Note** You cannot create an extended property in an existing group post.</span></span>

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

## <a name="request-headers"></a><span data-ttu-id="3f677-166">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3f677-166">Request headers</span></span>
| <span data-ttu-id="3f677-167">名前</span><span class="sxs-lookup"><span data-stu-id="3f677-167">Name</span></span>       | <span data-ttu-id="3f677-168">値</span><span class="sxs-lookup"><span data-stu-id="3f677-168">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="3f677-169">Authorization</span><span class="sxs-lookup"><span data-stu-id="3f677-169">Authorization</span></span> | <span data-ttu-id="3f677-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3f677-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3f677-172">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3f677-172">Content-Type</span></span> | <span data-ttu-id="3f677-173">application/json</span><span class="sxs-lookup"><span data-stu-id="3f677-173">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="3f677-174">要求本文</span><span class="sxs-lookup"><span data-stu-id="3f677-174">Request body</span></span>

<span data-ttu-id="3f677-175">リソース インスタンスの **singleValueExtendedProperties** コレクション プロパティに、各 [singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md) オブジェクトの JSON 本文を指定します。</span><span class="sxs-lookup"><span data-stu-id="3f677-175">Provide a JSON body of each [singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md) object in the **singleValueExtendedProperties** collection property of the resource instance.</span></span>

|<span data-ttu-id="3f677-176">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3f677-176">Property</span></span>|<span data-ttu-id="3f677-177">型</span><span class="sxs-lookup"><span data-stu-id="3f677-177">Type</span></span>|<span data-ttu-id="3f677-178">説明</span><span class="sxs-lookup"><span data-stu-id="3f677-178">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="3f677-179">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="3f677-179">singleValueExtendedProperties</span></span>|<span data-ttu-id="3f677-180">[singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="3f677-180">[singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md) collection</span></span>| <span data-ttu-id="3f677-181">1 つ以上の単一値を持つ拡張プロパティの配列。</span><span class="sxs-lookup"><span data-stu-id="3f677-181">An array of one or more single-valued extended properties.</span></span> |
|<span data-ttu-id="3f677-182">id</span><span class="sxs-lookup"><span data-stu-id="3f677-182">id</span></span>|<span data-ttu-id="3f677-183">String</span><span class="sxs-lookup"><span data-stu-id="3f677-183">String</span></span>|<span data-ttu-id="3f677-p104">**singleValueExtendedProperties** コレクションの各プロパティに対して、これを指定することでプロパティを特定します。サポートされている形式のいずれかに従う必要があります。詳しくは、「[Outlook の拡張プロパティの概要](../resources/extended-properties-overview.md)」を参照してください。必須。</span><span class="sxs-lookup"><span data-stu-id="3f677-p104">For each property in the **singleValueExtendedProperties** collection, specify this to identify the property. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|
|<span data-ttu-id="3f677-188">value</span><span class="sxs-lookup"><span data-stu-id="3f677-188">value</span></span>|<span data-ttu-id="3f677-189">文字列</span><span class="sxs-lookup"><span data-stu-id="3f677-189">string</span></span>|<span data-ttu-id="3f677-p105">**singleValueExtendedProperties** コレクションの各プロパティについて、プロパティの値を特定します。必須。</span><span class="sxs-lookup"><span data-stu-id="3f677-p105">For each property in the **singleValueExtendedProperties** collection, specify the property value. Required.</span></span>|

<span data-ttu-id="3f677-192">_新しい_リソース インスタンスに拡張プロパティを作成する場合は、新しい **singleValueExtendedProperties**コレクションのほか、そのリソース インスタンスの JSON 表現を指定します ([message](../resources/message.md)、[mailFolder](../resources/mailfolder.md)、[event](../resources/event.md) など)。</span><span class="sxs-lookup"><span data-stu-id="3f677-192">When creating an extended property in a _new_ resource instance, in addition to the new **singleValueExtendedProperties** collection, provide a JSON representation of that resource instance (that is, a [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), etc.)</span></span>

## <a name="response"></a><span data-ttu-id="3f677-193">応答</span><span class="sxs-lookup"><span data-stu-id="3f677-193">Response</span></span>

#### <a name="response-code"></a><span data-ttu-id="3f677-194">応答コード</span><span class="sxs-lookup"><span data-stu-id="3f677-194">Response code</span></span>
<span data-ttu-id="3f677-195">新しいリソース インスタンスに拡張プロパティが正常に作成されると、`201 Created` が返されます。ただし新しいグループ投稿の場合は別で、使用するメソッドに応じて、`200 OK` または `202 Accepted` が返されます。</span><span class="sxs-lookup"><span data-stu-id="3f677-195">An operation successful in creating an extended property in a new resource instance returns `201 Created`, except in a new group post, depending on the method used, the operation can return `200 OK` or `202 Accepted`.</span></span>

<span data-ttu-id="3f677-196">既存のリソース インスタンスに拡張プロパティが正常に作成されると、`200 OK` が返されます。</span><span class="sxs-lookup"><span data-stu-id="3f677-196">In an existing resource instance, a successful create operation returns `200 OK`.</span></span> 


#### <a name="response-body"></a><span data-ttu-id="3f677-197">応答本文</span><span class="sxs-lookup"><span data-stu-id="3f677-197">Response body</span></span>

<span data-ttu-id="3f677-p106">拡張プロパティを作成する場合、応答には新規または既存のインスタンスのみを含めて、新しい拡張プロパティは含めません。新しく作成された拡張プロパティを表示するには、[拡張プロパティを使用して展開されているインスタンスを取得](../api/singlevaluelegacyextendedproperty_get.md)します。</span><span class="sxs-lookup"><span data-stu-id="3f677-p106">When creating an extended property, the response includes only the new or existing instance but not the new extended property. To see the newly created extended property, [get the instance expanded with the extended property](../api/singlevaluelegacyextendedproperty_get.md).</span></span>

<span data-ttu-id="3f677-200">スレッドまたは投稿に返信することで、_新しい_[グループ投稿](../resources/post.md)に拡張プロパティを作成する場合、応答には応答コードのみを含めて、新しい投稿や拡張プロパティは含めません。</span><span class="sxs-lookup"><span data-stu-id="3f677-200">When creating an extended property in a _new_ [group post](../resources/post.md) by replying to a thread or post, the response includes only a response code but not the new post nor the extended property.</span></span>



## <a name="example"></a><span data-ttu-id="3f677-201">例</span><span class="sxs-lookup"><span data-stu-id="3f677-201">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="3f677-202">要求 1</span><span class="sxs-lookup"><span data-stu-id="3f677-202">Request 1</span></span>

<span data-ttu-id="3f677-p107">最初の例では、同じ POST 操作で新しいイベントと単一値の拡張プロパティを作成します。新しいイベントに通常含めるプロパティとは別に、1 つの単一値の拡張プロパティを含む **singleValueExtendedProperties** コレクションを要求の本文に含め、そのプロパティは次のようにします。</span><span class="sxs-lookup"><span data-stu-id="3f677-p107">The first example creates a new event and a single-value extended property in the same POST operation. Apart from the properties you'd normally include for a new event, the request body includes the **singleValueExtendedProperties** collection that contains one single-value extended property, and the following for the property:</span></span>
- <span data-ttu-id="3f677-205">**id** は、プロパティの型を `String` (GUID) として指定し、`Fun` という名前のプロパティとして指定します。</span><span class="sxs-lookup"><span data-stu-id="3f677-205">**id** specifies the property type as `String`, the GUID, and the property named `Fun`.</span></span>
- <span data-ttu-id="3f677-206">**value** は、`Fun` プロパティの値として `Food` を指定します。</span><span class="sxs-lookup"><span data-stu-id="3f677-206">**value** specifies `Food` as the value of the `Fun` property.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/me/events
Content-Type: application/json

{
  "subject": "Celebrate Thanksgiving",
  "body": {
    "contentType": "HTML",
    "content": "Let's get together!"
  },
  "start": {
      "dateTime": "2015-11-26T18:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2015-11-26T23:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "attendees": [
    {
      "emailAddress": {
        "address": "Terrie@contoso.com",
        "name": "Terrie Barrera"
      },
      "type": "Required"
    }
  ],
  "singleValueExtendedProperties": [
     {
           "id":"String {66f5a359-4659-4830-9070-00040ec6ac6e} Name Fun",
           "value":"Food"
     }
  ]
}
```

##### <a name="response-1"></a><span data-ttu-id="3f677-207">応答 1</span><span class="sxs-lookup"><span data-stu-id="3f677-207">Response 1</span></span>

<span data-ttu-id="3f677-p108">[イベントのみの作成](../api/user_post_events.md)からの応答と同様に、`HTTP 201 Created` 応答コードによって正常な応答が示され、応答の本文に新しいイベントが含まれます。応答には、新しく作成された拡張プロパティは含まれません。</span><span class="sxs-lookup"><span data-stu-id="3f677-p108">A successful response is indicated by an `HTTP 201 Created` response code, and includes the new event in the response body, similar to the response from [creating just an event](../api/user_post_events.md). The response does not include any newly created extended properties.</span></span>

<span data-ttu-id="3f677-210">新しく作成された拡張プロパティを表示するには、[拡張プロパティを使用して展開されているイベントを取得](../api/singlevaluelegacyextendedproperty_get.md)します。</span><span class="sxs-lookup"><span data-stu-id="3f677-210">To see the newly created extended property, [get the event expanded with the extended property](../api/singlevaluelegacyextendedproperty_get.md).</span></span>


****

##### <a name="request-2"></a><span data-ttu-id="3f677-211">要求 2</span><span class="sxs-lookup"><span data-stu-id="3f677-211">Request 2</span></span>

<span data-ttu-id="3f677-p109">2 番目の例では、指定した既存のメッセージに 1 つの単一値の拡張プロパティを作成します。拡張プロパティは、**singleValueExtendedProperties** 配列内の唯一の要素です。要求本文には、拡張プロパティに関する次のものが含まれています。</span><span class="sxs-lookup"><span data-stu-id="3f677-p109">The second example creates one single-value extended property for the specified existing message. That extended property is the only element in the **singleValueExtendedProperties** array. The request body includes the following for the extended property:</span></span>
- <span data-ttu-id="3f677-215">**id** は、プロパティの型を `String` (GUID) として指定し、`Color` という名前のプロパティとして指定します。</span><span class="sxs-lookup"><span data-stu-id="3f677-215">**id** specifies the property type as `String`, the GUID, and the property named `Color`.</span></span>
- <span data-ttu-id="3f677-216">**value** は、`Color` プロパティの値として `Green` を指定します。</span><span class="sxs-lookup"><span data-stu-id="3f677-216">**value** specifies `Green` as the value of the `Color` property.</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2_bs88AACHsLqWAAA=

Content-Type: application/json

{
  "singleValueExtendedProperties": [
      {
         "id":"String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color",
         "value":"Green"
      }
    ]
}
```

##### <a name="response-2"></a><span data-ttu-id="3f677-217">応答 2</span><span class="sxs-lookup"><span data-stu-id="3f677-217">Response 2</span></span>

<span data-ttu-id="3f677-p110">[メッセージの更新](../api/message_update.md)からの応答と同様に、`HTTP 200 OK` 応答コードによって正常な応答が示され、応答の本文に指定したメッセージが含まれています。応答には、新しく作成された拡張プロパティは含まれません。</span><span class="sxs-lookup"><span data-stu-id="3f677-p110">A successful response is indicated by an `HTTP 200 OK` response code, and includes the specified message in the response body, similar to the response from [updating a message](../api/message_update.md). The response does not include the newly created extended property.</span></span>

<span data-ttu-id="3f677-220">新しく作成された拡張プロパティを表示するには、[拡張プロパティを使用して展開されているメッセージを取得](../api/singlevaluelegacyextendedproperty_get.md)します。</span><span class="sxs-lookup"><span data-stu-id="3f677-220">To see the newly created extended property, [get the message expanded with the extended property](../api/singlevaluelegacyextendedproperty_get.md).</span></span>

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

