---
title: 複数値の拡張プロパティを作成する
description: 'リソースの新規または既存のインスタンスに、1 つ以上の複数値の拡張プロパティを作成します。 '
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 2e1f9840661354f9ff2d7b2e5f4386f2d17ca0fa
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35983804"
---
# <a name="create-multi-value-extended-property"></a><span data-ttu-id="f834b-103">複数値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="f834b-103">Create multi-value extended property</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f834b-104">リソースの新規または既存のインスタンスに、1 つ以上の複数値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="f834b-104">Create one or more multi-value extended properties in a new or existing instance of a resource.</span></span> 

<span data-ttu-id="f834b-105">次のユーザー リソースがサポートされます。</span><span class="sxs-lookup"><span data-stu-id="f834b-105">The following user resources are supported:</span></span>

- [<span data-ttu-id="f834b-106">calendar</span><span class="sxs-lookup"><span data-stu-id="f834b-106">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="f834b-107">contact</span><span class="sxs-lookup"><span data-stu-id="f834b-107">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="f834b-108">contactFolder</span><span class="sxs-lookup"><span data-stu-id="f834b-108">contactFolder</span></span>](../resources/contactfolder.md) 
- [<span data-ttu-id="f834b-109">event</span><span class="sxs-lookup"><span data-stu-id="f834b-109">event</span></span>](../resources/event.md)
- [<span data-ttu-id="f834b-110">mailFolder</span><span class="sxs-lookup"><span data-stu-id="f834b-110">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="f834b-111">message</span><span class="sxs-lookup"><span data-stu-id="f834b-111">message</span></span>](../resources/message.md)
- [<span data-ttu-id="f834b-112">Outlook タスク</span><span class="sxs-lookup"><span data-stu-id="f834b-112">Outlook task</span></span>](../resources/outlooktask.md)
- [<span data-ttu-id="f834b-113">Outlook タスク フォルダー</span><span class="sxs-lookup"><span data-stu-id="f834b-113">Outlook task folder</span></span>](../resources/outlooktaskfolder.md)

<span data-ttu-id="f834b-114">次のグループ リソースもサポートされます。</span><span class="sxs-lookup"><span data-stu-id="f834b-114">As well as the following group resources:</span></span>

