---
title: 単一値の拡張プロパティを作成する
description: 'リソースの新規または既存のインスタンスに、1 つ以上の単一値の拡張プロパティを作成します。 '
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: c90c8fca501e813635e3e3b208c1a5be6808b728
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35975593"
---
# <a name="create-single-value-extended-property"></a><span data-ttu-id="e1a01-103">単一値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="e1a01-103">Create single-value extended property</span></span>

<span data-ttu-id="e1a01-104">リソースの新規または既存のインスタンスに、1 つ以上の単一値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="e1a01-104">Create one or more single-value extended properties in a new or existing instance of a resource.</span></span> 

<span data-ttu-id="e1a01-105">次のユーザー リソースがサポートされます。</span><span class="sxs-lookup"><span data-stu-id="e1a01-105">The following user resources are supported:</span></span>

- [<span data-ttu-id="e1a01-106">calendar</span><span class="sxs-lookup"><span data-stu-id="e1a01-106">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="e1a01-107">contact</span><span class="sxs-lookup"><span data-stu-id="e1a01-107">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="e1a01-108">contactFolder</span><span class="sxs-lookup"><span data-stu-id="e1a01-108">contactFolder</span></span>](../resources/contactfolder.md) 
- [<span data-ttu-id="e1a01-109">event</span><span class="sxs-lookup"><span data-stu-id="e1a01-109">event</span></span>](../resources/event.md)
- [<span data-ttu-id="e1a01-110">mailFolder</span><span class="sxs-lookup"><span data-stu-id="e1a01-110">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="e1a01-111">message</span><span class="sxs-lookup"><span data-stu-id="e1a01-111">message</span></span>](../resources/message.md)

<span data-ttu-id="e1a01-112">次のグループ リソースもサポートされます。</span><span class="sxs-lookup"><span data-stu-id="e1a01-112">As well as the following group resources:</span></span>

