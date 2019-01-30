---
title: 単一値の拡張プロパティを作成する
description: 'リソースの新規または既存のインスタンスに、1 つ以上の単一値の拡張プロパティを作成します。 '
localization_priority: Normal
ms.openlocfilehash: 3b122eb1a02ddd9e413f5c58bf840b912dd8365f
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641394"
---
# <a name="create-single-value-extended-property"></a><span data-ttu-id="108f4-103">単一値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="108f4-103">Create single-value extended property</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="108f4-104">リソースの新規または既存のインスタンスに、1 つ以上の単一値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="108f4-104">Create one or more single-value extended properties in a new or existing instance of a resource.</span></span> 

<span data-ttu-id="108f4-105">次のユーザー リソースがサポートされます。</span><span class="sxs-lookup"><span data-stu-id="108f4-105">The following user resources are supported:</span></span>

- [<span data-ttu-id="108f4-106">calendar</span><span class="sxs-lookup"><span data-stu-id="108f4-106">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="108f4-107">contact</span><span class="sxs-lookup"><span data-stu-id="108f4-107">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="108f4-108">contactFolder</span><span class="sxs-lookup"><span data-stu-id="108f4-108">contactFolder</span></span>](../resources/contactfolder.md) 
- [<span data-ttu-id="108f4-109">event</span><span class="sxs-lookup"><span data-stu-id="108f4-109">event</span></span>](../resources/event.md)
- [<span data-ttu-id="108f4-110">mailFolder</span><span class="sxs-lookup"><span data-stu-id="108f4-110">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="108f4-111">message</span><span class="sxs-lookup"><span data-stu-id="108f4-111">message</span></span>](../resources/message.md)
- [<span data-ttu-id="108f4-112">Outlook タスク</span><span class="sxs-lookup"><span data-stu-id="108f4-112">Outlook task</span></span>](../resources/outlooktask.md)
- [<span data-ttu-id="108f4-113">Outlook の仕事フォルダー</span><span class="sxs-lookup"><span data-stu-id="108f4-113">Outlook task folder</span></span>](../resources/outlooktaskfolder.md)

<span data-ttu-id="108f4-114">次のグループ リソースもサポートされます。</span><span class="sxs-lookup"><span data-stu-id="108f4-114">As well as the following group resources:</span></span>

