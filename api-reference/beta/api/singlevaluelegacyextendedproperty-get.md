---
title: singleValueLegacyExtendedProperty を取得する
description: 特定の拡張プロパティを使用して展開された単一のリソースインスタンス、またはリソースインスタンスのコレクションを取得できます。
localization_priority: Normal
ms.openlocfilehash: b2522f122746ce4054eb8c15bdad65cd8f75b0b2
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35271618"
---
# <a name="get-singlevaluelegacyextendedproperty"></a><span data-ttu-id="d144a-103">singleValueLegacyExtendedProperty を取得する</span><span class="sxs-lookup"><span data-stu-id="d144a-103">Get singleValueLegacyExtendedProperty</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d144a-104">特定の拡張プロパティで展開された単一のリソース インスタンス、または 1 つのフィルターと一致する拡張プロパティを含むリソース インスタンスのコレクションを取得できます。</span><span class="sxs-lookup"><span data-stu-id="d144a-104">You can get a single resource instance expanded with a specific extended property, or a collection of resource instances that include extended properties matching a filter.</span></span>

<span data-ttu-id="d144a-105">クエリ パラメーター `$expand` を使用すると、指定した拡張プロパティで展開された特定のリソース インスタンスを取得できます。</span><span class="sxs-lookup"><span data-stu-id="d144a-105">Using the query parameter `$expand` allows you to get the specified resource instance expanded with a specific extended property.</span></span> <span data-ttu-id="d144a-106">**id** プロパティ上で `$filter` および `eq` 演算子を使用して拡張プロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="d144a-106">Use a `$filter` and `eq` operator on the **id** property to specify the extended property.</span></span> <span data-ttu-id="d144a-107">これは、現時点で、拡張プロパティを表す [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) オブジェクトを取得する唯一の方法です。</span><span class="sxs-lookup"><span data-stu-id="d144a-107">This is currently the only way to get the [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object that represents an extended property.</span></span> 

<span data-ttu-id="d144a-108">特定の拡張プロパティを含むリソース インスタンスを取得するには、`$filter` クエリ パラメーターを使用して、`eq` 演算子を **id** プロパティに適用します。</span><span class="sxs-lookup"><span data-stu-id="d144a-108">To get resource instances that have certain extended properties, use the `$filter` query parameter and apply an `eq` operator on the **id** property.</span></span> <span data-ttu-id="d144a-109">さらに、数値の拡張プロパティについては、**value** プロパティで `eq`、`ne`、`ge`、`gt`、`le`、`lt` 演算子のいずれかを適用します。</span><span class="sxs-lookup"><span data-stu-id="d144a-109">In addition, for numeric extended properties, apply one of the following operators on the **value** property: `eq`, `ne`,`ge`, `gt`, `le`, or `lt`.</span></span> <span data-ttu-id="d144a-110">文字列型の拡張プロパティについては、`contains`、`startswith`、`eq`、`ne` 演算子を **value** に適用します。</span><span class="sxs-lookup"><span data-stu-id="d144a-110">For string-typed extended properties, apply a `contains`, `startswith`, `eq`, or `ne` operator on **value**.</span></span> 

<span data-ttu-id="d144a-111">拡張プロパティの **id** で文字列名 (`Name`) をフィルタリングする場合は、大文字と小文字が区別されます。</span><span class="sxs-lookup"><span data-stu-id="d144a-111">Filtering the string name (`Name`) in the **id** of an extended property is case-sensitive.</span></span> <span data-ttu-id="d144a-112">拡張プロパティの **value** プロパティをフィルタリングする場合は、大文字と小文字が区別されません。</span><span class="sxs-lookup"><span data-stu-id="d144a-112">Filtering the **value** property of an extended property is case-insensitive.</span></span>

<span data-ttu-id="d144a-113">次のユーザー リソースがサポートされます。</span><span class="sxs-lookup"><span data-stu-id="d144a-113">The following user resources are supported:</span></span>

- [<span data-ttu-id="d144a-114">calendar</span><span class="sxs-lookup"><span data-stu-id="d144a-114">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="d144a-115">contact</span><span class="sxs-lookup"><span data-stu-id="d144a-115">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="d144a-116">contactFolder</span><span class="sxs-lookup"><span data-stu-id="d144a-116">contactFolder</span></span>](../resources/contactfolder.md) 
- [<span data-ttu-id="d144a-117">event</span><span class="sxs-lookup"><span data-stu-id="d144a-117">event</span></span>](../resources/event.md)
- [<span data-ttu-id="d144a-118">mailFolder</span><span class="sxs-lookup"><span data-stu-id="d144a-118">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="d144a-119">message</span><span class="sxs-lookup"><span data-stu-id="d144a-119">message</span></span>](../resources/message.md) 
- [<span data-ttu-id="d144a-120">Outlook タスク</span><span class="sxs-lookup"><span data-stu-id="d144a-120">Outlook task</span></span>](../resources/outlooktask.md)
- [<span data-ttu-id="d144a-121">Outlook タスク フォルダー</span><span class="sxs-lookup"><span data-stu-id="d144a-121">Outlook task folder</span></span>](../resources/outlooktaskfolder.md)

<span data-ttu-id="d144a-122">次のグループ リソースもサポートされます。</span><span class="sxs-lookup"><span data-stu-id="d144a-122">As well as the following group resources:</span></span>

- <span data-ttu-id="d144a-123">グループ [calendar](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="d144a-123">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="d144a-124">グループ [event](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="d144a-124">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="d144a-125">グループ [post](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="d144a-125">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="d144a-126">オープン拡張機能または拡張プロパティを使用するのに適した状況と、拡張プロパティを指定する方法の詳細については、「[拡張プロパティの概要](../resources/extended-properties-overview.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d144a-126">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="d144a-127">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d144a-127">Permissions</span></span>
<span data-ttu-id="d144a-128">この API を呼び出すには、拡張プロパティの取得元のリソースと、要求したアクセス許可の種類 (委任またはアプリケーション) に応じて、次の表で指定されているアクセス許可が最低限必要です。</span><span class="sxs-lookup"><span data-stu-id="d144a-128">Depending on the resource you're getting the extended property from and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="d144a-129">アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d144a-129">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d144a-130">サポートされているリソース</span><span class="sxs-lookup"><span data-stu-id="d144a-130">Supported resource</span></span> | <span data-ttu-id="d144a-131">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d144a-131">Delegated (work or school account)</span></span> | <span data-ttu-id="d144a-132">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d144a-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d144a-133">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d144a-133">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="d144a-134">calendar</span><span class="sxs-lookup"><span data-stu-id="d144a-134">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="d144a-135">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d144a-135">Calendars.Read</span></span> | <span data-ttu-id="d144a-136">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d144a-136">Calendars.Read</span></span> | <span data-ttu-id="d144a-137">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d144a-137">Calendars.Read</span></span> |
| [<span data-ttu-id="d144a-138">連絡先</span><span class="sxs-lookup"><span data-stu-id="d144a-138">contact</span></span>](../resources/contact.md) | <span data-ttu-id="d144a-139">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="d144a-139">Contacts.Read</span></span> | <span data-ttu-id="d144a-140">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="d144a-140">Contacts.Read</span></span> | <span data-ttu-id="d144a-141">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="d144a-141">Contacts.Read</span></span> |
| [<span data-ttu-id="d144a-142">contactFolder</span><span class="sxs-lookup"><span data-stu-id="d144a-142">contactFolder</span></span>](../resources/contactfolder.md) | <span data-ttu-id="d144a-143">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="d144a-143">Contacts.Read</span></span> | <span data-ttu-id="d144a-144">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="d144a-144">Contacts.Read</span></span> | <span data-ttu-id="d144a-145">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="d144a-145">Contacts.Read</span></span> |
| [<span data-ttu-id="d144a-146">event</span><span class="sxs-lookup"><span data-stu-id="d144a-146">event</span></span>](../resources/event.md) | <span data-ttu-id="d144a-147">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d144a-147">Calendars.Read</span></span> | <span data-ttu-id="d144a-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d144a-148">Calendars.Read</span></span> |  <span data-ttu-id="d144a-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d144a-149">Calendars.Read</span></span>|
| <span data-ttu-id="d144a-150">グループ [calendar](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="d144a-150">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="d144a-151">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="d144a-151">Group.Read.All</span></span> | <span data-ttu-id="d144a-152">非サポート</span><span class="sxs-lookup"><span data-stu-id="d144a-152">Not supported</span></span> | <span data-ttu-id="d144a-153">非サポート</span><span class="sxs-lookup"><span data-stu-id="d144a-153">Not supported</span></span> |
| <span data-ttu-id="d144a-154">グループ [event](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="d144a-154">group [event](../resources/event.md)</span></span> | <span data-ttu-id="d144a-155">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="d144a-155">Group.Read.All</span></span> | <span data-ttu-id="d144a-156">非サポート</span><span class="sxs-lookup"><span data-stu-id="d144a-156">Not supported</span></span> | <span data-ttu-id="d144a-157">非サポート</span><span class="sxs-lookup"><span data-stu-id="d144a-157">Not supported</span></span> |
| <span data-ttu-id="d144a-158">グループ [post](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="d144a-158">group [post](../resources/post.md)</span></span> | <span data-ttu-id="d144a-159">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="d144a-159">Group.Read.All</span></span> | <span data-ttu-id="d144a-160">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="d144a-160">Not supported</span></span> | <span data-ttu-id="d144a-161">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="d144a-161">Group.Read.All</span></span> |
| [<span data-ttu-id="d144a-162">mailFolder</span><span class="sxs-lookup"><span data-stu-id="d144a-162">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="d144a-163">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="d144a-163">Mail.Read</span></span> | <span data-ttu-id="d144a-164">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="d144a-164">Mail.Read</span></span> | <span data-ttu-id="d144a-165">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="d144a-165">Mail.Read</span></span> |
| [<span data-ttu-id="d144a-166">message</span><span class="sxs-lookup"><span data-stu-id="d144a-166">message</span></span>](../resources/message.md) | <span data-ttu-id="d144a-167">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="d144a-167">Mail.Read</span></span> | <span data-ttu-id="d144a-168">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="d144a-168">Mail.Read</span></span> | <span data-ttu-id="d144a-169">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="d144a-169">Mail.Read</span></span> |
| [<span data-ttu-id="d144a-170">Outlook タスク</span><span class="sxs-lookup"><span data-stu-id="d144a-170">Outlook task</span></span>](../resources/outlooktask.md) | <span data-ttu-id="d144a-171">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="d144a-171">Tasks.Read</span></span> | <span data-ttu-id="d144a-172">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="d144a-172">Tasks.Read</span></span> | <span data-ttu-id="d144a-173">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="d144a-173">Not supported</span></span> |
| [<span data-ttu-id="d144a-174">Outlook タスク フォルダー</span><span class="sxs-lookup"><span data-stu-id="d144a-174">Outlook task folder</span></span>](../resources/outlooktaskfolder.md) | <span data-ttu-id="d144a-175">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="d144a-175">Tasks.Read</span></span> | <span data-ttu-id="d144a-176">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="d144a-176">Tasks.Read</span></span> | <span data-ttu-id="d144a-177">非サポート</span><span class="sxs-lookup"><span data-stu-id="d144a-177">Not supported</span></span> |


## <a name="http-request"></a><span data-ttu-id="d144a-178">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d144a-178">HTTP request</span></span>

#### <a name="get-a-resource-instance-expanded-with-an-extended-property-that-matches-a-filter"></a><span data-ttu-id="d144a-179">フィルターと一致する拡張プロパティで展開されたリソース インスタンスを取得する</span><span class="sxs-lookup"><span data-stu-id="d144a-179">GET a resource instance expanded with an extended property that matches a filter</span></span>
<span data-ttu-id="d144a-p105">**id** プロパティに対するフィルターと一致する拡張プロパティで展開された、リソース インスタンスを取得します。フィルター文字列内のスペース文字に [URL エンコード](https://www.w3schools.com/tags/ref_urlencode.asp)を適用していることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="d144a-p105">Get a resource instance expanded with the extended property which matches a filter on the **id** property. Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the filter string.</span></span>

<span data-ttu-id="d144a-182">**message** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="d144a-182">Get a **message** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="d144a-183">**mailFolder** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="d144a-183">Get a **mailFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="d144a-184">**event** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="d144a-184">Get an **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="d144a-185">**calendar** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="d144a-185">Get a **calendar** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="d144a-186">**contact** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="d144a-186">Get a **contact** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="d144a-187">**contactFolder** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="d144a-187">Get a **contactFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="d144a-188">**Outlooktask**インスタンスを取得します。</span><span class="sxs-lookup"><span data-stu-id="d144a-188">Get an **outlookTask** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskFolders/{id}/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="d144a-189">**Outlooktaskfolder**インスタンスを取得します。</span><span class="sxs-lookup"><span data-stu-id="d144a-189">Get an **outlookTaskFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskGroups/{id}/taskFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="d144a-190">グループ **event** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="d144a-190">Get a group **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="d144a-191">グループ **post** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="d144a-191">Get a group **post** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

#### <a name="get-resource-instances-that-include-numeric-extended-properties-matching-a-filter"></a><span data-ttu-id="d144a-192">フィルターと一致する数値の拡張プロパティを含むリソース インスタンスを取得する</span><span class="sxs-lookup"><span data-stu-id="d144a-192">GET resource instances that include numeric extended properties matching a filter</span></span>

<span data-ttu-id="d144a-193">フィルターと一致する数値の拡張プロパティを持つサポート対象リソースのインスタンスを取得します。</span><span class="sxs-lookup"><span data-stu-id="d144a-193">Get instances of a supported resource that have a numeric extended property matching a filter.</span></span> <span data-ttu-id="d144a-194">フィルターは **id** プロパティには `eq` 演算子を使用し、**value** プロパティには `eq`、`ne`、`ge`、`gt`、`le`、`lt` のいずれかの演算子を使用します。</span><span class="sxs-lookup"><span data-stu-id="d144a-194">The filter uses an `eq` operator on the **id** property, and one of the following operators on the **value** property: `eq`, `ne`,`ge`, `gt`, `le`, or `lt`.</span></span> <span data-ttu-id="d144a-195">必ず適用してください。フィルター文字列のコロン、スラッシュ、スペースで、次の文字に[URL エンコード](https://www.w3schools.com/tags/ref_urlencode.asp)を適用してください。</span><span class="sxs-lookup"><span data-stu-id="d144a-195">Make sure you apply Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the following characters in the filter string - colon, forward slash, and space.</span></span>

<span data-ttu-id="d144a-196">次の構文の行では、id に `eq` 演算子を使用し、プロパティ値にもう 1 つの `eq` 演算子を使用するフィルターを示しています。</span><span class="sxs-lookup"><span data-stu-id="d144a-196">The following syntax lines show a filter that uses an `eq` operator on the id, and another `eq` operator on the property value.</span></span> <span data-ttu-id="d144a-197">**value** に対する `eq` 演算子は、数値に適用される別の演算子 (`ne`、`ge`、`gt`、`le`、`lt`) のいずれかと置き換えることができます。</span><span class="sxs-lookup"><span data-stu-id="d144a-197">You can substitute the `eq` operator on the **value** by any one of the other operators (`ne`,`ge`, `gt`, `le`, or `lt`) that apply to numeric values.</span></span>

<span data-ttu-id="d144a-198">**message** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="d144a-198">Get **message** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="d144a-199">**mailFolder** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="d144a-199">Get **mailFolder** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="d144a-200">**event** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="d144a-200">Get **event** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="d144a-201">**calendar** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="d144a-201">Get **calendar** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="d144a-202">**contact** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="d144a-202">Get **contact** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="d144a-203">**contactFolder** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="d144a-203">Get **contactFolder** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="d144a-204">**Outlooktask**インスタンスを取得します。</span><span class="sxs-lookup"><span data-stu-id="d144a-204">Get an **outlookTask** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/outlook/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/outlook/taskFolders/{id}/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="d144a-205">**Outlooktaskfolder**インスタンスを取得します。</span><span class="sxs-lookup"><span data-stu-id="d144a-205">Get an **outlookTaskFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/outlook/taskGroups/{id}/taskFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="d144a-206">グループ **event** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="d144a-206">Get group **event** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="d144a-207">グループ **post** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="d144a-207">Get group **post** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

#### <a name="get-resource-instances-with-string-typed-extended-properties-matching-a-filter"></a><span data-ttu-id="d144a-208">フィルターと一致する文字列型の拡張プロパティを含むリソース インスタンスを取得する</span><span class="sxs-lookup"><span data-stu-id="d144a-208">GET resource instances with string-typed extended properties matching a filter</span></span>

<span data-ttu-id="d144a-209">フィルターと一致する文字列型の拡張プロパティを含む **message** または **event** リソースのインスタンスを取得します。</span><span class="sxs-lookup"><span data-stu-id="d144a-209">Get instances of the **message** or **event** resource that have a string-typed extended property matching a filter.</span></span> <span data-ttu-id="d144a-210">フィルターは **id** プロパティには `eq` 演算子を使用し、**value** プロパティには `contains`、`startswith`、`eq`、`ne` のいずれかの演算子を使用します。</span><span class="sxs-lookup"><span data-stu-id="d144a-210">The filter uses an `eq` operator on the **id** property, and one of the following operators on the **value** property: `contains`, `startswith`, `eq`, or `ne`.</span></span> <span data-ttu-id="d144a-211">フィルター文字列内のコロン、スラッシュ、スペースに [URL エンコード](https://www.w3schools.com/tags/ref_urlencode.asp)を適用していることをご確認ください。</span><span class="sxs-lookup"><span data-stu-id="d144a-211">Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the following characters in the filter string - colon, forward slash, and space.</span></span>


<span data-ttu-id="d144a-212">**message** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="d144a-212">Get **message** instances:</span></span>
<!-- { "blockType": "ignored" } -->
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

<span data-ttu-id="d144a-213">**event** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="d144a-213">Get **event** instances:</span></span>
<!-- { "blockType": "ignored" } -->
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

<span data-ttu-id="d144a-214">グループ **event** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="d144a-214">Get group **event** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
```

## <a name="path-parameters"></a><span data-ttu-id="d144a-215">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="d144a-215">Path parameters</span></span>
|<span data-ttu-id="d144a-216">**パラメーター**</span><span class="sxs-lookup"><span data-stu-id="d144a-216">**Parameter**</span></span>|<span data-ttu-id="d144a-217">**型**</span><span class="sxs-lookup"><span data-stu-id="d144a-217">**Type**</span></span>|<span data-ttu-id="d144a-218">**説明**</span><span class="sxs-lookup"><span data-stu-id="d144a-218">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="d144a-219">id_value</span><span class="sxs-lookup"><span data-stu-id="d144a-219">id_value</span></span>|<span data-ttu-id="d144a-220">String</span><span class="sxs-lookup"><span data-stu-id="d144a-220">String</span></span>|<span data-ttu-id="d144a-p109">照合する拡張プロパティの ID。サポートされている形式のいずれかに従う必要があります。詳しくは、「[Outlook の拡張プロパティの概要](../resources/extended-properties-overview.md)」を参照してください。必須。</span><span class="sxs-lookup"><span data-stu-id="d144a-p109">The ID of the extended property to match. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|
|<span data-ttu-id="d144a-225">property_value</span><span class="sxs-lookup"><span data-stu-id="d144a-225">property_value</span></span> |<span data-ttu-id="d144a-226">String</span><span class="sxs-lookup"><span data-stu-id="d144a-226">String</span></span>|<span data-ttu-id="d144a-227">照合する拡張プロパティの値。</span><span class="sxs-lookup"><span data-stu-id="d144a-227">The value of the extended property to match.</span></span> <span data-ttu-id="d144a-228">前述の「**HTTP 要求**」セクションに示した一覧で必要になります。</span><span class="sxs-lookup"><span data-stu-id="d144a-228">Required where listed in the **HTTP request** section above.</span></span> <span data-ttu-id="d144a-229">{property_value} が文字列ではない場合、`ep/value` を {property_value} と比較するときに、適切な Edm データ型に明示的にキャストしてください。</span><span class="sxs-lookup"><span data-stu-id="d144a-229">If {property_value} is not a string, make sure you explicitly cast `ep/value` to the appropriate Edm data type when comparing it with {property_value}.</span></span> <span data-ttu-id="d144a-230">例については、以下の[要求 4](#request-4) を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d144a-230">See [request 4](#request-4) below for examples.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="d144a-231">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d144a-231">Request headers</span></span>
| <span data-ttu-id="d144a-232">名前</span><span class="sxs-lookup"><span data-stu-id="d144a-232">Name</span></span>      |<span data-ttu-id="d144a-233">説明</span><span class="sxs-lookup"><span data-stu-id="d144a-233">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d144a-234">Authorization</span><span class="sxs-lookup"><span data-stu-id="d144a-234">Authorization</span></span>  | <span data-ttu-id="d144a-p111">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d144a-p111">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d144a-237">要求本文</span><span class="sxs-lookup"><span data-stu-id="d144a-237">Request body</span></span>
<span data-ttu-id="d144a-238">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d144a-238">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d144a-239">応答</span><span class="sxs-lookup"><span data-stu-id="d144a-239">Response</span></span>

<span data-ttu-id="d144a-240">成功した場合、このメソッドは `200 OK` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="d144a-240">If successful, this method returns a `200 OK` response code.</span></span>

#### <a name="get-resource-instance-using-expand"></a><span data-ttu-id="d144a-241">`$expand` を使用してリソース インスタンスを取得する</span><span class="sxs-lookup"><span data-stu-id="d144a-241">GET resource instance using `$expand`</span></span>
<span data-ttu-id="d144a-242">応答本文には、一致する [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) オブジェクトで展開された、要求したリソース インスタンスで表されるオブジェクトが含まれます。</span><span class="sxs-lookup"><span data-stu-id="d144a-242">The response body includes an object representing the requested resource instance, expanded with the matching [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object.</span></span>
  
#### <a name="get-resource-instances-that-contain-an-extended-property-matching-a-filter"></a><span data-ttu-id="d144a-243">フィルターと一致する拡張プロパティを含むリソース インスタンスを取得する</span><span class="sxs-lookup"><span data-stu-id="d144a-243">GET resource instances that contain an extended property matching a filter</span></span>
<span data-ttu-id="d144a-244">応答本文には、一致する拡張プロパティを含むリソース インスタンスを表す 1 つ以上のオブジェクトが含まれます。</span><span class="sxs-lookup"><span data-stu-id="d144a-244">The response body includes one or more objects representing the resource instances that contain a matching extended property.</span></span> <span data-ttu-id="d144a-245">応答本文には、拡張プロパティは含まれません。</span><span class="sxs-lookup"><span data-stu-id="d144a-245">The response body does not include the extended property.</span></span>

## <a name="example"></a><span data-ttu-id="d144a-246">例</span><span class="sxs-lookup"><span data-stu-id="d144a-246">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="d144a-247">要求 1</span><span class="sxs-lookup"><span data-stu-id="d144a-247">Request 1</span></span>

<span data-ttu-id="d144a-p113">最初の例では、単一値の拡張プロパティを含めることによって指定されたメッセージを取得して展開します。フィルターは、**id** が文字列 `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` と一致する拡張プロパティを返します (ここでは、読みやすくするため URL エンコードを削除しています)。</span><span class="sxs-lookup"><span data-stu-id="d144a-p113">The first example gets and expands the specified message by including a single-value extended property. The filter returns the extended property that has its **id** matching the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

<!-- {
  "blockType": "request",
  "name": "get_singlevaluelegacyextendedproperty_1"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages/AAMkAGE1M2_bs88AACHsLqWAAA=/?$expand=singleValueExtendedProperties($filter=id%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color')
```
#### <a name="response-1"></a><span data-ttu-id="d144a-250">応答 1</span><span class="sxs-lookup"><span data-stu-id="d144a-250">Response 1</span></span>
<span data-ttu-id="d144a-251">応答本文には、指定されたメッセージのすべてのプロパティと、フィルターから返される拡張プロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="d144a-251">The response body includes all the properties of the specified message and extended property returned from the filter.</span></span>

<span data-ttu-id="d144a-p114">注:簡潔にするために、ここに示す**メッセージ** オブジェクトは切り詰められています。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d144a-p114">Note: The **message** object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="d144a-254">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="d144a-254">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d144a-255">C#</span><span class="sxs-lookup"><span data-stu-id="d144a-255">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_singlevaluelegacyextendedproperty_1-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d144a-256">Javascript</span><span class="sxs-lookup"><span data-stu-id="d144a-256">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_singlevaluelegacyextendedproperty_1-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d144a-257">目的-C</span><span class="sxs-lookup"><span data-stu-id="d144a-257">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_singlevaluelegacyextendedproperty_1-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

#### <a name="request-2"></a><span data-ttu-id="d144a-258">要求 2</span><span class="sxs-lookup"><span data-stu-id="d144a-258">Request 2</span></span>

<span data-ttu-id="d144a-259">2 番目の例では、文字列で型指定され、フィルターで指定された単一値の拡張プロパティを持つメッセージを取得します。</span><span class="sxs-lookup"><span data-stu-id="d144a-259">The second example gets messages that have the string-typed single-value extended property specified in the filter.</span></span> <span data-ttu-id="d144a-260">フィルターは、以下のような拡張プロパティを検索します。</span><span class="sxs-lookup"><span data-stu-id="d144a-260">The filter looks for the extended property that has:</span></span>

- <span data-ttu-id="d144a-261">その **id** は文字列 `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` と一致します (ここでは、読みやすくするため URL エンコードを削除しています)。</span><span class="sxs-lookup"><span data-stu-id="d144a-261">Its **id** equal to the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

- <span data-ttu-id="d144a-262">その **value** は文字列 `Green` と一致します。</span><span class="sxs-lookup"><span data-stu-id="d144a-262">Its **value** equal to the string `Green`.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/messages?$filter=singleValueExtendedProperties%2FAny(ep%3A%20ep%2Fid%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color'%20and%20ep%2Fvalue%20eq%20'Green')
```

#### <a name="response-2"></a><span data-ttu-id="d144a-263">応答 2</span><span class="sxs-lookup"><span data-stu-id="d144a-263">Response 2</span></span>

<span data-ttu-id="d144a-p116">正常な応答が `HTTP 200 OK` 応答コードによって示され、応答の本文には、フィルターに一致する拡張プロパティを持つメッセージのすべてのプロパティが含まれます。応答本文は、[メッセージのコレクションの取得](../api/user-list-messages.md)からの応答に似ています。応答は、一致する拡張プロパティを含みません。</span><span class="sxs-lookup"><span data-stu-id="d144a-p116">A successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the filter. The response body is similar to the response from [getting a message collection](../api/user-list-messages.md). The response does not include the matching extended property.</span></span>


#### <a name="request-3"></a><span data-ttu-id="d144a-267">要求 3</span><span class="sxs-lookup"><span data-stu-id="d144a-267">Request 3</span></span>

<span data-ttu-id="d144a-268">3 番目の例では、文字列で型指定され、フィルターで指定された単一値の拡張プロパティを持つメッセージを取得します。</span><span class="sxs-lookup"><span data-stu-id="d144a-268">The third example gets messages that have the string-typed single-value extended property specified in the filter.</span></span> <span data-ttu-id="d144a-269">フィルターは、以下のような拡張プロパティを検索します。</span><span class="sxs-lookup"><span data-stu-id="d144a-269">The filter looks for the extended property that has:</span></span>

- <span data-ttu-id="d144a-270">その **id** は文字列 `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` と一致します (ここでは、読みやすくするため URL エンコードを削除しています)。</span><span class="sxs-lookup"><span data-stu-id="d144a-270">Its **id** equal to the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

- <span data-ttu-id="d144a-271">その **value** には文字列 `green` が含まれます。</span><span class="sxs-lookup"><span data-stu-id="d144a-271">Its **value** containing the string `green`.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/messages?$filter=singleValueExtendedProperties/any(ep:ep/Id eq 'String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color' and contains(ep/Value, 'green'))
```

#### <a name="response-3"></a><span data-ttu-id="d144a-272">応答 3</span><span class="sxs-lookup"><span data-stu-id="d144a-272">Response 3</span></span>

<span data-ttu-id="d144a-273">正常な応答が `HTTP 200 OK` 応答コードによって示され、応答の本文には、フィルターに一致する拡張プロパティを持つメッセージのすべてのプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="d144a-273">A successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the filter.</span></span> <span data-ttu-id="d144a-274">たとえば、**id** が文字列 `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color`、**value** `Light green` と等しい単一値の拡張プロパティのあるメッセージがフィルターと一致し、応答に含まれるとします。</span><span class="sxs-lookup"><span data-stu-id="d144a-274">For example, a message that has a single-value extended property with the **id** equal to the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color`, and the **value** `Light green`, would match the filter and be included in the response.</span></span>

<span data-ttu-id="d144a-275">応答本文は、[メッセージのコレクションの取得](../api/user-list-messages.md)からの応答に似ています。</span><span class="sxs-lookup"><span data-stu-id="d144a-275">The response body is similar to the response from [getting a message collection](../api/user-list-messages.md).</span></span> <span data-ttu-id="d144a-276">応答は、一致する拡張プロパティを含みません。</span><span class="sxs-lookup"><span data-stu-id="d144a-276">The response does not include the matching extended property.</span></span>


#### <a name="request-4"></a><span data-ttu-id="d144a-277">要求 4</span><span class="sxs-lookup"><span data-stu-id="d144a-277">Request 4</span></span>

<span data-ttu-id="d144a-278">次の 2 つの例では、文字列以外で型指定された単一値の拡張プロパティを持つメッセージを取得する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="d144a-278">The next 2 examples show how to get messages that have non-string typed single-value extended properties.</span></span> <span data-ttu-id="d144a-279">読みやすくするため、必要な URL エンコードは含まれていません。</span><span class="sxs-lookup"><span data-stu-id="d144a-279">For ease of reading, they do not include the necessary URL encoding.</span></span>

<span data-ttu-id="d144a-280">次の例は、以下のような拡張プロパティを検索するフィルターを示しています。</span><span class="sxs-lookup"><span data-stu-id="d144a-280">The following example shows a filter that looks for the extended property that has:</span></span>

- <span data-ttu-id="d144a-281">その **id** は文字列 `CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid` と一致します。</span><span class="sxs-lookup"><span data-stu-id="d144a-281">Its **id** matching the string `CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid`.</span></span>

- <span data-ttu-id="d144a-282">その **value** は GUID `b9cf8971-7d55-4b73-9ffa-a584611b600b` です。</span><span class="sxs-lookup"><span data-stu-id="d144a-282">Its **value** being the GUID `b9cf8971-7d55-4b73-9ffa-a584611b600b`.</span></span> <span data-ttu-id="d144a-283">プロパティ値を GUID と比較するには、`ep/value` を `Edm.Guid` にキャストします。</span><span class="sxs-lookup"><span data-stu-id="d144a-283">To compare the property value with a GUID, cast `ep/value` to `Edm.Guid`.</span></span>


<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/messages?$filter=singleValueExtendedProperties/any(ep:ep/id eq 'CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid' and cast(ep/value, Edm.Guid) eq (b9cf8971-7d55-4b73-9ffa-a584611b600b))
```

<span data-ttu-id="d144a-284">次の例は、以下のような拡張プロパティを検索するフィルターを示しています。</span><span class="sxs-lookup"><span data-stu-id="d144a-284">The next example shows a filter that looks for the extended property that has:</span></span>

- <span data-ttu-id="d144a-285">その **id** は文字列 `Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete` と一致します。</span><span class="sxs-lookup"><span data-stu-id="d144a-285">Its **id** matching the string `Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete`.</span></span>

- <span data-ttu-id="d144a-286">その **value** は整数 12 と等しくなります。</span><span class="sxs-lookup"><span data-stu-id="d144a-286">Its **value** equal to the integer 12.</span></span> <span data-ttu-id="d144a-287">プロパティ値を整数と比較するには、`ep/value` を `Edm.Int32` にキャストします。</span><span class="sxs-lookup"><span data-stu-id="d144a-287">To compare the property value with an integer, cast `ep/value` to `Edm.Int32`.</span></span>


<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/messages?$filter=singleValueExtendedProperties/any(ep:ep/id eq 'Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete' and cast(ep/value, Edm.Int32) eq 12)
```


#### <a name="response-4"></a><span data-ttu-id="d144a-288">応答 4</span><span class="sxs-lookup"><span data-stu-id="d144a-288">Response 4</span></span>

<span data-ttu-id="d144a-289">前の 2 つの例では、正常な応答が `HTTP 200 OK` 応答コードによって示され、応答の本文には、対応するフィルターに一致する拡張プロパティを持つメッセージのすべてのプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="d144a-289">For each of the preceding 2 examples, a successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the corresponding filter.</span></span> <span data-ttu-id="d144a-290">応答本文は、[メッセージのコレクションの取得](../api/user-list-messages.md)からの応答に似ています。</span><span class="sxs-lookup"><span data-stu-id="d144a-290">The response body is similar to the response from [getting a message collection](../api/user-list-messages.md).</span></span> <span data-ttu-id="d144a-291">応答は、一致する拡張プロパティを含みません。</span><span class="sxs-lookup"><span data-stu-id="d144a-291">The response does not include the matching extended property.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get singleValueLegacyExtendedProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/singlevaluelegacyextendedproperty-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/singlevaluelegacyextendedproperty-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/singlevaluelegacyextendedproperty-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
