---
title: multiValueLegacyExtendedProperty を取得する
description: 展開 ' です。
ms.openlocfilehash: 9429737f3965acbf4c6bcc61c516327556223111
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071522"
---
# <a name="get-multivaluelegacyextendedproperty"></a><span data-ttu-id="13021-103">multiValueLegacyExtendedProperty を取得する</span><span class="sxs-lookup"><span data-stu-id="13021-103">Get multiValueLegacyExtendedProperty</span></span>

> <span data-ttu-id="13021-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="13021-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="13021-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="13021-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="13021-106">`$expand` を使用して、複数値の拡張プロパティを含むリソース インスタンスを取得します。</span><span class="sxs-lookup"><span data-stu-id="13021-106">Get a resource instance that contains a multi-value extended property by using `$expand`.</span></span>

<span data-ttu-id="13021-107">クエリ パラメーター `$expand` を使用すると、指示された拡張プロパティで展開された特定のインスタンスを取得できます。</span><span class="sxs-lookup"><span data-stu-id="13021-107">Using the query parameter `$expand` allows you to get the specified instance expanded with the indicated extended property.</span></span> <span data-ttu-id="13021-108">これは、現時点で、拡張プロパティを表す [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) オブジェクトを取得する唯一の方法です。</span><span class="sxs-lookup"><span data-stu-id="13021-108">This is currently the only way to get the [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object that represents an extended property.</span></span>

<span data-ttu-id="13021-109">次のユーザー リソースがサポートされます。</span><span class="sxs-lookup"><span data-stu-id="13021-109">The following user resources are supported:</span></span>

- [<span data-ttu-id="13021-110">calendar</span><span class="sxs-lookup"><span data-stu-id="13021-110">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="13021-111">contact</span><span class="sxs-lookup"><span data-stu-id="13021-111">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="13021-112">contactFolder</span><span class="sxs-lookup"><span data-stu-id="13021-112">contactFolder</span></span>](../resources/contactfolder.md) 
- [<span data-ttu-id="13021-113">イベント</span><span class="sxs-lookup"><span data-stu-id="13021-113">event</span></span>](../resources/event.md)
- [<span data-ttu-id="13021-114">mailFolder</span><span class="sxs-lookup"><span data-stu-id="13021-114">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="13021-115">message</span><span class="sxs-lookup"><span data-stu-id="13021-115">message</span></span>](../resources/message.md) 
- [<span data-ttu-id="13021-116">Outlook タスク</span><span class="sxs-lookup"><span data-stu-id="13021-116">Outlook task</span></span>](../resources/outlooktask.md)
- [<span data-ttu-id="13021-117">Outlook の仕事フォルダー</span><span class="sxs-lookup"><span data-stu-id="13021-117">Outlook task folder</span></span>](../resources/outlooktaskfolder.md)

<span data-ttu-id="13021-118">次のグループ リソースもサポートされます。</span><span class="sxs-lookup"><span data-stu-id="13021-118">As well as the following group resources:</span></span>

- <span data-ttu-id="13021-119">グループ [calendar](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="13021-119">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="13021-120">グループ [event](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="13021-120">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="13021-121">グループ [post](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="13021-121">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="13021-122">オープン拡張機能または拡張プロパティを使用するのに適した状況と、拡張プロパティを指定する方法の詳細については、「[拡張プロパティの概要](../resources/extended-properties-overview.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="13021-122">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="13021-123">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="13021-123">Permissions</span></span>
<span data-ttu-id="13021-124">拡張プロパティを受信するリソースに応じて、アクセス許可が委任された (アプリケーション) を要求を入力する、次の表で指定されたアクセス許可は、この API を呼び出すために必要最低限。</span><span class="sxs-lookup"><span data-stu-id="13021-124">Depending on the resource you're getting the extended property from and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="13021-125">アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="13021-125">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="13021-126">サポートされているリソース</span><span class="sxs-lookup"><span data-stu-id="13021-126">Supported resource</span></span> | <span data-ttu-id="13021-127">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="13021-127">Delegated (work or school account)</span></span> | <span data-ttu-id="13021-128">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="13021-128">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="13021-129">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="13021-129">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="13021-130">calendar</span><span class="sxs-lookup"><span data-stu-id="13021-130">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="13021-131">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="13021-131">Calendars.Read</span></span> | <span data-ttu-id="13021-132">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="13021-132">Calendars.Read</span></span> | <span data-ttu-id="13021-133">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="13021-133">Calendars.Read</span></span> |
| [<span data-ttu-id="13021-134">連絡先</span><span class="sxs-lookup"><span data-stu-id="13021-134">contact</span></span>](../resources/contact.md) | <span data-ttu-id="13021-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="13021-135">Contacts.Read</span></span> | <span data-ttu-id="13021-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="13021-136">Contacts.Read</span></span> | <span data-ttu-id="13021-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="13021-137">Contacts.Read</span></span> |
| [<span data-ttu-id="13021-138">contactFolder</span><span class="sxs-lookup"><span data-stu-id="13021-138">contactFolder</span></span>](../resources/contactfolder.md) | <span data-ttu-id="13021-139">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="13021-139">Contacts.Read</span></span> | <span data-ttu-id="13021-140">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="13021-140">Contacts.Read</span></span> | <span data-ttu-id="13021-141">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="13021-141">Contacts.Read</span></span> |
| [<span data-ttu-id="13021-142">イベント</span><span class="sxs-lookup"><span data-stu-id="13021-142">event</span></span>](../resources/event.md) | <span data-ttu-id="13021-143">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="13021-143">Calendars.Read</span></span> | <span data-ttu-id="13021-144">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="13021-144">Calendars.Read</span></span> |  <span data-ttu-id="13021-145">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="13021-145">Calendars.Read</span></span>|
| <span data-ttu-id="13021-146">グループ [calendar](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="13021-146">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="13021-147">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="13021-147">Group.Read.All</span></span> | <span data-ttu-id="13021-148">使用不可</span><span class="sxs-lookup"><span data-stu-id="13021-148">Not supported</span></span> | <span data-ttu-id="13021-149">使用不可</span><span class="sxs-lookup"><span data-stu-id="13021-149">Not supported</span></span> |
| <span data-ttu-id="13021-150">グループ [event](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="13021-150">group [event](../resources/event.md)</span></span> | <span data-ttu-id="13021-151">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="13021-151">Group.Read.All</span></span> | <span data-ttu-id="13021-152">使用不可</span><span class="sxs-lookup"><span data-stu-id="13021-152">Not supported</span></span> | <span data-ttu-id="13021-153">使用不可</span><span class="sxs-lookup"><span data-stu-id="13021-153">Not supported</span></span> |
| <span data-ttu-id="13021-154">グループ [post](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="13021-154">group [post](../resources/post.md)</span></span> | <span data-ttu-id="13021-155">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="13021-155">Group.Read.All</span></span> | <span data-ttu-id="13021-156">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="13021-156">Not supported</span></span> | <span data-ttu-id="13021-157">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="13021-157">Group.Read.All</span></span> |
| [<span data-ttu-id="13021-158">mailFolder</span><span class="sxs-lookup"><span data-stu-id="13021-158">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="13021-159">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="13021-159">Mail.Read</span></span> | <span data-ttu-id="13021-160">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="13021-160">Mail.Read</span></span> | <span data-ttu-id="13021-161">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="13021-161">Mail.Read</span></span> |
| [<span data-ttu-id="13021-162">message</span><span class="sxs-lookup"><span data-stu-id="13021-162">message</span></span>](../resources/message.md) | <span data-ttu-id="13021-163">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="13021-163">Mail.Read</span></span> | <span data-ttu-id="13021-164">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="13021-164">Mail.Read</span></span> | <span data-ttu-id="13021-165">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="13021-165">Mail.Read</span></span> |
| [<span data-ttu-id="13021-166">Outlook タスク</span><span class="sxs-lookup"><span data-stu-id="13021-166">Outlook task</span></span>](../resources/outlooktask.md) | <span data-ttu-id="13021-167">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="13021-167">Tasks.Read</span></span> | <span data-ttu-id="13021-168">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="13021-168">Tasks.Read</span></span> | <span data-ttu-id="13021-169">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="13021-169">Not supported</span></span> |
| [<span data-ttu-id="13021-170">Outlook の仕事フォルダー</span><span class="sxs-lookup"><span data-stu-id="13021-170">Outlook task folder</span></span>](../resources/outlooktaskfolder.md) | <span data-ttu-id="13021-171">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="13021-171">Tasks.Read</span></span> | <span data-ttu-id="13021-172">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="13021-172">Tasks.Read</span></span> | <span data-ttu-id="13021-173">非サポート</span><span class="sxs-lookup"><span data-stu-id="13021-173">Not supported</span></span> |
 
## <a name="http-request"></a><span data-ttu-id="13021-174">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="13021-174">HTTP request</span></span>

<span data-ttu-id="13021-p104">**id** プロパティに対するフィルターと一致する拡張プロパティで展開された、リソース インスタンスを取得します。フィルター文字列内のスペース文字に [URL エンコード](https://www.w3schools.com/tags/ref_urlencode.asp)を適用していることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="13021-p104">Get a resource instance expanded with the extended property which matches a filter on the **id** property. Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the filter string.</span></span>

<span data-ttu-id="13021-177">**メッセージ**インスタンスを取得します。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="13021-177">Get a **message** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="13021-178">**MailFolder**のインスタンスを取得します。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="13021-178">Get a **mailFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/mailFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="13021-179">**イベント**インスタンスを取得します。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="13021-179">Get an **event** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="13021-180">**カレンダー**のインスタンスを取得します。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="13021-180">Get a **calendar** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/calendars/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="13021-181">**連絡**のインスタンスを取得します。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="13021-181">Get a **contact** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="13021-182">**ContactFolder**のインスタンスを取得します。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="13021-182">Get a **contactFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/contactfolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="13021-183">**OutlookTask**インスタンスを取得します。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="13021-183">Get an **outlookTask** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/outlook/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskFolders/{id}/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="13021-184">**OutlookTaskFolder**インスタンスを取得します。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="13021-184">Get an **outlookTaskFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/outlook/taskFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskGroups/{id}/taskFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="13021-185">グループ**イベント**のインスタンスを取得します。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="13021-185">Get a group **event** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="13021-186">グループの**投稿**のインスタンスを取得します。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="13021-186">Get a group **post** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

## <a name="path-parameters"></a><span data-ttu-id="13021-187">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="13021-187">Path parameters</span></span>
|<span data-ttu-id="13021-188">**パラメーター**</span><span class="sxs-lookup"><span data-stu-id="13021-188">**Parameter**</span></span>|<span data-ttu-id="13021-189">**型**</span><span class="sxs-lookup"><span data-stu-id="13021-189">**Type**</span></span>|<span data-ttu-id="13021-190">**説明**</span><span class="sxs-lookup"><span data-stu-id="13021-190">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="13021-191">id_value</span><span class="sxs-lookup"><span data-stu-id="13021-191">id_value</span></span>|<span data-ttu-id="13021-192">String</span><span class="sxs-lookup"><span data-stu-id="13021-192">String</span></span>|<span data-ttu-id="13021-p105">照合する拡張プロパティの ID。サポートされている形式のいずれかに従う必要があります。詳しくは、「[Outlook の拡張プロパティの概要](../resources/extended-properties-overview.md)」を参照してください。必須。</span><span class="sxs-lookup"><span data-stu-id="13021-p105">The ID of the extended property to match. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="13021-197">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="13021-197">Request headers</span></span>
| <span data-ttu-id="13021-198">名前</span><span class="sxs-lookup"><span data-stu-id="13021-198">Name</span></span>      |<span data-ttu-id="13021-199">説明</span><span class="sxs-lookup"><span data-stu-id="13021-199">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="13021-200">Authorization</span><span class="sxs-lookup"><span data-stu-id="13021-200">Authorization</span></span>  | <span data-ttu-id="13021-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="13021-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="13021-203">要求本文</span><span class="sxs-lookup"><span data-stu-id="13021-203">Request body</span></span>
<span data-ttu-id="13021-204">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="13021-204">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="13021-205">応答</span><span class="sxs-lookup"><span data-stu-id="13021-205">Response</span></span>

<span data-ttu-id="13021-206">成功した場合、このメソッドは `200 OK` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="13021-206">If successful, this method returns a `200 OK` response code.</span></span> 

<span data-ttu-id="13021-207">応答本文には、一致する [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) オブジェクトで展開された、要求したリソース インスタンスで表されるオブジェクトが含まれます。</span><span class="sxs-lookup"><span data-stu-id="13021-207">The response body includes an object representing the requested resource instance, expanded with the matching [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object.</span></span>

## <a name="example"></a><span data-ttu-id="13021-208">例</span><span class="sxs-lookup"><span data-stu-id="13021-208">Example</span></span>
##### <a name="request"></a><span data-ttu-id="13021-209">要求</span><span class="sxs-lookup"><span data-stu-id="13021-209">Request</span></span>
<span data-ttu-id="13021-p107">この例では、複数値の拡張プロパティを含めることで指定されたイベントを取得して展開します。フィルターは、**id** が文字列 `StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation` と一致する拡張プロパティを返します (ここでは、読みやすくするため URL エンコードを削除しています)。</span><span class="sxs-lookup"><span data-stu-id="13021-p107">This example gets and expands the specified event by including a multi-value extended property. The filter returns the extended property that has its **id** matching the string `StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation` (with URL encoding removed here for ease of reading).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/events('AAMkAGE1M2_bs88AACbuFiiAAA=')?$expand=multiValueExtendedProperties($filter=id%20eq%20'StringArray%20{66f5a359-4659-4830-9070-00050ec6ac6e}%20Name%20Recreation')
```
##### <a name="response"></a><span data-ttu-id="13021-212">応答</span><span class="sxs-lookup"><span data-stu-id="13021-212">Response</span></span>

<span data-ttu-id="13021-213">応答本文には、指定されたイベントのすべてのプロパティと、フィルターから返される拡張プロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="13021-213">The response body includes all the properties of the specified event and extended property returned from the filter.</span></span>

<span data-ttu-id="13021-p108">注:簡潔にするために、ここに示す**イベント** オブジェクトは切り詰められています。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="13021-p108">Note: The **event** object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/events/$entity",
    "@odata.id": "https://graph.microsoft.com/beta/users('ddfcd489-628b-40d7-b48b-57002df800e5@1717622f-1d94-4d0c-9d74-709fad664b77')/events('AAMkAGE1M2_bs88AACbuFiiAAA=')",
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
    "multiValueExtendedProperties@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/events('AAMkAGE1M2_bs88AACbuFiiAAA%3D')/multiValueExtendedProperties",
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