- <span data-ttu-id="108f4-115">グループ [calendar](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="108f4-115">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="108f4-116">グループ [event](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="108f4-116">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="108f4-117">グループ [post](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="108f4-117">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="108f4-118">オープン拡張機能または拡張プロパティを使用するのに適した状況と、拡張プロパティを指定する方法の詳細については、「[拡張プロパティの概要](../resources/extended-properties-overview.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="108f4-118">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="108f4-119">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="108f4-119">Permissions</span></span>
<span data-ttu-id="108f4-120">リソースに応じて、[拡張プロパティを作成するアクセス許可が委任された (アプリケーション) を要求を入力、次の表で指定されたアクセス許可は、この API を呼び出すために必要最低限。</span><span class="sxs-lookup"><span data-stu-id="108f4-120">Depending on the resource you're creating the extended property in and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="108f4-121">アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="108f4-121">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="108f4-122">サポートされているリソース</span><span class="sxs-lookup"><span data-stu-id="108f4-122">Supported resource</span></span> | <span data-ttu-id="108f4-123">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="108f4-123">Delegated (work or school account)</span></span> | <span data-ttu-id="108f4-124">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="108f4-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="108f4-125">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="108f4-125">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="108f4-126">calendar</span><span class="sxs-lookup"><span data-stu-id="108f4-126">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="108f4-127">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="108f4-127">Calendars.ReadWrite</span></span> | <span data-ttu-id="108f4-128">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="108f4-128">Calendars.ReadWrite</span></span> | <span data-ttu-id="108f4-129">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="108f4-129">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="108f4-130">連絡先</span><span class="sxs-lookup"><span data-stu-id="108f4-130">contact</span></span>](../resources/contact.md) | <span data-ttu-id="108f4-131">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="108f4-131">Contacts.ReadWrite</span></span> | <span data-ttu-id="108f4-132">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="108f4-132">Contacts.ReadWrite</span></span> | <span data-ttu-id="108f4-133">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="108f4-133">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="108f4-134">contactFolder</span><span class="sxs-lookup"><span data-stu-id="108f4-134">contactFolder</span></span>](../resources/contactfolder.md) | <span data-ttu-id="108f4-135">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="108f4-135">Contacts.ReadWrite</span></span> | <span data-ttu-id="108f4-136">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="108f4-136">Contacts.ReadWrite</span></span> | <span data-ttu-id="108f4-137">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="108f4-137">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="108f4-138">イベント</span><span class="sxs-lookup"><span data-stu-id="108f4-138">event</span></span>](../resources/event.md) | <span data-ttu-id="108f4-139">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="108f4-139">Calendars.ReadWrite</span></span> | <span data-ttu-id="108f4-140">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="108f4-140">Calendars.ReadWrite</span></span> |  <span data-ttu-id="108f4-141">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="108f4-141">Calendars.ReadWrite</span></span>|
| <span data-ttu-id="108f4-142">グループ [calendar](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="108f4-142">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="108f4-143">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="108f4-143">Group.ReadWrite.All</span></span> | <span data-ttu-id="108f4-144">使用不可</span><span class="sxs-lookup"><span data-stu-id="108f4-144">Not supported</span></span> | <span data-ttu-id="108f4-145">使用不可</span><span class="sxs-lookup"><span data-stu-id="108f4-145">Not supported</span></span> |
| <span data-ttu-id="108f4-146">グループ [event](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="108f4-146">group [event](../resources/event.md)</span></span> | <span data-ttu-id="108f4-147">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="108f4-147">Group.ReadWrite.All</span></span> | <span data-ttu-id="108f4-148">使用不可</span><span class="sxs-lookup"><span data-stu-id="108f4-148">Not supported</span></span> | <span data-ttu-id="108f4-149">使用不可</span><span class="sxs-lookup"><span data-stu-id="108f4-149">Not supported</span></span> |
| <span data-ttu-id="108f4-150">グループ [post](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="108f4-150">group [post](../resources/post.md)</span></span> | <span data-ttu-id="108f4-151">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="108f4-151">Group.ReadWrite.All</span></span> | <span data-ttu-id="108f4-152">使用不可</span><span class="sxs-lookup"><span data-stu-id="108f4-152">Not supported</span></span> | <span data-ttu-id="108f4-153">使用不可</span><span class="sxs-lookup"><span data-stu-id="108f4-153">Not supported</span></span> |
| [<span data-ttu-id="108f4-154">mailFolder</span><span class="sxs-lookup"><span data-stu-id="108f4-154">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="108f4-155">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="108f4-155">Mail.ReadWrite</span></span> | <span data-ttu-id="108f4-156">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="108f4-156">Mail.ReadWrite</span></span> | <span data-ttu-id="108f4-157">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="108f4-157">Mail.ReadWrite</span></span> |
| [<span data-ttu-id="108f4-158">メッセージ</span><span class="sxs-lookup"><span data-stu-id="108f4-158">message</span></span>](../resources/message.md) | <span data-ttu-id="108f4-159">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="108f4-159">Mail.ReadWrite</span></span> | <span data-ttu-id="108f4-160">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="108f4-160">Mail.ReadWrite</span></span> | <span data-ttu-id="108f4-161">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="108f4-161">Mail.ReadWrite</span></span> |
| [<span data-ttu-id="108f4-162">Outlook タスク</span><span class="sxs-lookup"><span data-stu-id="108f4-162">Outlook task</span></span>](../resources/outlooktask.md) | <span data-ttu-id="108f4-163">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="108f4-163">Tasks.ReadWrite</span></span> | <span data-ttu-id="108f4-164">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="108f4-164">Tasks.ReadWrite</span></span> | <span data-ttu-id="108f4-165">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="108f4-165">Not supported</span></span> |
| [<span data-ttu-id="108f4-166">Outlook の仕事フォルダー</span><span class="sxs-lookup"><span data-stu-id="108f4-166">Outlook task folder</span></span>](../resources/outlooktaskfolder.md) | <span data-ttu-id="108f4-167">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="108f4-167">Tasks.ReadWrite</span></span> | <span data-ttu-id="108f4-168">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="108f4-168">Tasks.ReadWrite</span></span> | <span data-ttu-id="108f4-169">非サポート</span><span class="sxs-lookup"><span data-stu-id="108f4-169">Not supported</span></span> |
 
## <a name="http-request"></a><span data-ttu-id="108f4-170">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="108f4-170">HTTP request</span></span>
<span data-ttu-id="108f4-171">新規または既存のリソースのインスタンスに、拡張プロパティを作成できます。</span><span class="sxs-lookup"><span data-stu-id="108f4-171">You can create extended properties in a new or existing resource instance.</span></span>

<span data-ttu-id="108f4-172">_新しい_リソースのインスタンスで 1 つまたは複数の拡張プロパティを作成、インスタンスを作成すると同じの残りの要求を使用して、要求の本文で、新しいリソースのインスタンス_と拡張プロパティ_のプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="108f4-172">To create one or more extended properties in a _new_ resource instance, use the same REST request as creating the instance, and include the properties of the new resource instance _and extended property_ in the request body.</span></span>
<span data-ttu-id="108f4-173">いくつかのリソースが 1 つ以上の方法での作成をサポートすることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="108f4-173">Note that some resources support creation in more than one way.</span></span> <span data-ttu-id="108f4-174">[メッセージ](../resources/message.md)、 [mailFolder](../api/user-post-mailfolders.md)、[イベント](../api/user-post-events.md)、[予定表](../api/user-post-calendars.md)、[連絡先](../api/user-post-contacts.md)、 [contactFolder](../api/user-post-contactfolders.md)を作成するための対応するトピックを参照してくださいこれらのリソースのインスタンスを作成する方法の詳細については、 [Outlook の仕事](../resources/outlooktask.md)、 [Outlook の仕事フォルダー](../resources/outlooktaskfolder.md)、[グループのイベント](../api/group-post-events.md)、および[グループの投稿](../resources/post.md)です。</span><span class="sxs-lookup"><span data-stu-id="108f4-174">For more information on creating these resource instances, see the corresponding topics for creating a [message](../resources/message.md), [mailFolder](../api/user-post-mailfolders.md), [event](../api/user-post-events.md), [calendar](../api/user-post-calendars.md), [contact](../api/user-post-contacts.md), [contactFolder](../api/user-post-contactfolders.md), [Outlook task](../resources/outlooktask.md), [Outlook task folder](../resources/outlooktaskfolder.md), [group event](../api/group-post-events.md), and [group post](../resources/post.md).</span></span> 
 
<span data-ttu-id="108f4-175">以下に要求の構文を示します。</span><span class="sxs-lookup"><span data-stu-id="108f4-175">The following is the syntax of the requests.</span></span> 

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

<span data-ttu-id="108f4-176">既存のリソースのインスタンスで 1 つ以上の拡張プロパティを作成するには、要求でインスタンスを指定し、要求本文に拡張プロパティを含めます。</span><span class="sxs-lookup"><span data-stu-id="108f4-176">To create one or more extended properties in an existing resource instance, specify the instance in the request, and include the extended property in the request body.</span></span>

<span data-ttu-id="108f4-177">**注** 既存のグループ投稿には拡張プロパティを作成できません。</span><span class="sxs-lookup"><span data-stu-id="108f4-177">**Note** You cannot create an extended property in an existing group post.</span></span>

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

## <a name="request-headers"></a><span data-ttu-id="108f4-178">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="108f4-178">Request headers</span></span>
| <span data-ttu-id="108f4-179">名前</span><span class="sxs-lookup"><span data-stu-id="108f4-179">Name</span></span>       | <span data-ttu-id="108f4-180">値</span><span class="sxs-lookup"><span data-stu-id="108f4-180">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="108f4-181">Authorization</span><span class="sxs-lookup"><span data-stu-id="108f4-181">Authorization</span></span> | <span data-ttu-id="108f4-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="108f4-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="108f4-184">Content-Type</span><span class="sxs-lookup"><span data-stu-id="108f4-184">Content-Type</span></span> | <span data-ttu-id="108f4-185">application/json</span><span class="sxs-lookup"><span data-stu-id="108f4-185">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="108f4-186">要求本文</span><span class="sxs-lookup"><span data-stu-id="108f4-186">Request body</span></span>

<span data-ttu-id="108f4-187">リソース インスタンスの **singleValueExtendedProperties** コレクション プロパティに、各 [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) オブジェクトの JSON 本文を指定します。</span><span class="sxs-lookup"><span data-stu-id="108f4-187">Provide a JSON body of each [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object in the **singleValueExtendedProperties** collection property of the resource instance.</span></span>

|<span data-ttu-id="108f4-188">**プロパティ**</span><span class="sxs-lookup"><span data-stu-id="108f4-188">**Property**</span></span>|<span data-ttu-id="108f4-189">**型**</span><span class="sxs-lookup"><span data-stu-id="108f4-189">**Type**</span></span>|<span data-ttu-id="108f4-190">**説明**</span><span class="sxs-lookup"><span data-stu-id="108f4-190">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="108f4-191">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="108f4-191">singleValueExtendedProperties</span></span>|<span data-ttu-id="108f4-192">[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="108f4-192">[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="108f4-193">1 つ以上の単一値を持つ拡張プロパティの配列。</span><span class="sxs-lookup"><span data-stu-id="108f4-193">An array of one or more single-valued extended properties.</span></span> |
|<span data-ttu-id="108f4-194">id</span><span class="sxs-lookup"><span data-stu-id="108f4-194">id</span></span>|<span data-ttu-id="108f4-195">String</span><span class="sxs-lookup"><span data-stu-id="108f4-195">String</span></span>|<span data-ttu-id="108f4-p104">**singleValueExtendedProperties** コレクションの各プロパティに対して、これを指定することでプロパティを特定します。サポートされている形式のいずれかに従う必要があります。詳しくは、「[Outlook の拡張プロパティの概要](../resources/extended-properties-overview.md)」を参照してください。必須。</span><span class="sxs-lookup"><span data-stu-id="108f4-p104">For each property in the **singleValueExtendedProperties** collection, specify this to identify the property. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|
|<span data-ttu-id="108f4-200">value</span><span class="sxs-lookup"><span data-stu-id="108f4-200">value</span></span>|<span data-ttu-id="108f4-201">string</span><span class="sxs-lookup"><span data-stu-id="108f4-201">string</span></span>|<span data-ttu-id="108f4-p105">**singleValueExtendedProperties** コレクションの各プロパティについて、プロパティの値を特定します。必須。</span><span class="sxs-lookup"><span data-stu-id="108f4-p105">For each property in the **singleValueExtendedProperties** collection, specify the property value. Required.</span></span>|

<span data-ttu-id="108f4-204">_新しい_リソース インスタンスに拡張プロパティを作成する場合は、新しい **singleValueExtendedProperties**コレクションのほか、そのリソース インスタンスの JSON 表現を指定します ([message](../resources/message.md)、[mailFolder](../resources/mailfolder.md)、[event](../resources/event.md) など)。</span><span class="sxs-lookup"><span data-stu-id="108f4-204">When creating an extended property in a _new_ resource instance, in addition to the new **singleValueExtendedProperties** collection, provide a JSON representation of that resource instance (that is, a [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), etc.)</span></span>

## <a name="response"></a><span data-ttu-id="108f4-205">応答</span><span class="sxs-lookup"><span data-stu-id="108f4-205">Response</span></span>

#### <a name="response-code"></a><span data-ttu-id="108f4-206">応答コード</span><span class="sxs-lookup"><span data-stu-id="108f4-206">Response code</span></span>
<span data-ttu-id="108f4-207">新しいリソース インスタンスに拡張プロパティが正常に作成されると、`201 Created` が返されます。ただし新しいグループ投稿の場合は別で、使用するメソッドに応じて、`200 OK` または `202 Accepted` が返されます。</span><span class="sxs-lookup"><span data-stu-id="108f4-207">An operation successful in creating an extended property in a new resource instance returns `201 Created`, except in a new group post, depending on the method used, the operation can return `200 OK` or `202 Accepted`.</span></span>

<span data-ttu-id="108f4-208">既存のリソース インスタンスに拡張プロパティが正常に作成されると、`200 OK` が返されます。</span><span class="sxs-lookup"><span data-stu-id="108f4-208">In an existing resource instance, a successful create operation returns `200 OK`.</span></span> 


#### <a name="response-body"></a><span data-ttu-id="108f4-209">応答本文</span><span class="sxs-lookup"><span data-stu-id="108f4-209">Response body</span></span>

<span data-ttu-id="108f4-p106">拡張プロパティを作成する場合、応答には新規または既存のインスタンスのみを含めて、新しい拡張プロパティは含めません。新しく作成された拡張プロパティを表示するには、[拡張プロパティを使用して展開されているインスタンスを取得](../api/singlevaluelegacyextendedproperty-get.md)します。</span><span class="sxs-lookup"><span data-stu-id="108f4-p106">When creating an extended property, the response includes only the new or existing instance but not the new extended property. To see the newly created extended property, [get the instance expanded with the extended property](../api/singlevaluelegacyextendedproperty-get.md).</span></span>

<span data-ttu-id="108f4-212">スレッドまたは投稿に返信することで、_新しい_[グループ投稿](../resources/post.md)に拡張プロパティを作成する場合、応答には応答コードのみを含めて、新しい投稿や拡張プロパティは含めません。</span><span class="sxs-lookup"><span data-stu-id="108f4-212">When creating an extended property in a _new_ [group post](../resources/post.md) by replying to a thread or post, the response includes only a response code but not the new post nor the extended property.</span></span>



## <a name="example"></a><span data-ttu-id="108f4-213">例</span><span class="sxs-lookup"><span data-stu-id="108f4-213">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="108f4-214">要求 1</span><span class="sxs-lookup"><span data-stu-id="108f4-214">Request 1</span></span>

<span data-ttu-id="108f4-p107">最初の例では、同じ POST 操作で新しいイベントと単一値の拡張プロパティを作成します。新しいイベントに通常含めるプロパティとは別に、1 つの単一値の拡張プロパティを含む **singleValueExtendedProperties** コレクションを要求の本文に含め、そのプロパティは次のようにします。</span><span class="sxs-lookup"><span data-stu-id="108f4-p107">The first example creates a new event and a single-value extended property in the same POST operation. Apart from the properties you'd normally include for a new event, the request body includes the **singleValueExtendedProperties** collection that contains one single-value extended property, and the following for the property:</span></span>

- <span data-ttu-id="108f4-217">**id** は、プロパティの型を `String` (GUID) として指定し、`Fun` という名前のプロパティとして指定します。</span><span class="sxs-lookup"><span data-stu-id="108f4-217">**id** specifies the property type as `String`, the GUID, and the property named `Fun`.</span></span>
- <span data-ttu-id="108f4-218">**value** は、`Fun` プロパティの値として `Food` を指定します。</span><span class="sxs-lookup"><span data-stu-id="108f4-218">**value** specifies `Food` as the value of the `Fun` property.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/me/events
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

##### <a name="response-1"></a><span data-ttu-id="108f4-219">応答 1</span><span class="sxs-lookup"><span data-stu-id="108f4-219">Response 1</span></span>

<span data-ttu-id="108f4-p108">[イベントのみの作成](../api/user-post-events.md)からの応答と同様に、`HTTP 201 Created` 応答コードによって正常な応答が示され、応答の本文に新しいイベントが含まれます。応答には、新しく作成された拡張プロパティは含まれません。</span><span class="sxs-lookup"><span data-stu-id="108f4-p108">A successful response is indicated by an `HTTP 201 Created` response code, and includes the new event in the response body, similar to the response from [creating just an event](../api/user-post-events.md). The response does not include any newly created extended properties.</span></span>

<span data-ttu-id="108f4-222">新しく作成された拡張プロパティを表示するには、[拡張プロパティを使用して展開されているイベントを取得](../api/singlevaluelegacyextendedproperty-get.md)します。</span><span class="sxs-lookup"><span data-stu-id="108f4-222">To see the newly created extended property, [get the event expanded with the extended property](../api/singlevaluelegacyextendedproperty-get.md).</span></span>


****

##### <a name="request-2"></a><span data-ttu-id="108f4-223">要求 2</span><span class="sxs-lookup"><span data-stu-id="108f4-223">Request 2</span></span>

<span data-ttu-id="108f4-p109">2 番目の例では、指定した既存のメッセージに 1 つの単一値の拡張プロパティを作成します。拡張プロパティは、**singleValueExtendedProperties** 配列内の唯一の要素です。要求本文には、拡張プロパティに関する次のものが含まれています。</span><span class="sxs-lookup"><span data-stu-id="108f4-p109">The second example creates one single-value extended property for the specified existing message. That extended property is the only element in the **singleValueExtendedProperties** array. The request body includes the following for the extended property:</span></span>
- <span data-ttu-id="108f4-227">**id** は、プロパティの型を `String` (GUID) として指定し、`Color` という名前のプロパティとして指定します。</span><span class="sxs-lookup"><span data-stu-id="108f4-227">**id** specifies the property type as `String`, the GUID, and the property named `Color`.</span></span>
- <span data-ttu-id="108f4-228">**value** は、`Color` プロパティの値として `Green` を指定します。</span><span class="sxs-lookup"><span data-stu-id="108f4-228">**value** specifies `Green` as the value of the `Color` property.</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/beta/me/messages('AAMkAGE1M2_bs88AACHsLqWAAA=')

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

##### <a name="response-2"></a><span data-ttu-id="108f4-229">応答 2</span><span class="sxs-lookup"><span data-stu-id="108f4-229">Response 2</span></span>

<span data-ttu-id="108f4-p110">[メッセージの更新](../api/message-update.md)からの応答と同様に、`HTTP 200 OK` 応答コードによって正常な応答が示され、応答の本文に指定したメッセージが含まれています。応答には、新しく作成された拡張プロパティは含まれません。</span><span class="sxs-lookup"><span data-stu-id="108f4-p110">A successful response is indicated by an `HTTP 200 OK` response code, and includes the specified message in the response body, similar to the response from [updating a message](../api/message-update.md). The response does not include the newly created extended property.</span></span>

<span data-ttu-id="108f4-232">新しく作成された拡張プロパティを表示するには、[拡張プロパティを使用して展開されているメッセージを取得](../api/singlevaluelegacyextendedproperty-get.md)します。</span><span class="sxs-lookup"><span data-stu-id="108f4-232">To see the newly created extended property, [get the message expanded with the extended property](../api/singlevaluelegacyextendedproperty-get.md).</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