- <span data-ttu-id="f834b-115">グループ [calendar](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="f834b-115">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="f834b-116">グループ [event](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="f834b-116">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="f834b-117">グループ [post](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="f834b-117">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="f834b-118">オープン拡張機能または拡張プロパティを使用するのに適した状況と、拡張プロパティを指定する方法の詳細については、「[拡張プロパティの概要](../resources/extended-properties-overview.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f834b-118">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="f834b-119">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f834b-119">Permissions</span></span>
<span data-ttu-id="f834b-120">この API を呼び出すには、拡張プロパティを作成しているリソースと、要求したアクセス許可の種類 (委任またはアプリケーション) によって、次の表で指定されているアクセス許可が最低限必要です。</span><span class="sxs-lookup"><span data-stu-id="f834b-120">Depending on the resource you're creating the extended property in and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="f834b-121">アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f834b-121">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f834b-122">サポートされているリソース</span><span class="sxs-lookup"><span data-stu-id="f834b-122">Supported resource</span></span> | <span data-ttu-id="f834b-123">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f834b-123">Delegated (work or school account)</span></span> | <span data-ttu-id="f834b-124">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f834b-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f834b-125">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f834b-125">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="f834b-126">calendar</span><span class="sxs-lookup"><span data-stu-id="f834b-126">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="f834b-127">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f834b-127">Calendars.ReadWrite</span></span> | <span data-ttu-id="f834b-128">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f834b-128">Calendars.ReadWrite</span></span> | <span data-ttu-id="f834b-129">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f834b-129">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="f834b-130">contact</span><span class="sxs-lookup"><span data-stu-id="f834b-130">contact</span></span>](../resources/contact.md) | <span data-ttu-id="f834b-131">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f834b-131">Contacts.ReadWrite</span></span> | <span data-ttu-id="f834b-132">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f834b-132">Contacts.ReadWrite</span></span> | <span data-ttu-id="f834b-133">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f834b-133">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="f834b-134">contactFolder</span><span class="sxs-lookup"><span data-stu-id="f834b-134">contactFolder</span></span>](../resources/contactfolder.md) | <span data-ttu-id="f834b-135">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f834b-135">Contacts.ReadWrite</span></span> | <span data-ttu-id="f834b-136">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f834b-136">Contacts.ReadWrite</span></span> | <span data-ttu-id="f834b-137">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f834b-137">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="f834b-138">イベント</span><span class="sxs-lookup"><span data-stu-id="f834b-138">event</span></span>](../resources/event.md) | <span data-ttu-id="f834b-139">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f834b-139">Calendars.ReadWrite</span></span> | <span data-ttu-id="f834b-140">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f834b-140">Calendars.ReadWrite</span></span> |  <span data-ttu-id="f834b-141">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f834b-141">Calendars.ReadWrite</span></span>|
| <span data-ttu-id="f834b-142">グループ [calendar](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="f834b-142">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="f834b-143">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f834b-143">Group.ReadWrite.All</span></span> | <span data-ttu-id="f834b-144">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="f834b-144">Not supported</span></span> | <span data-ttu-id="f834b-145">非サポート</span><span class="sxs-lookup"><span data-stu-id="f834b-145">Not supported</span></span> |
| <span data-ttu-id="f834b-146">グループ [event](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="f834b-146">group [event](../resources/event.md)</span></span> | <span data-ttu-id="f834b-147">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f834b-147">Group.ReadWrite.All</span></span> | <span data-ttu-id="f834b-148">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="f834b-148">Not supported</span></span> | <span data-ttu-id="f834b-149">非サポート</span><span class="sxs-lookup"><span data-stu-id="f834b-149">Not supported</span></span> |
| <span data-ttu-id="f834b-150">グループ [post](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="f834b-150">group [post](../resources/post.md)</span></span> | <span data-ttu-id="f834b-151">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f834b-151">Group.ReadWrite.All</span></span> | <span data-ttu-id="f834b-152">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="f834b-152">Not supported</span></span> | <span data-ttu-id="f834b-153">非サポート</span><span class="sxs-lookup"><span data-stu-id="f834b-153">Not supported</span></span> |
| [<span data-ttu-id="f834b-154">mailFolder</span><span class="sxs-lookup"><span data-stu-id="f834b-154">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="f834b-155">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f834b-155">Mail.ReadWrite</span></span> | <span data-ttu-id="f834b-156">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f834b-156">Mail.ReadWrite</span></span> | <span data-ttu-id="f834b-157">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f834b-157">Mail.ReadWrite</span></span> |
| [<span data-ttu-id="f834b-158">メッセージ</span><span class="sxs-lookup"><span data-stu-id="f834b-158">message</span></span>](../resources/message.md) | <span data-ttu-id="f834b-159">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f834b-159">Mail.ReadWrite</span></span> | <span data-ttu-id="f834b-160">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f834b-160">Mail.ReadWrite</span></span> | <span data-ttu-id="f834b-161">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f834b-161">Mail.ReadWrite</span></span> |
| [<span data-ttu-id="f834b-162">Outlook タスク</span><span class="sxs-lookup"><span data-stu-id="f834b-162">Outlook task</span></span>](../resources/outlooktask.md) | <span data-ttu-id="f834b-163">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f834b-163">Tasks.ReadWrite</span></span> | <span data-ttu-id="f834b-164">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f834b-164">Tasks.ReadWrite</span></span> | <span data-ttu-id="f834b-165">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="f834b-165">Not supported</span></span> |
| [<span data-ttu-id="f834b-166">Outlook タスク フォルダー</span><span class="sxs-lookup"><span data-stu-id="f834b-166">Outlook task folder</span></span>](../resources/outlooktaskfolder.md) | <span data-ttu-id="f834b-167">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f834b-167">Tasks.ReadWrite</span></span> | <span data-ttu-id="f834b-168">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f834b-168">Tasks.ReadWrite</span></span> | <span data-ttu-id="f834b-169">非サポート</span><span class="sxs-lookup"><span data-stu-id="f834b-169">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="f834b-170">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f834b-170">HTTP request</span></span>
<span data-ttu-id="f834b-171">新規または既存のリソースのインスタンスに、拡張プロパティを作成できます。</span><span class="sxs-lookup"><span data-stu-id="f834b-171">You can create extended properties in a new or existing resource instance.</span></span>

<span data-ttu-id="f834b-172">1 つ以上の拡張プロパティを_新しい_リソースのインスタンスに作成するには、インスタンスの作成と同じ REST 要求を使用し、新しいリソース インスタンスのプロパティ_と拡張プロパティを_要求の本文に含めます。</span><span class="sxs-lookup"><span data-stu-id="f834b-172">To create one or more extended properties in a _new_ resource instance, use the same REST request as creating the instance, and include the properties of the new resource instance _and extended property_ in the request body.</span></span>
<span data-ttu-id="f834b-173">一部のリソースでは複数の作成方法がサポートされていますので、注意してください。</span><span class="sxs-lookup"><span data-stu-id="f834b-173">Note that some resources support creation in more than one way.</span></span> <span data-ttu-id="f834b-174">これらのリソースインスタンスを作成する方法の詳細については、「 [message](../resources/message.md), [mailfolder](../api/user-post-mailfolders.md), [event](../api/user-post-events.md), [calendar](../api/user-post-calendars.md), [contact](../api/user-post-contacts.md), [contactfolder](../api/user-post-contactfolders.md), [Outlook task](../resources/outlooktask.md), [」を作成するための対応するトピックを参照してください。Outlook のタスクフォルダー](../resources/outlooktaskfolder.md)、[グループイベント](../api/group-post-events.md)、および[グループ投稿](../resources/post.md)。</span><span class="sxs-lookup"><span data-stu-id="f834b-174">For more information on creating these resource instances, see the corresponding topics for creating a [message](../resources/message.md), [mailFolder](../api/user-post-mailfolders.md), [event](../api/user-post-events.md), [calendar](../api/user-post-calendars.md), [contact](../api/user-post-contacts.md), [contactFolder](../api/user-post-contactfolders.md), [Outlook task](../resources/outlooktask.md), [Outlook task folder](../resources/outlooktaskfolder.md), [group event](../api/group-post-events.md), and [group post](../resources/post.md).</span></span> 
 
<span data-ttu-id="f834b-175">以下に要求の構文を示します。</span><span class="sxs-lookup"><span data-stu-id="f834b-175">The following is the syntax of the requests.</span></span> 

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

POST /me/outlook/tasks
POST /users/{id|userPrincipalName}/outlook/tasks
POST /me/outlook/taskFolders/{id}/tasks
POST /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks
POST /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks
POST /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks

POST /me/outlook/taskFolders
POST /users/{id|userPrincipalName}/outlook/taskFolders
POST /me/outlook/taskGroups/{id}/taskFolders
POST /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders

POST /groups/{id}/events

POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/reply
POST /groups/{id}/threads/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/reply
POST /groups/{id}/threads
POST /groups/{id}/conversations
```

<span data-ttu-id="f834b-176">既存のリソースのインスタンスで 1 つ以上の拡張プロパティを作成するには、要求でインスタンスを指定し、要求本文に拡張プロパティを含めます。</span><span class="sxs-lookup"><span data-stu-id="f834b-176">To create one or more extended properties in an existing resource instance, specify the instance in the request, and include the extended property in the request body.</span></span>

<span data-ttu-id="f834b-177">**注** 既存のグループ投稿には拡張プロパティを作成できません。</span><span class="sxs-lookup"><span data-stu-id="f834b-177">**Note** You cannot create an extended property in an existing group post.</span></span>

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

PATCH /me/outlook/tasks/{id}
PATCH /users/{id|userPrincipalName}/outlook/tasks/{id}
PATCH /me/outlook/taskFolders/{id}/tasks/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks/{id}
PATCH /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}

PATCH /me/outlook/taskFolders/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskFolders/{id}
PATCH /me/outlook/taskGroups/{id}/taskFolders/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}

PATCH /groups/{id}/events/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f834b-178">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f834b-178">Request headers</span></span>
| <span data-ttu-id="f834b-179">名前</span><span class="sxs-lookup"><span data-stu-id="f834b-179">Name</span></span>       | <span data-ttu-id="f834b-180">値</span><span class="sxs-lookup"><span data-stu-id="f834b-180">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="f834b-181">Authorization</span><span class="sxs-lookup"><span data-stu-id="f834b-181">Authorization</span></span> | <span data-ttu-id="f834b-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f834b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f834b-184">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f834b-184">Content-Type</span></span> | <span data-ttu-id="f834b-185">application/json</span><span class="sxs-lookup"><span data-stu-id="f834b-185">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="f834b-186">要求本文</span><span class="sxs-lookup"><span data-stu-id="f834b-186">Request body</span></span>

<span data-ttu-id="f834b-187">リソース インスタンスの [multiValueExtendedProperties](../resources/multivaluelegacyextendedproperty.md) コレクション プロパティに、各 **multiValueLegacyExtendedProperty** オブジェクトの JSON 本文を指定します。</span><span class="sxs-lookup"><span data-stu-id="f834b-187">Provide a JSON body of each [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object in the **multiValueExtendedProperties** collection property of the resource instance.</span></span>

|<span data-ttu-id="f834b-188">**プロパティ**</span><span class="sxs-lookup"><span data-stu-id="f834b-188">**Property**</span></span>|<span data-ttu-id="f834b-189">**型**</span><span class="sxs-lookup"><span data-stu-id="f834b-189">**Type**</span></span>|<span data-ttu-id="f834b-190">**説明**</span><span class="sxs-lookup"><span data-stu-id="f834b-190">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="f834b-191">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="f834b-191">multiValueExtendedProperties</span></span>|<span data-ttu-id="f834b-192">[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="f834b-192">[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="f834b-193">1 つ以上の複数値を持つ拡張プロパティの配列。</span><span class="sxs-lookup"><span data-stu-id="f834b-193">An array of one or more multi-valued extended properties.</span></span> |
|<span data-ttu-id="f834b-194">id</span><span class="sxs-lookup"><span data-stu-id="f834b-194">id</span></span>|<span data-ttu-id="f834b-195">String</span><span class="sxs-lookup"><span data-stu-id="f834b-195">String</span></span>|<span data-ttu-id="f834b-p104">**multiValueExtendedProperties** コレクションの各プロパティに対してこれを指定し、プロパティを特定します。サポートされている形式のいずれかに従う必要があります。詳しくは、[「Outlook の拡張プロパティの概要」](../resources/extended-properties-overview.md)をご覧ください。必須。</span><span class="sxs-lookup"><span data-stu-id="f834b-p104">For each property in the **multiValueExtendedProperties** collection, specify this to identify the property. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|
|<span data-ttu-id="f834b-200">value</span><span class="sxs-lookup"><span data-stu-id="f834b-200">value</span></span>|<span data-ttu-id="f834b-201">string</span><span class="sxs-lookup"><span data-stu-id="f834b-201">string</span></span>|<span data-ttu-id="f834b-p105">**multiValueExtendedProperties** コレクションの各プロパティに対し、プロパティの値を特定します。必須。</span><span class="sxs-lookup"><span data-stu-id="f834b-p105">For each property in the **multiValueExtendedProperties** collection, specify the property value. Required.</span></span>|

<span data-ttu-id="f834b-204">_新しい_リソース インスタンスに拡張プロパティを作成する場合は、新しい **multiValueExtendedProperties** コレクションのほか、そのリソース インスタンスの JSON 表現を指定します ([message](../resources/message.md)、[mailFolder](../resources/mailfolder.md)、[event](../resources/event.md) など)。</span><span class="sxs-lookup"><span data-stu-id="f834b-204">When creating an extended property in a _new_ resource instance, in addition to the new **multiValueExtendedProperties** collection, provide a JSON representation of that resource instance (that is, a [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), etc.)</span></span>

## <a name="response"></a><span data-ttu-id="f834b-205">応答</span><span class="sxs-lookup"><span data-stu-id="f834b-205">Response</span></span>

#### <a name="response-code"></a><span data-ttu-id="f834b-206">応答コード</span><span class="sxs-lookup"><span data-stu-id="f834b-206">Response code</span></span>
<span data-ttu-id="f834b-207">新しいリソース インスタンスに拡張プロパティが正常に作成されると、`201 Created` が返されます。ただし新しいグループ投稿の場合は別で、使用するメソッドに応じて、`200 OK` または `202 Accepted` が返されます。</span><span class="sxs-lookup"><span data-stu-id="f834b-207">An operation successful in creating an extended property in a new resource instance returns `201 Created`, except in a new group post, depending on the method used, the operation can return `200 OK` or `202 Accepted`.</span></span>

<span data-ttu-id="f834b-208">既存のリソース インスタンスに拡張プロパティが正常に作成されると、`200 OK` が返されます。</span><span class="sxs-lookup"><span data-stu-id="f834b-208">In an existing resource instance, a successful create operation returns `200 OK`.</span></span> 


#### <a name="response-body"></a><span data-ttu-id="f834b-209">応答本文</span><span class="sxs-lookup"><span data-stu-id="f834b-209">Response body</span></span>

<span data-ttu-id="f834b-p106">[グループ投稿](../resources/post.md)以外のサポートされているリソースで拡張プロパティを作成する場合、応答には新規または既存のインスタンスだけが含まれ、新しい拡張プロパティは含まれません。新しく作成された拡張プロパティを表示するには、[拡張プロパティを使用して展開されているインスタンスを取得](../api/multivaluelegacyextendedproperty-get.md)します。</span><span class="sxs-lookup"><span data-stu-id="f834b-p106">When creating an extended property in a supported resource other than [group post](../resources/post.md), the response includes only the new or existing instance but not the new extended property. To see the newly created extended property, [get the instance expanded with the extended property](../api/multivaluelegacyextendedproperty-get.md).</span></span>

<span data-ttu-id="f834b-p107">_新しい_グループ投稿に拡張プロパティを作成する場合、応答には応答コードだけが含まれ、新しい投稿や拡張プロパティは含まれません。既存のグループ投稿には拡張プロパティを作成できません。</span><span class="sxs-lookup"><span data-stu-id="f834b-p107">When creating an extended property in a _new_ group post, the response includes only a response code but not the new post nor the extended property. You cannot create an extended property in an existing group post.</span></span>


## <a name="example"></a><span data-ttu-id="f834b-214">例</span><span class="sxs-lookup"><span data-stu-id="f834b-214">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="f834b-215">要求 1</span><span class="sxs-lookup"><span data-stu-id="f834b-215">Request 1</span></span>

<span data-ttu-id="f834b-p108">最初の例では、すべて同じ POST 操作の新しいイベントで複数値の拡張プロパティを作成します。新しいイベントに通常含まれるプロパティとは別に、要求の本文に 1 つの拡張プロパティを含む **multiValueExtendedProperties** コレクションが含まれます。要求本文には、その複数値の拡張プロパティに関する次のものが含まれています。</span><span class="sxs-lookup"><span data-stu-id="f834b-p108">The first example creates a multi-value extended property in a new event all in the same POST operation. Apart from the properties you'd normally include for a new event, the request body includes the **multiValueExtendedProperties** collection which contains one extended property. The request body includes the following for that multi-value extended property:</span></span>

- <span data-ttu-id="f834b-219">**id** 指定された GUID と名前 `Recreation` の文字列の配列としてプロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="f834b-219">**id** which specifies the property as an array of strings with the specified GUID and the name `Recreation`.</span></span> 
- <span data-ttu-id="f834b-220">**value** は、3 つの文字列値 `Recreation` の配列として `["Food", "Hiking", "Swimming"]` を指定します。</span><span class="sxs-lookup"><span data-stu-id="f834b-220">**value** which specifies `Recreation` as an array of 3 string values, `["Food", "Hiking", "Swimming"]`.</span></span>
 

<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/me/events
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

##### <a name="response-1"></a><span data-ttu-id="f834b-221">応答 1</span><span class="sxs-lookup"><span data-stu-id="f834b-221">Response 1</span></span>

<span data-ttu-id="f834b-p109">`HTTP 201 Created`からの応答と同様に、[](../api/user-post-events.md) 応答コードによって正常な応答が示され、応答の本文に新しいイベントが含まれます。応答には、新しく作成された拡張プロパティは含まれません。</span><span class="sxs-lookup"><span data-stu-id="f834b-p109">A successful response is indicated by an `HTTP 201 Created` response code, and includes the new event in the response body, similar to the response from [creating just an event](../api/user-post-events.md). The response does not include any newly created extended properties.</span></span>

<span data-ttu-id="f834b-224">新しく作成された拡張プロパティを表示するには、[拡張プロパティを使用して展開されているイベントを取得](../api/multivaluelegacyextendedproperty-get.md)します。</span><span class="sxs-lookup"><span data-stu-id="f834b-224">To see the newly created extended property, [get the event expanded with the extended property](../api/multivaluelegacyextendedproperty-get.md).</span></span>


****

##### <a name="request-2"></a><span data-ttu-id="f834b-225">要求 2</span><span class="sxs-lookup"><span data-stu-id="f834b-225">Request 2</span></span>

<span data-ttu-id="f834b-p110">2 番目の例では、指定したメッセージに対して 1 つの複数値の拡張プロパティを作成します。拡張プロパティは、**multiValueExtendedProperties** コレクションの唯一の要素です。要求本文には、拡張プロパティに関する次のものが含まれています。</span><span class="sxs-lookup"><span data-stu-id="f834b-p110">The second example creates one multi-value extended property for the specified message. That extended property is the only element in the **multiValueExtendedProperties** collection. The request body includes the following for the extended property:</span></span>

- <span data-ttu-id="f834b-229">**id** 指定された GUID と名前 `Palette` を使って、文字列の配列としてプロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="f834b-229">**id** specifies the property as an array of strings with the specified GUID and the name `Palette`.</span></span>
- <span data-ttu-id="f834b-230">**value** 3 つの文字列値 `Palette` の配列として `["Green", "Aqua", "Blue"]` を指定します。</span><span class="sxs-lookup"><span data-stu-id="f834b-230">**value** specifies `Palette` as an array of 3 string values, `["Green", "Aqua", "Blue"]`.</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/beta/me/messages('AAMkAGE1M2_as77AACHsLrBBBA=')

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

##### <a name="response-2"></a><span data-ttu-id="f834b-231">応答 2</span><span class="sxs-lookup"><span data-stu-id="f834b-231">Response 2</span></span>

<span data-ttu-id="f834b-p111">[メッセージの更新](../api/message-update.md)からの応答と同様に、`HTTP 200 OK` 応答コードによって正常な応答が示され、応答の本文に指定したメッセージが含まれています。応答には、新しく作成された拡張プロパティは含まれません。</span><span class="sxs-lookup"><span data-stu-id="f834b-p111">A successful response is indicated by an `HTTP 200 OK` response code, and includes the specified message in the response body, similar to the response from [updating a message](../api/message-update.md). The response does not include the newly created extended property.</span></span>

<span data-ttu-id="f834b-234">新しく作成された拡張プロパティを表示するには、[拡張プロパティを使用して展開されているメッセージを取得](../api/multivaluelegacyextendedproperty-get.md)します。</span><span class="sxs-lookup"><span data-stu-id="f834b-234">To see the newly created extended property, [get the message expanded with the extended property](../api/multivaluelegacyextendedproperty-get.md).</span></span>


<!-- This page was manually created. -->
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create a single-value extended property",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->




