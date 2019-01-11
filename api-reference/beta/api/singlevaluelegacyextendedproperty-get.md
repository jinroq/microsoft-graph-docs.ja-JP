---
title: singleValueLegacyExtendedProperty を取得する
description: 特定の拡張プロパティ、またはリソースのインスタンスのコレクションに展開されている 1 つのリソースのインスタンスを取得します。
localization_priority: Normal
ms.openlocfilehash: ee9d51f945650c8051badd27f1b934d03f47cc7b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27873186"
---
# <a name="get-singlevaluelegacyextendedproperty"></a><span data-ttu-id="441ee-103">singleValueLegacyExtendedProperty を取得する</span><span class="sxs-lookup"><span data-stu-id="441ee-103">Get singleValueLegacyExtendedProperty</span></span>

> <span data-ttu-id="441ee-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="441ee-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="441ee-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="441ee-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="441ee-106">特定の拡張プロパティで展開された単一のリソース インスタンス、または 1 つのフィルターと一致する拡張プロパティを含むリソース インスタンスのコレクションを取得できます。</span><span class="sxs-lookup"><span data-stu-id="441ee-106">You can get a single resource instance expanded with a specific extended property, or a collection of resource instances that include extended properties matching a filter.</span></span>

<span data-ttu-id="441ee-107">クエリ パラメーター `$expand` を使用すると、指定した拡張プロパティで展開された特定のリソース インスタンスを取得できます。</span><span class="sxs-lookup"><span data-stu-id="441ee-107">Using the query parameter `$expand` allows you to get the specified resource instance expanded with a specific extended property.</span></span> <span data-ttu-id="441ee-108">**id** プロパティ上で `$filter` および `eq` 演算子を使用して拡張プロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="441ee-108">Use a `$filter` and `eq` operator on the **id** property to specify the extended property.</span></span> <span data-ttu-id="441ee-109">これは、現時点で、拡張プロパティを表す [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) オブジェクトを取得する唯一の方法です。</span><span class="sxs-lookup"><span data-stu-id="441ee-109">This is currently the only way to get the [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object that represents an extended property.</span></span> 

<span data-ttu-id="441ee-110">特定の拡張プロパティを含むリソース インスタンスを取得するには、`$filter` クエリ パラメーターを使用して、`eq` 演算子を **id** プロパティに適用します。</span><span class="sxs-lookup"><span data-stu-id="441ee-110">To get resource instances that have certain extended properties, use the `$filter` query parameter and apply an `eq` operator on the **id** property.</span></span> <span data-ttu-id="441ee-111">さらに、数値の拡張プロパティについては、**value** プロパティで `eq`、`ne`、`ge`、`gt`、`le`、`lt` 演算子のいずれかを適用します。</span><span class="sxs-lookup"><span data-stu-id="441ee-111">In addition, for numeric extended properties, apply one of the following operators on the **value** property: `eq`, `ne`,`ge`, `gt`, `le`, or `lt`.</span></span> <span data-ttu-id="441ee-112">文字列型の拡張プロパティについては、`contains`、`startswith`、`eq`、`ne` 演算子を **value** に適用します。</span><span class="sxs-lookup"><span data-stu-id="441ee-112">For string-typed extended properties, apply a `contains`, `startswith`, `eq`, or `ne` operator on **value**.</span></span> 

<span data-ttu-id="441ee-113">拡張プロパティの **id** で文字列名 (`Name`) をフィルタリングする場合は、大文字と小文字が区別されます。</span><span class="sxs-lookup"><span data-stu-id="441ee-113">Filtering the string name (`Name`) in the **id** of an extended property is case-sensitive.</span></span> <span data-ttu-id="441ee-114">拡張プロパティの **value** プロパティをフィルタリングする場合は、大文字と小文字が区別されません。</span><span class="sxs-lookup"><span data-stu-id="441ee-114">Filtering the **value** property of an extended property is case-insensitive.</span></span>

<span data-ttu-id="441ee-115">次のユーザー リソースがサポートされます。</span><span class="sxs-lookup"><span data-stu-id="441ee-115">The following user resources are supported:</span></span>

- [<span data-ttu-id="441ee-116">calendar</span><span class="sxs-lookup"><span data-stu-id="441ee-116">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="441ee-117">contact</span><span class="sxs-lookup"><span data-stu-id="441ee-117">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="441ee-118">contactFolder</span><span class="sxs-lookup"><span data-stu-id="441ee-118">contactFolder</span></span>](../resources/contactfolder.md) 
- [<span data-ttu-id="441ee-119">イベント</span><span class="sxs-lookup"><span data-stu-id="441ee-119">event</span></span>](../resources/event.md)
- [<span data-ttu-id="441ee-120">mailFolder</span><span class="sxs-lookup"><span data-stu-id="441ee-120">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="441ee-121">message</span><span class="sxs-lookup"><span data-stu-id="441ee-121">message</span></span>](../resources/message.md) 
- [<span data-ttu-id="441ee-122">Outlook タスク</span><span class="sxs-lookup"><span data-stu-id="441ee-122">Outlook task</span></span>](../resources/outlooktask.md)
- [<span data-ttu-id="441ee-123">Outlook の仕事フォルダー</span><span class="sxs-lookup"><span data-stu-id="441ee-123">Outlook task folder</span></span>](../resources/outlooktaskfolder.md)

<span data-ttu-id="441ee-124">次のグループ リソースもサポートされます。</span><span class="sxs-lookup"><span data-stu-id="441ee-124">As well as the following group resources:</span></span>

- <span data-ttu-id="441ee-125">グループ [calendar](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="441ee-125">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="441ee-126">グループ [event](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="441ee-126">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="441ee-127">グループ [post](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="441ee-127">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="441ee-128">オープン拡張機能または拡張プロパティを使用するのに適した状況と、拡張プロパティを指定する方法の詳細については、「[拡張プロパティの概要](../resources/extended-properties-overview.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="441ee-128">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="441ee-129">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="441ee-129">Permissions</span></span>
<span data-ttu-id="441ee-130">拡張プロパティを受信するリソースに応じて、アクセス許可が委任された (アプリケーション) を要求を入力する、次の表で指定されたアクセス許可は、この API を呼び出すために必要最低限。</span><span class="sxs-lookup"><span data-stu-id="441ee-130">Depending on the resource you're getting the extended property from and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="441ee-131">アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="441ee-131">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="441ee-132">サポートされているリソース</span><span class="sxs-lookup"><span data-stu-id="441ee-132">Supported resource</span></span> | <span data-ttu-id="441ee-133">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="441ee-133">Delegated (work or school account)</span></span> | <span data-ttu-id="441ee-134">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="441ee-134">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="441ee-135">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="441ee-135">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="441ee-136">calendar</span><span class="sxs-lookup"><span data-stu-id="441ee-136">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="441ee-137">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="441ee-137">Calendars.Read</span></span> | <span data-ttu-id="441ee-138">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="441ee-138">Calendars.Read</span></span> | <span data-ttu-id="441ee-139">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="441ee-139">Calendars.Read</span></span> |
| [<span data-ttu-id="441ee-140">連絡先</span><span class="sxs-lookup"><span data-stu-id="441ee-140">contact</span></span>](../resources/contact.md) | <span data-ttu-id="441ee-141">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="441ee-141">Contacts.Read</span></span> | <span data-ttu-id="441ee-142">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="441ee-142">Contacts.Read</span></span> | <span data-ttu-id="441ee-143">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="441ee-143">Contacts.Read</span></span> |
| [<span data-ttu-id="441ee-144">contactFolder</span><span class="sxs-lookup"><span data-stu-id="441ee-144">contactFolder</span></span>](../resources/contactfolder.md) | <span data-ttu-id="441ee-145">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="441ee-145">Contacts.Read</span></span> | <span data-ttu-id="441ee-146">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="441ee-146">Contacts.Read</span></span> | <span data-ttu-id="441ee-147">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="441ee-147">Contacts.Read</span></span> |
| [<span data-ttu-id="441ee-148">イベント</span><span class="sxs-lookup"><span data-stu-id="441ee-148">event</span></span>](../resources/event.md) | <span data-ttu-id="441ee-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="441ee-149">Calendars.Read</span></span> | <span data-ttu-id="441ee-150">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="441ee-150">Calendars.Read</span></span> |  <span data-ttu-id="441ee-151">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="441ee-151">Calendars.Read</span></span>|
| <span data-ttu-id="441ee-152">グループ [calendar](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="441ee-152">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="441ee-153">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="441ee-153">Group.Read.All</span></span> | <span data-ttu-id="441ee-154">使用不可</span><span class="sxs-lookup"><span data-stu-id="441ee-154">Not supported</span></span> | <span data-ttu-id="441ee-155">使用不可</span><span class="sxs-lookup"><span data-stu-id="441ee-155">Not supported</span></span> |
| <span data-ttu-id="441ee-156">グループ [event](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="441ee-156">group [event](../resources/event.md)</span></span> | <span data-ttu-id="441ee-157">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="441ee-157">Group.Read.All</span></span> | <span data-ttu-id="441ee-158">使用不可</span><span class="sxs-lookup"><span data-stu-id="441ee-158">Not supported</span></span> | <span data-ttu-id="441ee-159">使用不可</span><span class="sxs-lookup"><span data-stu-id="441ee-159">Not supported</span></span> |
| <span data-ttu-id="441ee-160">グループ [post](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="441ee-160">group [post](../resources/post.md)</span></span> | <span data-ttu-id="441ee-161">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="441ee-161">Group.Read.All</span></span> | <span data-ttu-id="441ee-162">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="441ee-162">Not supported</span></span> | <span data-ttu-id="441ee-163">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="441ee-163">Group.Read.All</span></span> |
| [<span data-ttu-id="441ee-164">mailFolder</span><span class="sxs-lookup"><span data-stu-id="441ee-164">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="441ee-165">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="441ee-165">Mail.Read</span></span> | <span data-ttu-id="441ee-166">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="441ee-166">Mail.Read</span></span> | <span data-ttu-id="441ee-167">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="441ee-167">Mail.Read</span></span> |
| [<span data-ttu-id="441ee-168">message</span><span class="sxs-lookup"><span data-stu-id="441ee-168">message</span></span>](../resources/message.md) | <span data-ttu-id="441ee-169">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="441ee-169">Mail.Read</span></span> | <span data-ttu-id="441ee-170">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="441ee-170">Mail.Read</span></span> | <span data-ttu-id="441ee-171">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="441ee-171">Mail.Read</span></span> |
| [<span data-ttu-id="441ee-172">Outlook タスク</span><span class="sxs-lookup"><span data-stu-id="441ee-172">Outlook task</span></span>](../resources/outlooktask.md) | <span data-ttu-id="441ee-173">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="441ee-173">Tasks.Read</span></span> | <span data-ttu-id="441ee-174">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="441ee-174">Tasks.Read</span></span> | <span data-ttu-id="441ee-175">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="441ee-175">Not supported</span></span> |
| [<span data-ttu-id="441ee-176">Outlook の仕事フォルダー</span><span class="sxs-lookup"><span data-stu-id="441ee-176">Outlook task folder</span></span>](../resources/outlooktaskfolder.md) | <span data-ttu-id="441ee-177">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="441ee-177">Tasks.Read</span></span> | <span data-ttu-id="441ee-178">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="441ee-178">Tasks.Read</span></span> | <span data-ttu-id="441ee-179">非サポート</span><span class="sxs-lookup"><span data-stu-id="441ee-179">Not supported</span></span> |


## <a name="http-request"></a><span data-ttu-id="441ee-180">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="441ee-180">HTTP request</span></span>

#### <a name="get-a-resource-instance-expanded-with-an-extended-property-that-matches-a-filter"></a><span data-ttu-id="441ee-181">フィルターと一致する拡張プロパティで展開されたリソース インスタンスを取得する</span><span class="sxs-lookup"><span data-stu-id="441ee-181">GET a resource instance expanded with an extended property that matches a filter</span></span>
<span data-ttu-id="441ee-p106">**id** プロパティに対するフィルターと一致する拡張プロパティで展開された、リソース インスタンスを取得します。フィルター文字列内のスペース文字に [URL エンコード](https://www.w3schools.com/tags/ref_urlencode.asp)を適用していることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="441ee-p106">Get a resource instance expanded with the extended property which matches a filter on the **id** property. Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the filter string.</span></span>

<span data-ttu-id="441ee-184">**メッセージ**インスタンスを取得します。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="441ee-184">Get a **message** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="441ee-185">**MailFolder**のインスタンスを取得します。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="441ee-185">Get a **mailFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="441ee-186">**イベント**インスタンスを取得します。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="441ee-186">Get an **event** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="441ee-187">**カレンダー**のインスタンスを取得します。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="441ee-187">Get a **calendar** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="441ee-188">**連絡**のインスタンスを取得します。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="441ee-188">Get a **contact** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="441ee-189">**ContactFolder**のインスタンスを取得します。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="441ee-189">Get a **contactFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/contactfolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="441ee-190">**OutlookTask**インスタンスを取得します。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="441ee-190">Get an **outlookTask** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/outlook/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskFolders/{id}/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="441ee-191">**OutlookTaskFolder**インスタンスを取得します。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="441ee-191">Get an **outlookTaskFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/outlook/taskFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskGroups/{id}/taskFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="441ee-192">グループ**イベント**のインスタンスを取得します。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="441ee-192">Get a group **event** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="441ee-193">グループの**投稿**のインスタンスを取得します。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="441ee-193">Get a group **post** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

#### <a name="get-resource-instances-that-include-numeric-extended-properties-matching-a-filter"></a><span data-ttu-id="441ee-194">フィルターと一致する数値の拡張プロパティを含むリソース インスタンスを取得する</span><span class="sxs-lookup"><span data-stu-id="441ee-194">GET resource instances that include numeric extended properties matching a filter</span></span>

<span data-ttu-id="441ee-195">フィルターと一致する数値の拡張プロパティを持つサポート対象リソースのインスタンスを取得します。</span><span class="sxs-lookup"><span data-stu-id="441ee-195">Get instances of a supported resource that have a numeric extended property matching a filter.</span></span> <span data-ttu-id="441ee-196">フィルターは **id** プロパティには `eq` 演算子を使用し、**value** プロパティには `eq`、`ne`、`ge`、`gt`、`le`、`lt` のいずれかの演算子を使用します。</span><span class="sxs-lookup"><span data-stu-id="441ee-196">The filter uses an `eq` operator on the **id** property, and one of the following operators on the **value** property: `eq`, `ne`,`ge`, `gt`, `le`, or `lt`.</span></span> <span data-ttu-id="441ee-197">Make を適用するかどうかを確認確かに適用する[URL エンコード](https://www.w3schools.com/tags/ref_urlencode.asp)次の文字のフィルター文字列のコロン、スラッシュ、およびスペースです。</span><span class="sxs-lookup"><span data-stu-id="441ee-197">Make sure you apply Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the following characters in the filter string - colon, forward slash, and space.</span></span>

<span data-ttu-id="441ee-198">次の構文の行では、id に `eq` 演算子を使用し、プロパティ値にもう 1 つの `eq` 演算子を使用するフィルターを示しています。</span><span class="sxs-lookup"><span data-stu-id="441ee-198">The following syntax lines show a filter that uses an `eq` operator on the id, and another `eq` operator on the property value.</span></span> <span data-ttu-id="441ee-199">**value** に対する `eq` 演算子は、数値に適用される別の演算子 (`ne`、`ge`、`gt`、`le`、`lt`) のいずれかと置き換えることができます。</span><span class="sxs-lookup"><span data-stu-id="441ee-199">You can substitute the `eq` operator on the **value** by any one of the other operators (`ne`,`ge`, `gt`, `le`, or `lt`) that apply to numeric values.</span></span>

<span data-ttu-id="441ee-200">**メッセージ**インスタンスを取得します。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="441ee-200">Get **message** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="441ee-201">**MailFolder**のインスタンスを取得します。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="441ee-201">Get **mailFolder** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="441ee-202">**イベント**のインスタンスを取得します。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="441ee-202">Get **event** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="441ee-203">**予定表**のインスタンスを取得します。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="441ee-203">Get **calendar** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="441ee-204">**連絡**のインスタンスを取得します。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="441ee-204">Get **contact** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="441ee-205">**ContactFolder**のインスタンスを取得します。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="441ee-205">Get **contactFolder** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/contactfolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="441ee-206">**OutlookTask**インスタンスを取得します。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="441ee-206">Get an **outlookTask** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/outlook/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/outlook/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/outlook/taskFolders/{id}/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="441ee-207">**OutlookTaskFolder**インスタンスを取得します。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="441ee-207">Get an **outlookTaskFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/outlook/taskFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/outlook/taskGroups/{id}/taskFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="441ee-208">グループの**イベント**のインスタンスを取得します。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="441ee-208">Get group **event** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="441ee-209">グループの**投稿**のインスタンスを取得します。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="441ee-209">Get group **post** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

#### <a name="get-resource-instances-with-string-typed-extended-properties-matching-a-filter"></a><span data-ttu-id="441ee-210">フィルターと一致する文字列型の拡張プロパティを含むリソース インスタンスを取得する</span><span class="sxs-lookup"><span data-stu-id="441ee-210">GET resource instances with string-typed extended properties matching a filter</span></span>

<span data-ttu-id="441ee-211">フィルターと一致する文字列型の拡張プロパティを含む **message** または **event** リソースのインスタンスを取得します。</span><span class="sxs-lookup"><span data-stu-id="441ee-211">Get instances of the **message** or **event** resource that have a string-typed extended property matching a filter.</span></span> <span data-ttu-id="441ee-212">フィルターは **id** プロパティには `eq` 演算子を使用し、**value** プロパティには `contains`、`startswith`、`eq`、`ne` のいずれかの演算子を使用します。</span><span class="sxs-lookup"><span data-stu-id="441ee-212">The filter uses an `eq` operator on the **id** property, and one of the following operators on the **value** property: `contains`, `startswith`, `eq`, or `ne`.</span></span> <span data-ttu-id="441ee-213">フィルター文字列内のコロン、スラッシュ、スペースに [URL エンコード](https://www.w3schools.com/tags/ref_urlencode.asp)を適用していることをご確認ください。</span><span class="sxs-lookup"><span data-stu-id="441ee-213">Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the following characters in the filter string - colon, forward slash, and space.</span></span>


<span data-ttu-id="441ee-214">**メッセージ**インスタンスを取得します。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="441ee-214">Get **message** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))

GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))

GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')

GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
```

<span data-ttu-id="441ee-215">**イベント**のインスタンスを取得します。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="441ee-215">Get **event** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))

GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))

GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')

GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
```

<span data-ttu-id="441ee-216">グループの**イベント**のインスタンスを取得します。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="441ee-216">Get group **event** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
```

## <a name="path-parameters"></a><span data-ttu-id="441ee-217">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="441ee-217">Path parameters</span></span>
|<span data-ttu-id="441ee-218">**パラメーター**</span><span class="sxs-lookup"><span data-stu-id="441ee-218">**Parameter**</span></span>|<span data-ttu-id="441ee-219">**型**</span><span class="sxs-lookup"><span data-stu-id="441ee-219">**Type**</span></span>|<span data-ttu-id="441ee-220">**説明**</span><span class="sxs-lookup"><span data-stu-id="441ee-220">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="441ee-221">id_value</span><span class="sxs-lookup"><span data-stu-id="441ee-221">id_value</span></span>|<span data-ttu-id="441ee-222">String</span><span class="sxs-lookup"><span data-stu-id="441ee-222">String</span></span>|<span data-ttu-id="441ee-p110">照合する拡張プロパティの ID。サポートされている形式のいずれかに従う必要があります。詳しくは、「[Outlook の拡張プロパティの概要](../resources/extended-properties-overview.md)」を参照してください。必須。</span><span class="sxs-lookup"><span data-stu-id="441ee-p110">The ID of the extended property to match. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|
|<span data-ttu-id="441ee-227">property_value</span><span class="sxs-lookup"><span data-stu-id="441ee-227">property_value</span></span> |<span data-ttu-id="441ee-228">文字列</span><span class="sxs-lookup"><span data-stu-id="441ee-228">String</span></span>|<span data-ttu-id="441ee-229">照合する拡張プロパティの値。</span><span class="sxs-lookup"><span data-stu-id="441ee-229">The value of the extended property to match.</span></span> <span data-ttu-id="441ee-230">前述の「**HTTP 要求**」セクションに示した一覧で必要になります。</span><span class="sxs-lookup"><span data-stu-id="441ee-230">Required where listed in the **HTTP request** section above.</span></span> <span data-ttu-id="441ee-231">{property_value} が文字列ではない場合、`ep/value` を {property_value} と比較するときに、適切な Edm データ型に明示的にキャストしてください。</span><span class="sxs-lookup"><span data-stu-id="441ee-231">If {property_value} is not a string, make sure you explicitly cast `ep/value` to the appropriate Edm data type when comparing it with {property_value}.</span></span> <span data-ttu-id="441ee-232">例については、以下の[要求 4](#request-4) を参照してください。</span><span class="sxs-lookup"><span data-stu-id="441ee-232">See [request 4](#request-4) below for examples.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="441ee-233">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="441ee-233">Request headers</span></span>
| <span data-ttu-id="441ee-234">名前</span><span class="sxs-lookup"><span data-stu-id="441ee-234">Name</span></span>      |<span data-ttu-id="441ee-235">説明</span><span class="sxs-lookup"><span data-stu-id="441ee-235">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="441ee-236">Authorization</span><span class="sxs-lookup"><span data-stu-id="441ee-236">Authorization</span></span>  | <span data-ttu-id="441ee-p112">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="441ee-p112">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="441ee-239">要求本文</span><span class="sxs-lookup"><span data-stu-id="441ee-239">Request body</span></span>
<span data-ttu-id="441ee-240">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="441ee-240">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="441ee-241">応答</span><span class="sxs-lookup"><span data-stu-id="441ee-241">Response</span></span>

<span data-ttu-id="441ee-242">成功した場合、このメソッドは `200 OK` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="441ee-242">If successful, this method returns a `200 OK` response code.</span></span>

#### <a name="get-resource-instance-using-expand"></a><span data-ttu-id="441ee-243">`$expand` を使用してリソース インスタンスを取得する</span><span class="sxs-lookup"><span data-stu-id="441ee-243">GET resource instance using `$expand`</span></span>
<span data-ttu-id="441ee-244">応答本文には、一致する [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) オブジェクトで展開された、要求したリソース インスタンスで表されるオブジェクトが含まれます。</span><span class="sxs-lookup"><span data-stu-id="441ee-244">The response body includes an object representing the requested resource instance, expanded with the matching [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object.</span></span>
  
#### <a name="get-resource-instances-that-contain-an-extended-property-matching-a-filter"></a><span data-ttu-id="441ee-245">フィルターと一致する拡張プロパティを含むリソース インスタンスを取得する</span><span class="sxs-lookup"><span data-stu-id="441ee-245">GET resource instances that contain an extended property matching a filter</span></span>
<span data-ttu-id="441ee-246">応答本文には、一致する拡張プロパティを含むリソース インスタンスを表す 1 つ以上のオブジェクトが含まれます。</span><span class="sxs-lookup"><span data-stu-id="441ee-246">The response body includes one or more objects representing the resource instances that contain a matching extended property.</span></span> <span data-ttu-id="441ee-247">応答本文には、拡張プロパティは含まれません。</span><span class="sxs-lookup"><span data-stu-id="441ee-247">The response body does not include the extended property.</span></span>

## <a name="example"></a><span data-ttu-id="441ee-248">例</span><span class="sxs-lookup"><span data-stu-id="441ee-248">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="441ee-249">要求 1</span><span class="sxs-lookup"><span data-stu-id="441ee-249">Request 1</span></span>

<span data-ttu-id="441ee-p114">最初の例では、単一値の拡張プロパティを含めることによって指定されたメッセージを取得して展開します。フィルターは、**id** が文字列 `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` と一致する拡張プロパティを返します (ここでは、読みやすくするため URL エンコードを削除しています)。</span><span class="sxs-lookup"><span data-stu-id="441ee-p114">The first example gets and expands the specified message by including a single-value extended property. The filter returns the extended property that has its **id** matching the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

<!-- {
  "blockType": "request",
  "name": "get_singlevaluelegacyextendedproperty_1"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages('AAMkAGE1M2_bs88AACHsLqWAAA=')?$expand=singleValueExtendedProperties($filter=id%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color')
```
#### <a name="response-1"></a><span data-ttu-id="441ee-252">応答 1</span><span class="sxs-lookup"><span data-stu-id="441ee-252">Response 1</span></span>
<span data-ttu-id="441ee-253">応答本文には、指定されたメッセージのすべてのプロパティと、フィルターから返される拡張プロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="441ee-253">The response body includes all the properties of the specified message and extended property returned from the filter.</span></span>

<span data-ttu-id="441ee-p115">注:簡潔にするために、ここに示す**メッセージ** オブジェクトは切り詰められています。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="441ee-p115">Note: The **message** object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages/$entity",
    "@odata.id": "https://graph.microsoft.com/beta/users('ddfcd489-628b-40d7-b48b-57002df800e5@1717622f-1d94-4d0c-9d74-709fad664b77')/messages('AAMkAGE1M2_bs88AACHsLqWAAA=')",
    "@odata.etag": "W/\"CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AACbyS4H\"",
    "id": "AAMkAGE1M2_bs88AACHsLqWAAA=",
    "subject": "RE: Talk about emergency prep",
    "sender": {
        "emailAddress": {
            "name": "Christine Irwin",
            "address": "christine@contoso.com"
        }
    },
    "from": null,
    "toRecipients": [
        {
            "emailAddress": {
                "name": "Christine Irwin",
                "address": "christine@contoso.com"
            }
        }
    ],
    "singleValueExtendedProperties@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages('AAMkAGE1M2_bs88AACHsLqWAAA%3D')/singleValueExtendedProperties",
    "singleValueExtendedProperties": [
        {
            "id": "String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color",
            "value": "Green"
        }
    ]
}
```

#### <a name="request-2"></a><span data-ttu-id="441ee-256">要求 2</span><span class="sxs-lookup"><span data-stu-id="441ee-256">Request 2</span></span>

<span data-ttu-id="441ee-257">2 番目の例では、文字列で型指定され、フィルターで指定された単一値の拡張プロパティを持つメッセージを取得します。</span><span class="sxs-lookup"><span data-stu-id="441ee-257">The second example gets messages that have the string-typed single-value extended property specified in the filter.</span></span> <span data-ttu-id="441ee-258">フィルターは、以下のような拡張プロパティを検索します。</span><span class="sxs-lookup"><span data-stu-id="441ee-258">The filter looks for the extended property that has:</span></span>

- <span data-ttu-id="441ee-259">その **id** は文字列 `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` と一致します (ここでは、読みやすくするため URL エンコードを削除しています)。</span><span class="sxs-lookup"><span data-stu-id="441ee-259">Its **id** equal to the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

- <span data-ttu-id="441ee-260">その **value** は文字列 `Green` と一致します。</span><span class="sxs-lookup"><span data-stu-id="441ee-260">Its **value** equal to the string `Green`.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/Me/messages?$filter=singleValueExtendedProperties%2FAny(ep%3A%20ep%2Fid%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color'%20and%20ep%2Fvalue%20eq%20'Green')
```

#### <a name="response-2"></a><span data-ttu-id="441ee-261">応答 2</span><span class="sxs-lookup"><span data-stu-id="441ee-261">Response 2</span></span>

<span data-ttu-id="441ee-p117">正常な応答が `HTTP 200 OK` 応答コードによって示され、応答の本文には、フィルターに一致する拡張プロパティを持つメッセージのすべてのプロパティが含まれます。応答本文は、[メッセージのコレクションの取得](../api/user-list-messages.md)からの応答に似ています。応答は、一致する拡張プロパティを含みません。</span><span class="sxs-lookup"><span data-stu-id="441ee-p117">A successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the filter. The response body is similar to the response from [getting a message collection](../api/user-list-messages.md). The response does not include the matching extended property.</span></span>


#### <a name="request-3"></a><span data-ttu-id="441ee-265">要求 3</span><span class="sxs-lookup"><span data-stu-id="441ee-265">Request 3</span></span>

<span data-ttu-id="441ee-266">3 番目の例では、文字列で型指定され、フィルターで指定された単一値の拡張プロパティを持つメッセージを取得します。</span><span class="sxs-lookup"><span data-stu-id="441ee-266">The third example gets messages that have the string-typed single-value extended property specified in the filter.</span></span> <span data-ttu-id="441ee-267">フィルターは、以下のような拡張プロパティを検索します。</span><span class="sxs-lookup"><span data-stu-id="441ee-267">The filter looks for the extended property that has:</span></span>

- <span data-ttu-id="441ee-268">その **id** は文字列 `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` と一致します (ここでは、読みやすくするため URL エンコードを削除しています)。</span><span class="sxs-lookup"><span data-stu-id="441ee-268">Its **id** equal to the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

- <span data-ttu-id="441ee-269">その **value** には文字列 `green` が含まれます。</span><span class="sxs-lookup"><span data-stu-id="441ee-269">Its **value** containing the string `green`.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/Me/messages?$filter=singleValueExtendedProperties/any(ep:ep/Id eq 'String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color' and contains(ep/Value, 'green'))
```

#### <a name="response-3"></a><span data-ttu-id="441ee-270">応答 3</span><span class="sxs-lookup"><span data-stu-id="441ee-270">Response 3</span></span>

<span data-ttu-id="441ee-271">正常な応答が `HTTP 200 OK` 応答コードによって示され、応答の本文には、フィルターに一致する拡張プロパティを持つメッセージのすべてのプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="441ee-271">A successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the filter.</span></span> <span data-ttu-id="441ee-272">たとえば、**id** が文字列 `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color`、**value** `Light green` と等しい単一値の拡張プロパティのあるメッセージがフィルターと一致し、応答に含まれるとします。</span><span class="sxs-lookup"><span data-stu-id="441ee-272">For example, a message that has a single-value extended property with the **id** equal to the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color`, and the **value** `Light green`, would match the filter and be included in the response.</span></span>

<span data-ttu-id="441ee-273">応答本文は、[メッセージのコレクションの取得](../api/user-list-messages.md)からの応答に似ています。</span><span class="sxs-lookup"><span data-stu-id="441ee-273">The response body is similar to the response from [getting a message collection](../api/user-list-messages.md).</span></span> <span data-ttu-id="441ee-274">応答は、一致する拡張プロパティを含みません。</span><span class="sxs-lookup"><span data-stu-id="441ee-274">The response does not include the matching extended property.</span></span>


#### <a name="request-4"></a><span data-ttu-id="441ee-275">要求 4</span><span class="sxs-lookup"><span data-stu-id="441ee-275">Request 4</span></span>

<span data-ttu-id="441ee-276">次の 2 つの例では、文字列以外で型指定された単一値の拡張プロパティを持つメッセージを取得する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="441ee-276">The next 2 examples show how to get messages that have non-string typed single-value extended properties.</span></span> <span data-ttu-id="441ee-277">読みやすくするため、必要な URL エンコードは含まれていません。</span><span class="sxs-lookup"><span data-stu-id="441ee-277">For ease of reading, they do not include the necessary URL encoding.</span></span>

<span data-ttu-id="441ee-278">次の例は、以下のような拡張プロパティを検索するフィルターを示しています。</span><span class="sxs-lookup"><span data-stu-id="441ee-278">The following example shows a filter that looks for the extended property that has:</span></span>

- <span data-ttu-id="441ee-279">その **id** は文字列 `CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid` と一致します。</span><span class="sxs-lookup"><span data-stu-id="441ee-279">Its **id** matching the string `CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid`.</span></span>

- <span data-ttu-id="441ee-280">その **value** は GUID `b9cf8971-7d55-4b73-9ffa-a584611b600b` です。</span><span class="sxs-lookup"><span data-stu-id="441ee-280">Its **value** being the GUID `b9cf8971-7d55-4b73-9ffa-a584611b600b`.</span></span> <span data-ttu-id="441ee-281">プロパティ値を GUID と比較するには、`ep/value` を `Edm.Guid` にキャストします。</span><span class="sxs-lookup"><span data-stu-id="441ee-281">To compare the property value with a GUID, cast `ep/value` to `Edm.Guid`.</span></span>


<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/messages?$filter=singleValueExtendedProperties/any(ep:ep/id eq 'CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid' and cast(ep/value, Edm.Guid) eq (b9cf8971-7d55-4b73-9ffa-a584611b600b))
```

<span data-ttu-id="441ee-282">次の例は、以下のような拡張プロパティを検索するフィルターを示しています。</span><span class="sxs-lookup"><span data-stu-id="441ee-282">The next example shows a filter that looks for the extended property that has:</span></span>

- <span data-ttu-id="441ee-283">その **id** は文字列 `Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete` と一致します。</span><span class="sxs-lookup"><span data-stu-id="441ee-283">Its **id** matching the string `Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete`.</span></span>

- <span data-ttu-id="441ee-284">その **value** は整数 12 と等しくなります。</span><span class="sxs-lookup"><span data-stu-id="441ee-284">Its **value** equal to the integer 12.</span></span> <span data-ttu-id="441ee-285">プロパティ値を整数と比較するには、`ep/value` を `Edm.Int32` にキャストします。</span><span class="sxs-lookup"><span data-stu-id="441ee-285">To compare the property value with an integer, cast `ep/value` to `Edm.Int32`.</span></span>


<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/messages?$filter=singleValueExtendedProperties/any(ep:ep/id eq 'Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete' and cast(ep/value, Edm.Int32) eq 12)
```


#### <a name="response-4"></a><span data-ttu-id="441ee-286">応答 4</span><span class="sxs-lookup"><span data-stu-id="441ee-286">Response 4</span></span>

<span data-ttu-id="441ee-287">前の 2 つの例では、正常な応答が `HTTP 200 OK` 応答コードによって示され、応答の本文には、対応するフィルターに一致する拡張プロパティを持つメッセージのすべてのプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="441ee-287">For each of the preceding 2 examples, a successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the corresponding filter.</span></span> <span data-ttu-id="441ee-288">応答本文は、[メッセージのコレクションの取得](../api/user-list-messages.md)からの応答に似ています。</span><span class="sxs-lookup"><span data-stu-id="441ee-288">The response body is similar to the response from [getting a message collection](../api/user-list-messages.md).</span></span> <span data-ttu-id="441ee-289">応答は、一致する拡張プロパティを含みません。</span><span class="sxs-lookup"><span data-stu-id="441ee-289">The response does not include the matching extended property.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get singleValueLegacyExtendedProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
