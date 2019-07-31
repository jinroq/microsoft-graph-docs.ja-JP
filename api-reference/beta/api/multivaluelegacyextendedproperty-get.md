---
title: multiValueLegacyExtendedProperty を取得する
description: '[] を展開します。'
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: cdde391b0dfec4932a8142ede97a08621a5f16bd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35992788"
---
# <a name="get-multivaluelegacyextendedproperty"></a><span data-ttu-id="58ab1-103">multiValueLegacyExtendedProperty を取得する</span><span class="sxs-lookup"><span data-stu-id="58ab1-103">Get multiValueLegacyExtendedProperty</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="58ab1-104">`$expand` を使用して、複数値の拡張プロパティを含むリソース インスタンスを取得します。</span><span class="sxs-lookup"><span data-stu-id="58ab1-104">Get a resource instance that contains a multi-value extended property by using `$expand`.</span></span>

<span data-ttu-id="58ab1-105">クエリ パラメーター `$expand` を使用すると、指示された拡張プロパティで展開された特定のインスタンスを取得できます。</span><span class="sxs-lookup"><span data-stu-id="58ab1-105">Using the query parameter `$expand` allows you to get the specified instance expanded with the indicated extended property.</span></span> <span data-ttu-id="58ab1-106">これは、現時点で、拡張プロパティを表す [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) オブジェクトを取得する唯一の方法です。</span><span class="sxs-lookup"><span data-stu-id="58ab1-106">This is currently the only way to get the [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object that represents an extended property.</span></span>

<span data-ttu-id="58ab1-107">次のユーザー リソースがサポートされます。</span><span class="sxs-lookup"><span data-stu-id="58ab1-107">The following user resources are supported:</span></span>

- [<span data-ttu-id="58ab1-108">calendar</span><span class="sxs-lookup"><span data-stu-id="58ab1-108">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="58ab1-109">contact</span><span class="sxs-lookup"><span data-stu-id="58ab1-109">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="58ab1-110">contactFolder</span><span class="sxs-lookup"><span data-stu-id="58ab1-110">contactFolder</span></span>](../resources/contactfolder.md) 
- [<span data-ttu-id="58ab1-111">event</span><span class="sxs-lookup"><span data-stu-id="58ab1-111">event</span></span>](../resources/event.md)
- [<span data-ttu-id="58ab1-112">mailFolder</span><span class="sxs-lookup"><span data-stu-id="58ab1-112">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="58ab1-113">message</span><span class="sxs-lookup"><span data-stu-id="58ab1-113">message</span></span>](../resources/message.md) 
- [<span data-ttu-id="58ab1-114">Outlook タスク</span><span class="sxs-lookup"><span data-stu-id="58ab1-114">Outlook task</span></span>](../resources/outlooktask.md)
- [<span data-ttu-id="58ab1-115">Outlook タスク フォルダー</span><span class="sxs-lookup"><span data-stu-id="58ab1-115">Outlook task folder</span></span>](../resources/outlooktaskfolder.md)

<span data-ttu-id="58ab1-116">次のグループ リソースもサポートされます。</span><span class="sxs-lookup"><span data-stu-id="58ab1-116">As well as the following group resources:</span></span>

- <span data-ttu-id="58ab1-117">グループ [calendar](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="58ab1-117">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="58ab1-118">グループ [event](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="58ab1-118">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="58ab1-119">グループ [post](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="58ab1-119">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="58ab1-120">オープン拡張機能または拡張プロパティを使用するのに適した状況と、拡張プロパティを指定する方法の詳細については、「[拡張プロパティの概要](../resources/extended-properties-overview.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="58ab1-120">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="58ab1-121">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="58ab1-121">Permissions</span></span>
<span data-ttu-id="58ab1-122">この API を呼び出すには、拡張プロパティの取得元のリソースと、要求したアクセス許可の種類 (委任またはアプリケーション) に応じて、次の表で指定されているアクセス許可が最低限必要です。</span><span class="sxs-lookup"><span data-stu-id="58ab1-122">Depending on the resource you're getting the extended property from and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="58ab1-123">アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="58ab1-123">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="58ab1-124">サポートされているリソース</span><span class="sxs-lookup"><span data-stu-id="58ab1-124">Supported resource</span></span> | <span data-ttu-id="58ab1-125">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="58ab1-125">Delegated (work or school account)</span></span> | <span data-ttu-id="58ab1-126">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="58ab1-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58ab1-127">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="58ab1-127">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="58ab1-128">calendar</span><span class="sxs-lookup"><span data-stu-id="58ab1-128">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="58ab1-129">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="58ab1-129">Calendars.Read</span></span> | <span data-ttu-id="58ab1-130">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="58ab1-130">Calendars.Read</span></span> | <span data-ttu-id="58ab1-131">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="58ab1-131">Calendars.Read</span></span> |
| [<span data-ttu-id="58ab1-132">連絡先</span><span class="sxs-lookup"><span data-stu-id="58ab1-132">contact</span></span>](../resources/contact.md) | <span data-ttu-id="58ab1-133">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="58ab1-133">Contacts.Read</span></span> | <span data-ttu-id="58ab1-134">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="58ab1-134">Contacts.Read</span></span> | <span data-ttu-id="58ab1-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="58ab1-135">Contacts.Read</span></span> |
| [<span data-ttu-id="58ab1-136">contactFolder</span><span class="sxs-lookup"><span data-stu-id="58ab1-136">contactFolder</span></span>](../resources/contactfolder.md) | <span data-ttu-id="58ab1-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="58ab1-137">Contacts.Read</span></span> | <span data-ttu-id="58ab1-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="58ab1-138">Contacts.Read</span></span> | <span data-ttu-id="58ab1-139">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="58ab1-139">Contacts.Read</span></span> |
| [<span data-ttu-id="58ab1-140">event</span><span class="sxs-lookup"><span data-stu-id="58ab1-140">event</span></span>](../resources/event.md) | <span data-ttu-id="58ab1-141">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="58ab1-141">Calendars.Read</span></span> | <span data-ttu-id="58ab1-142">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="58ab1-142">Calendars.Read</span></span> |  <span data-ttu-id="58ab1-143">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="58ab1-143">Calendars.Read</span></span>|
| <span data-ttu-id="58ab1-144">グループ [calendar](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="58ab1-144">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="58ab1-145">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="58ab1-145">Group.Read.All</span></span> | <span data-ttu-id="58ab1-146">非サポート</span><span class="sxs-lookup"><span data-stu-id="58ab1-146">Not supported</span></span> | <span data-ttu-id="58ab1-147">非サポート</span><span class="sxs-lookup"><span data-stu-id="58ab1-147">Not supported</span></span> |
| <span data-ttu-id="58ab1-148">グループ [event](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="58ab1-148">group [event](../resources/event.md)</span></span> | <span data-ttu-id="58ab1-149">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="58ab1-149">Group.Read.All</span></span> | <span data-ttu-id="58ab1-150">非サポート</span><span class="sxs-lookup"><span data-stu-id="58ab1-150">Not supported</span></span> | <span data-ttu-id="58ab1-151">非サポート</span><span class="sxs-lookup"><span data-stu-id="58ab1-151">Not supported</span></span> |
| <span data-ttu-id="58ab1-152">グループ [post](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="58ab1-152">group [post](../resources/post.md)</span></span> | <span data-ttu-id="58ab1-153">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="58ab1-153">Group.Read.All</span></span> | <span data-ttu-id="58ab1-154">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="58ab1-154">Not supported</span></span> | <span data-ttu-id="58ab1-155">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="58ab1-155">Group.Read.All</span></span> |
| [<span data-ttu-id="58ab1-156">mailFolder</span><span class="sxs-lookup"><span data-stu-id="58ab1-156">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="58ab1-157">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="58ab1-157">Mail.Read</span></span> | <span data-ttu-id="58ab1-158">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="58ab1-158">Mail.Read</span></span> | <span data-ttu-id="58ab1-159">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="58ab1-159">Mail.Read</span></span> |
| [<span data-ttu-id="58ab1-160">message</span><span class="sxs-lookup"><span data-stu-id="58ab1-160">message</span></span>](../resources/message.md) | <span data-ttu-id="58ab1-161">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="58ab1-161">Mail.Read</span></span> | <span data-ttu-id="58ab1-162">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="58ab1-162">Mail.Read</span></span> | <span data-ttu-id="58ab1-163">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="58ab1-163">Mail.Read</span></span> |
| [<span data-ttu-id="58ab1-164">Outlook タスク</span><span class="sxs-lookup"><span data-stu-id="58ab1-164">Outlook task</span></span>](../resources/outlooktask.md) | <span data-ttu-id="58ab1-165">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="58ab1-165">Tasks.Read</span></span> | <span data-ttu-id="58ab1-166">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="58ab1-166">Tasks.Read</span></span> | <span data-ttu-id="58ab1-167">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="58ab1-167">Not supported</span></span> |
| [<span data-ttu-id="58ab1-168">Outlook タスク フォルダー</span><span class="sxs-lookup"><span data-stu-id="58ab1-168">Outlook task folder</span></span>](../resources/outlooktaskfolder.md) | <span data-ttu-id="58ab1-169">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="58ab1-169">Tasks.Read</span></span> | <span data-ttu-id="58ab1-170">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="58ab1-170">Tasks.Read</span></span> | <span data-ttu-id="58ab1-171">非サポート</span><span class="sxs-lookup"><span data-stu-id="58ab1-171">Not supported</span></span> |
 
## <a name="http-request"></a><span data-ttu-id="58ab1-172">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="58ab1-172">HTTP request</span></span>

<span data-ttu-id="58ab1-p103">**id** プロパティに対するフィルターと一致する拡張プロパティで展開された、リソース インスタンスを取得します。フィルター文字列内のスペース文字に [URL エンコード](https://www.w3schools.com/tags/ref_urlencode.asp)を適用していることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="58ab1-p103">Get a resource instance expanded with the extended property which matches a filter on the **id** property. Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the filter string.</span></span>

<span data-ttu-id="58ab1-175">**message** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="58ab1-175">Get a **message** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="58ab1-176">**mailFolder** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="58ab1-176">Get a **mailFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="58ab1-177">**event** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="58ab1-177">Get an **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="58ab1-178">**calendar** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="58ab1-178">Get a **calendar** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="58ab1-179">**contact** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="58ab1-179">Get a **contact** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="58ab1-180">**contactFolder** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="58ab1-180">Get a **contactFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="58ab1-181">**Outlooktask**インスタンスを取得します。</span><span class="sxs-lookup"><span data-stu-id="58ab1-181">Get an **outlookTask** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskFolders/{id}/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="58ab1-182">**Outlooktaskfolder**インスタンスを取得します。</span><span class="sxs-lookup"><span data-stu-id="58ab1-182">Get an **outlookTaskFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskGroups/{id}/taskFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="58ab1-183">グループ **event** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="58ab1-183">Get a group **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="58ab1-184">グループ **post** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="58ab1-184">Get a group **post** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

## <a name="path-parameters"></a><span data-ttu-id="58ab1-185">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="58ab1-185">Path parameters</span></span>
|<span data-ttu-id="58ab1-186">**パラメーター**</span><span class="sxs-lookup"><span data-stu-id="58ab1-186">**Parameter**</span></span>|<span data-ttu-id="58ab1-187">**型**</span><span class="sxs-lookup"><span data-stu-id="58ab1-187">**Type**</span></span>|<span data-ttu-id="58ab1-188">**説明**</span><span class="sxs-lookup"><span data-stu-id="58ab1-188">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="58ab1-189">id_value</span><span class="sxs-lookup"><span data-stu-id="58ab1-189">id_value</span></span>|<span data-ttu-id="58ab1-190">String</span><span class="sxs-lookup"><span data-stu-id="58ab1-190">String</span></span>|<span data-ttu-id="58ab1-p104">照合する拡張プロパティの ID。サポートされている形式のいずれかに従う必要があります。詳しくは、「[Outlook の拡張プロパティの概要](../resources/extended-properties-overview.md)」を参照してください。必須。</span><span class="sxs-lookup"><span data-stu-id="58ab1-p104">The ID of the extended property to match. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="58ab1-195">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="58ab1-195">Request headers</span></span>
| <span data-ttu-id="58ab1-196">名前</span><span class="sxs-lookup"><span data-stu-id="58ab1-196">Name</span></span>      |<span data-ttu-id="58ab1-197">説明</span><span class="sxs-lookup"><span data-stu-id="58ab1-197">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="58ab1-198">Authorization</span><span class="sxs-lookup"><span data-stu-id="58ab1-198">Authorization</span></span>  | <span data-ttu-id="58ab1-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="58ab1-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="58ab1-201">要求本文</span><span class="sxs-lookup"><span data-stu-id="58ab1-201">Request body</span></span>
<span data-ttu-id="58ab1-202">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="58ab1-202">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="58ab1-203">応答</span><span class="sxs-lookup"><span data-stu-id="58ab1-203">Response</span></span>

<span data-ttu-id="58ab1-204">成功した場合、このメソッドは `200 OK` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="58ab1-204">If successful, this method returns a `200 OK` response code.</span></span> 

<span data-ttu-id="58ab1-205">応答本文には、一致する [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) オブジェクトで展開された、要求したリソース インスタンスで表されるオブジェクトが含まれます。</span><span class="sxs-lookup"><span data-stu-id="58ab1-205">The response body includes an object representing the requested resource instance, expanded with the matching [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object.</span></span>

## <a name="example"></a><span data-ttu-id="58ab1-206">例</span><span class="sxs-lookup"><span data-stu-id="58ab1-206">Example</span></span>
##### <a name="request"></a><span data-ttu-id="58ab1-207">要求</span><span class="sxs-lookup"><span data-stu-id="58ab1-207">Request</span></span>
<span data-ttu-id="58ab1-p106">この例では、複数値の拡張プロパティを含めることで指定されたイベントを取得して展開します。フィルターは、**id** が文字列 `StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation` と一致する拡張プロパティを返します (ここでは、読みやすくするため URL エンコードを削除しています)。</span><span class="sxs-lookup"><span data-stu-id="58ab1-p106">This example gets and expands the specified event by including a multi-value extended property. The filter returns the extended property that has its **id** matching the string `StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation` (with URL encoding removed here for ease of reading).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/events('AAMkAGE1M2_bs88AACbuFiiAAA=')?$expand=multiValueExtendedProperties($filter=id%20eq%20'StringArray%20{66f5a359-4659-4830-9070-00050ec6ac6e}%20Name%20Recreation')
```
##### <a name="response"></a><span data-ttu-id="58ab1-210">応答</span><span class="sxs-lookup"><span data-stu-id="58ab1-210">Response</span></span>

<span data-ttu-id="58ab1-211">応答本文には、指定されたイベントのすべてのプロパティと、フィルターから返される拡張プロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="58ab1-211">The response body includes all the properties of the specified event and extended property returned from the filter.</span></span>

<span data-ttu-id="58ab1-p107">注:簡潔にするために、ここに示す**イベント** オブジェクトは切り詰められています。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="58ab1-p107">Note: The **event** object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Get multiValueLegacyExtendedProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