- <span data-ttu-id="e1a01-113">グループ [calendar](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="e1a01-113">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="e1a01-114">グループ [event](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="e1a01-114">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="e1a01-115">グループ [post](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="e1a01-115">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="e1a01-116">オープン拡張機能または拡張プロパティを使用するのに適した状況と、拡張プロパティを指定する方法の詳細については、「[拡張プロパティの概要](../resources/extended-properties-overview.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e1a01-116">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="e1a01-117">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e1a01-117">Permissions</span></span>
<span data-ttu-id="e1a01-118">この API を呼び出すには、拡張プロパティを作成しているリソースと、要求したアクセス許可の種類 (委任またはアプリケーション) によって、次の表で指定されているアクセス許可が最低限必要です。</span><span class="sxs-lookup"><span data-stu-id="e1a01-118">Depending on the resource you're creating the extended property in and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="e1a01-119">アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e1a01-119">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e1a01-120">サポートされているリソース</span><span class="sxs-lookup"><span data-stu-id="e1a01-120">Supported resource</span></span> | <span data-ttu-id="e1a01-121">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e1a01-121">Delegated (work or school account)</span></span> | <span data-ttu-id="e1a01-122">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e1a01-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1a01-123">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e1a01-123">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="e1a01-124">calendar</span><span class="sxs-lookup"><span data-stu-id="e1a01-124">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="e1a01-125">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1a01-125">Calendars.ReadWrite</span></span> | <span data-ttu-id="e1a01-126">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1a01-126">Calendars.ReadWrite</span></span> | <span data-ttu-id="e1a01-127">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1a01-127">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="e1a01-128">contact</span><span class="sxs-lookup"><span data-stu-id="e1a01-128">contact</span></span>](../resources/contact.md) | <span data-ttu-id="e1a01-129">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1a01-129">Contacts.ReadWrite</span></span> | <span data-ttu-id="e1a01-130">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1a01-130">Contacts.ReadWrite</span></span> | <span data-ttu-id="e1a01-131">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1a01-131">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="e1a01-132">contactFolder</span><span class="sxs-lookup"><span data-stu-id="e1a01-132">contactFolder</span></span>](../resources/contactfolder.md) | <span data-ttu-id="e1a01-133">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1a01-133">Contacts.ReadWrite</span></span> | <span data-ttu-id="e1a01-134">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1a01-134">Contacts.ReadWrite</span></span> | <span data-ttu-id="e1a01-135">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1a01-135">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="e1a01-136">イベント</span><span class="sxs-lookup"><span data-stu-id="e1a01-136">event</span></span>](../resources/event.md) | <span data-ttu-id="e1a01-137">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1a01-137">Calendars.ReadWrite</span></span> | <span data-ttu-id="e1a01-138">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1a01-138">Calendars.ReadWrite</span></span> |  <span data-ttu-id="e1a01-139">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1a01-139">Calendars.ReadWrite</span></span>|
| <span data-ttu-id="e1a01-140">グループ [calendar](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="e1a01-140">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="e1a01-141">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1a01-141">Group.ReadWrite.All</span></span> | <span data-ttu-id="e1a01-142">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="e1a01-142">Not supported</span></span> | <span data-ttu-id="e1a01-143">非サポート</span><span class="sxs-lookup"><span data-stu-id="e1a01-143">Not supported</span></span> |
| <span data-ttu-id="e1a01-144">グループ [event](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="e1a01-144">group [event](../resources/event.md)</span></span> | <span data-ttu-id="e1a01-145">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1a01-145">Group.ReadWrite.All</span></span> | <span data-ttu-id="e1a01-146">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="e1a01-146">Not supported</span></span> | <span data-ttu-id="e1a01-147">非サポート</span><span class="sxs-lookup"><span data-stu-id="e1a01-147">Not supported</span></span> |
| <span data-ttu-id="e1a01-148">グループ [post](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="e1a01-148">group [post](../resources/post.md)</span></span> | <span data-ttu-id="e1a01-149">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1a01-149">Group.ReadWrite.All</span></span> | <span data-ttu-id="e1a01-150">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="e1a01-150">Not supported</span></span> | <span data-ttu-id="e1a01-151">非サポート</span><span class="sxs-lookup"><span data-stu-id="e1a01-151">Not supported</span></span> |
| [<span data-ttu-id="e1a01-152">mailFolder</span><span class="sxs-lookup"><span data-stu-id="e1a01-152">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="e1a01-153">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1a01-153">Mail.ReadWrite</span></span> | <span data-ttu-id="e1a01-154">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1a01-154">Mail.ReadWrite</span></span> | <span data-ttu-id="e1a01-155">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1a01-155">Mail.ReadWrite</span></span> |
| [<span data-ttu-id="e1a01-156">メッセージ</span><span class="sxs-lookup"><span data-stu-id="e1a01-156">message</span></span>](../resources/message.md) | <span data-ttu-id="e1a01-157">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1a01-157">Mail.ReadWrite</span></span> | <span data-ttu-id="e1a01-158">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1a01-158">Mail.ReadWrite</span></span> | <span data-ttu-id="e1a01-159">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1a01-159">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e1a01-160">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e1a01-160">HTTP request</span></span>
<span data-ttu-id="e1a01-161">新規または既存のリソースのインスタンスに、拡張プロパティを作成できます。</span><span class="sxs-lookup"><span data-stu-id="e1a01-161">You can create extended properties in a new or existing resource instance.</span></span>

<span data-ttu-id="e1a01-p102">1 つ以上の拡張プロパティを_新しい_リソースのインスタンスに作成するには、インスタンスの作成と同じ REST 要求を使用し、新しいリソース インスタンスのプロパティ_と拡張プロパティを_要求の本文に含めます。一部のリソースでは複数の作成方法がサポートされていますので、注意してください。これらのリソース インスタンスの作成に関して詳しくは、[メッセージ](../resources/message.md)、[mailFolder](../api/user-post-mailfolders.md)、[イベント](../api/user-post-events.md)、[予定表](../api/user-post-calendars.md)、[連絡先](../api/user-post-contacts.md)、[contactFolder](../api/user-post-contactfolders.md)、[グループ イベント](../api/group-post-events.md)、および [グループ投稿](../resources/post.md)作成の該当する各トピックをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="e1a01-p102">To create one or more extended properties in a _new_ resource instance, use the same REST request as creating the instance, and include the properties of the new resource instance _and extended property_ in the request body. Note that some resources support creation in more than one way. For more information on creating these resource instances, see the corresponding topics for creating a [message](../resources/message.md), [mailFolder](../api/user-post-mailfolders.md), [event](../api/user-post-events.md), [calendar](../api/user-post-calendars.md), [contact](../api/user-post-contacts.md), [contactFolder](../api/user-post-contactfolders.md), [group event](../api/group-post-events.md), and [group post](../resources/post.md).</span></span> 
 
<span data-ttu-id="e1a01-165">以下に要求の構文を示します。</span><span class="sxs-lookup"><span data-stu-id="e1a01-165">The following is the syntax of the requests.</span></span> 

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

<span data-ttu-id="e1a01-166">既存のリソースのインスタンスで 1 つ以上の拡張プロパティを作成するには、要求でインスタンスを指定し、要求本文に拡張プロパティを含めます。</span><span class="sxs-lookup"><span data-stu-id="e1a01-166">To create one or more extended properties in an existing resource instance, specify the instance in the request, and include the extended property in the request body.</span></span>

<span data-ttu-id="e1a01-167">**注** 既存のグループ投稿には拡張プロパティを作成できません。</span><span class="sxs-lookup"><span data-stu-id="e1a01-167">**Note** You cannot create an extended property in an existing group post.</span></span>

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

## <a name="request-headers"></a><span data-ttu-id="e1a01-168">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e1a01-168">Request headers</span></span>
| <span data-ttu-id="e1a01-169">名前</span><span class="sxs-lookup"><span data-stu-id="e1a01-169">Name</span></span>       | <span data-ttu-id="e1a01-170">値</span><span class="sxs-lookup"><span data-stu-id="e1a01-170">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="e1a01-171">Authorization</span><span class="sxs-lookup"><span data-stu-id="e1a01-171">Authorization</span></span> | <span data-ttu-id="e1a01-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e1a01-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e1a01-174">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e1a01-174">Content-Type</span></span> | <span data-ttu-id="e1a01-175">application/json</span><span class="sxs-lookup"><span data-stu-id="e1a01-175">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="e1a01-176">要求本文</span><span class="sxs-lookup"><span data-stu-id="e1a01-176">Request body</span></span>

<span data-ttu-id="e1a01-177">リソース インスタンスの [singleValueExtendedProperties](../resources/singlevaluelegacyextendedproperty.md) コレクション プロパティに、各 **singleValueLegacyExtendedProperty** オブジェクトの JSON 本文を指定します。</span><span class="sxs-lookup"><span data-stu-id="e1a01-177">Provide a JSON body of each [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object in the **singleValueExtendedProperties** collection property of the resource instance.</span></span>

|<span data-ttu-id="e1a01-178">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e1a01-178">Property</span></span>|<span data-ttu-id="e1a01-179">型</span><span class="sxs-lookup"><span data-stu-id="e1a01-179">Type</span></span>|<span data-ttu-id="e1a01-180">説明</span><span class="sxs-lookup"><span data-stu-id="e1a01-180">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="e1a01-181">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="e1a01-181">singleValueExtendedProperties</span></span>|<span data-ttu-id="e1a01-182">[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e1a01-182">[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="e1a01-183">1 つ以上の単一値を持つ拡張プロパティの配列。</span><span class="sxs-lookup"><span data-stu-id="e1a01-183">An array of one or more single-valued extended properties.</span></span> |
|<span data-ttu-id="e1a01-184">id</span><span class="sxs-lookup"><span data-stu-id="e1a01-184">id</span></span>|<span data-ttu-id="e1a01-185">String</span><span class="sxs-lookup"><span data-stu-id="e1a01-185">String</span></span>|<span data-ttu-id="e1a01-p104">**singleValueExtendedProperties** コレクションの各プロパティに対して、これを指定することでプロパティを特定します。サポートされている形式のいずれかに従う必要があります。詳しくは、「[Outlook の拡張プロパティの概要](../resources/extended-properties-overview.md)」を参照してください。必須。</span><span class="sxs-lookup"><span data-stu-id="e1a01-p104">For each property in the **singleValueExtendedProperties** collection, specify this to identify the property. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|
|<span data-ttu-id="e1a01-190">value</span><span class="sxs-lookup"><span data-stu-id="e1a01-190">value</span></span>|<span data-ttu-id="e1a01-191">string</span><span class="sxs-lookup"><span data-stu-id="e1a01-191">string</span></span>|<span data-ttu-id="e1a01-p105">**singleValueExtendedProperties** コレクションの各プロパティについて、プロパティの値を特定します。必須。</span><span class="sxs-lookup"><span data-stu-id="e1a01-p105">For each property in the **singleValueExtendedProperties** collection, specify the property value. Required.</span></span>|

<span data-ttu-id="e1a01-194">_新しい_リソース インスタンスに拡張プロパティを作成する場合は、新しい **singleValueExtendedProperties**コレクションのほか、そのリソース インスタンスの JSON 表現を指定します ([message](../resources/message.md)、[mailFolder](../resources/mailfolder.md)、[event](../resources/event.md) など)。</span><span class="sxs-lookup"><span data-stu-id="e1a01-194">When creating an extended property in a _new_ resource instance, in addition to the new **singleValueExtendedProperties** collection, provide a JSON representation of that resource instance (that is, a [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), etc.)</span></span>

## <a name="response"></a><span data-ttu-id="e1a01-195">応答</span><span class="sxs-lookup"><span data-stu-id="e1a01-195">Response</span></span>

#### <a name="response-code"></a><span data-ttu-id="e1a01-196">応答コード</span><span class="sxs-lookup"><span data-stu-id="e1a01-196">Response code</span></span>
<span data-ttu-id="e1a01-197">新しいリソース インスタンスに拡張プロパティが正常に作成されると、`201 Created` が返されます。ただし新しいグループ投稿の場合は別で、使用するメソッドに応じて、`200 OK` または `202 Accepted` が返されます。</span><span class="sxs-lookup"><span data-stu-id="e1a01-197">An operation successful in creating an extended property in a new resource instance returns `201 Created`, except in a new group post, depending on the method used, the operation can return `200 OK` or `202 Accepted`.</span></span>

<span data-ttu-id="e1a01-198">既存のリソース インスタンスに拡張プロパティが正常に作成されると、`200 OK` が返されます。</span><span class="sxs-lookup"><span data-stu-id="e1a01-198">In an existing resource instance, a successful create operation returns `200 OK`.</span></span> 


#### <a name="response-body"></a><span data-ttu-id="e1a01-199">応答本文</span><span class="sxs-lookup"><span data-stu-id="e1a01-199">Response body</span></span>

<span data-ttu-id="e1a01-p106">拡張プロパティを作成する場合、応答には新規または既存のインスタンスのみを含めて、新しい拡張プロパティは含めません。新しく作成された拡張プロパティを表示するには、[拡張プロパティを使用して展開されているインスタンスを取得](../api/singlevaluelegacyextendedproperty-get.md)します。</span><span class="sxs-lookup"><span data-stu-id="e1a01-p106">When creating an extended property, the response includes only the new or existing instance but not the new extended property. To see the newly created extended property, [get the instance expanded with the extended property](../api/singlevaluelegacyextendedproperty-get.md).</span></span>

<span data-ttu-id="e1a01-202">スレッドまたは投稿に返信することで、_新しい_[グループ投稿](../resources/post.md)に拡張プロパティを作成する場合、応答には応答コードのみを含めて、新しい投稿や拡張プロパティは含めません。</span><span class="sxs-lookup"><span data-stu-id="e1a01-202">When creating an extended property in a _new_ [group post](../resources/post.md) by replying to a thread or post, the response includes only a response code but not the new post nor the extended property.</span></span>



## <a name="example"></a><span data-ttu-id="e1a01-203">例</span><span class="sxs-lookup"><span data-stu-id="e1a01-203">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="e1a01-204">要求 1</span><span class="sxs-lookup"><span data-stu-id="e1a01-204">Request 1</span></span>

<span data-ttu-id="e1a01-p107">最初の例では、同じ POST 操作で新しいイベントと単一値の拡張プロパティを作成します。新しいイベントに通常含めるプロパティとは別に、1 つの単一値の拡張プロパティを含む **singleValueExtendedProperties** コレクションを要求の本文に含め、そのプロパティは次のようにします。</span><span class="sxs-lookup"><span data-stu-id="e1a01-p107">The first example creates a new event and a single-value extended property in the same POST operation. Apart from the properties you'd normally include for a new event, the request body includes the **singleValueExtendedProperties** collection that contains one single-value extended property, and the following for the property:</span></span>
- <span data-ttu-id="e1a01-207">**id** は、プロパティの型を `String` (GUID) として指定し、`Fun` という名前のプロパティとして指定します。</span><span class="sxs-lookup"><span data-stu-id="e1a01-207">**id** specifies the property type as `String`, the GUID, and the property named `Fun`.</span></span>
- <span data-ttu-id="e1a01-208">**value** は、`Food` プロパティの値として `Fun` を指定します。</span><span class="sxs-lookup"><span data-stu-id="e1a01-208">**value** specifies `Food` as the value of the `Fun` property.</span></span> 

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

##### <a name="response-1"></a><span data-ttu-id="e1a01-209">応答 1</span><span class="sxs-lookup"><span data-stu-id="e1a01-209">Response 1</span></span>

<span data-ttu-id="e1a01-p108">`HTTP 201 Created`からの応答と同様に、[](../api/user-post-events.md) 応答コードによって正常な応答が示され、応答の本文に新しいイベントが含まれます。応答には、新しく作成された拡張プロパティは含まれません。</span><span class="sxs-lookup"><span data-stu-id="e1a01-p108">A successful response is indicated by an `HTTP 201 Created` response code, and includes the new event in the response body, similar to the response from [creating just an event](../api/user-post-events.md). The response does not include any newly created extended properties.</span></span>

<span data-ttu-id="e1a01-212">新しく作成された拡張プロパティを表示するには、[拡張プロパティを使用して展開されているイベントを取得](../api/singlevaluelegacyextendedproperty-get.md)します。</span><span class="sxs-lookup"><span data-stu-id="e1a01-212">To see the newly created extended property, [get the event expanded with the extended property](../api/singlevaluelegacyextendedproperty-get.md).</span></span>


****

##### <a name="request-2"></a><span data-ttu-id="e1a01-213">要求 2</span><span class="sxs-lookup"><span data-stu-id="e1a01-213">Request 2</span></span>

<span data-ttu-id="e1a01-p109">2 番目の例では、指定した既存のメッセージに 1 つの単一値の拡張プロパティを作成します。拡張プロパティは、**singleValueExtendedProperties** 配列内の唯一の要素です。要求本文には、拡張プロパティに関する次のものが含まれています。</span><span class="sxs-lookup"><span data-stu-id="e1a01-p109">The second example creates one single-value extended property for the specified existing message. That extended property is the only element in the **singleValueExtendedProperties** array. The request body includes the following for the extended property:</span></span>
- <span data-ttu-id="e1a01-217">**id** は、プロパティの型を `String` (GUID) として指定し、`Color` という名前のプロパティとして指定します。</span><span class="sxs-lookup"><span data-stu-id="e1a01-217">**id** specifies the property type as `String`, the GUID, and the property named `Color`.</span></span>
- <span data-ttu-id="e1a01-218">**value** は、`Green` プロパティの値として `Color` を指定します。</span><span class="sxs-lookup"><span data-stu-id="e1a01-218">**value** specifies `Green` as the value of the `Color` property.</span></span>

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

##### <a name="response-2"></a><span data-ttu-id="e1a01-219">応答 2</span><span class="sxs-lookup"><span data-stu-id="e1a01-219">Response 2</span></span>

<span data-ttu-id="e1a01-p110">[メッセージの更新](../api/message-update.md)からの応答と同様に、`HTTP 200 OK` 応答コードによって正常な応答が示され、応答の本文に指定したメッセージが含まれています。応答には、新しく作成された拡張プロパティは含まれません。</span><span class="sxs-lookup"><span data-stu-id="e1a01-p110">A successful response is indicated by an `HTTP 200 OK` response code, and includes the specified message in the response body, similar to the response from [updating a message](../api/message-update.md). The response does not include the newly created extended property.</span></span>

<span data-ttu-id="e1a01-222">新しく作成された拡張プロパティを表示するには、[拡張プロパティを使用して展開されているメッセージを取得](../api/singlevaluelegacyextendedproperty-get.md)します。</span><span class="sxs-lookup"><span data-stu-id="e1a01-222">To see the newly created extended property, [get the message expanded with the extended property](../api/singlevaluelegacyextendedproperty-get.md).</span></span>

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

