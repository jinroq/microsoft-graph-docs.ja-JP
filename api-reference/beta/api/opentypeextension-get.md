---
title: オープン拡張機能を取得する
description: 名前または完全修飾名で識別されたオープン拡張機能 (openTypeExtension オブジェクト) を取得します。
ms.openlocfilehash: 599422384ed7e821f0ca50235fd164594bccd4d1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073427"
---
# <a name="get-open-extension"></a><span data-ttu-id="9a1a0-103">オープン拡張機能を取得する</span><span class="sxs-lookup"><span data-stu-id="9a1a0-103">Get open extension</span></span>

> <span data-ttu-id="9a1a0-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9a1a0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9a1a0-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9a1a0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9a1a0-106">名前または完全修飾名で識別されたオープン拡張機能 ([openTypeExtension](../resources/opentypeextension.md) オブジェクト) を取得します。</span><span class="sxs-lookup"><span data-stu-id="9a1a0-106">Get an open extension ([openTypeExtension](../resources/opentypeextension.md) object) identified by name or fully qualified name.</span></span>

<span data-ttu-id="9a1a0-107">次の表は、サポートされているリソース インスタンスからオープン拡張機能を取得できる 3 つのシナリオの一覧です。</span><span class="sxs-lookup"><span data-stu-id="9a1a0-107">The following table lists the three scenarios where you can get an open extension from a supported resource instance.</span></span>

|<span data-ttu-id="9a1a0-108">**GET シナリオ**</span><span class="sxs-lookup"><span data-stu-id="9a1a0-108">**GET scenario**</span></span>|<span data-ttu-id="9a1a0-109">**サポートされているリソース**</span><span class="sxs-lookup"><span data-stu-id="9a1a0-109">**Supported resources**</span></span>|<span data-ttu-id="9a1a0-110">**応答本文**</span><span class="sxs-lookup"><span data-stu-id="9a1a0-110">**Response body**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="9a1a0-111">既知のリソース インスタンスから特定の拡張機能を取得します。</span><span class="sxs-lookup"><span data-stu-id="9a1a0-111">Get a specific extension from a known resource instance.</span></span>| <span data-ttu-id="9a1a0-112">[ユニットの管理](../resources/administrativeunit.md)、[デバイス](../resources/device.md)、[イベント](../resources/event.md)、[グループ](../resources/group.md)[グループのイベント](../resources/event.md)[グループの投稿](../resources/post.md)、[メッセージ](../resources/message.md)、[組織](../resources/organization.md)、[個人の連絡先](../resources/contact.md)、[ユーザー](../resources/user.md)</span><span class="sxs-lookup"><span data-stu-id="9a1a0-112">[Administrative unit](../resources/administrativeunit.md), [device](../resources/device.md), [event](../resources/event.md), [group](../resources/group.md), [group event](../resources/event.md), [group post](../resources/post.md), [message](../resources/message.md), [organization](../resources/organization.md), [personal contact](../resources/contact.md), [user](../resources/user.md)</span></span> | <span data-ttu-id="9a1a0-113">オープン拡張機能のみ。</span><span class="sxs-lookup"><span data-stu-id="9a1a0-113">Open extension only.</span></span>|
|<span data-ttu-id="9a1a0-114">特定の拡張機能で展開された既知のリソース インスタンスを取得します。</span><span class="sxs-lookup"><span data-stu-id="9a1a0-114">Get a known resource instance expanded with a specific extension.</span></span>|<span data-ttu-id="9a1a0-115">単位の管理、デバイス、イベント、グループ、グループのイベント、グループの投稿、メッセージ、組織、個人の連絡先、ユーザー</span><span class="sxs-lookup"><span data-stu-id="9a1a0-115">Administrative unit, device, event, group, group event, group post, message, organization, personal contact, user</span></span> |<span data-ttu-id="9a1a0-116">オープン拡張機能で展開されたリソース インスタンス。</span><span class="sxs-lookup"><span data-stu-id="9a1a0-116">A resource instance expanded with the open extension.</span></span>|
|<span data-ttu-id="9a1a0-117">特定の拡張機能でリソース インスタンスを検索し、展開します。</span><span class="sxs-lookup"><span data-stu-id="9a1a0-117">Find and expand resource instances with a specific extension.</span></span> | <span data-ttu-id="9a1a0-118">イベント、グループ イベント、グループの投稿、メッセージ、個人用連絡先</span><span class="sxs-lookup"><span data-stu-id="9a1a0-118">Event, group event, group post, message, personal contact</span></span> |<span data-ttu-id="9a1a0-119">オープン拡張機能で展開されたリソース インスタンス。</span><span class="sxs-lookup"><span data-stu-id="9a1a0-119">Resource instances expanded with the open extension.</span></span>|

## <a name="permissions"></a><span data-ttu-id="9a1a0-120">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9a1a0-120">Permissions</span></span>

<span data-ttu-id="9a1a0-121">拡張機能とアクセス許可が含まれるリソースによって委任された (アプリケーション) の種類を要求、次の表で指定されたアクセス許可は、この API を呼び出すために必要最低限の特権。</span><span class="sxs-lookup"><span data-stu-id="9a1a0-121">Depending on the resource that contains the extension and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="9a1a0-122">アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9a1a0-122">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9a1a0-123">サポートされているリソース</span><span class="sxs-lookup"><span data-stu-id="9a1a0-123">Supported resource</span></span> | <span data-ttu-id="9a1a0-124">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9a1a0-124">Delegated (work or school account)</span></span> | <span data-ttu-id="9a1a0-125">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9a1a0-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a1a0-126">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9a1a0-126">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="9a1a0-127">device</span><span class="sxs-lookup"><span data-stu-id="9a1a0-127">device</span></span>](../resources/device.md) | <span data-ttu-id="9a1a0-128">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="9a1a0-128">Directory.Read.All</span></span> | <span data-ttu-id="9a1a0-129">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="9a1a0-129">Not supported</span></span> | <span data-ttu-id="9a1a0-130">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a1a0-130">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="9a1a0-131">イベント</span><span class="sxs-lookup"><span data-stu-id="9a1a0-131">event</span></span>](../resources/event.md) | <span data-ttu-id="9a1a0-132">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="9a1a0-132">Calendars.Read</span></span> | <span data-ttu-id="9a1a0-133">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="9a1a0-133">Calendars.Read</span></span> | <span data-ttu-id="9a1a0-134">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="9a1a0-134">Calendars.Read</span></span> |
| [<span data-ttu-id="9a1a0-135">group</span><span class="sxs-lookup"><span data-stu-id="9a1a0-135">group</span></span>](../resources/group.md) | <span data-ttu-id="9a1a0-136">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="9a1a0-136">Group.Read.All</span></span> | <span data-ttu-id="9a1a0-137">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="9a1a0-137">Not supported</span></span> | <span data-ttu-id="9a1a0-138">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="9a1a0-138">Group.Read.All</span></span> |
| [<span data-ttu-id="9a1a0-139">グループ イベント</span><span class="sxs-lookup"><span data-stu-id="9a1a0-139">group event</span></span>](../resources/event.md) | <span data-ttu-id="9a1a0-140">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="9a1a0-140">Group.Read.All</span></span> | <span data-ttu-id="9a1a0-141">使用不可</span><span class="sxs-lookup"><span data-stu-id="9a1a0-141">Not supported</span></span> | <span data-ttu-id="9a1a0-142">使用不可</span><span class="sxs-lookup"><span data-stu-id="9a1a0-142">Not supported</span></span> |
| [<span data-ttu-id="9a1a0-143">グループの投稿</span><span class="sxs-lookup"><span data-stu-id="9a1a0-143">group post</span></span>](../resources/post.md) | <span data-ttu-id="9a1a0-144">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="9a1a0-144">Group.Read.All</span></span> | <span data-ttu-id="9a1a0-145">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="9a1a0-145">Not supported</span></span> | <span data-ttu-id="9a1a0-146">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="9a1a0-146">Group.Read.All</span></span> |
| [<span data-ttu-id="9a1a0-147">message</span><span class="sxs-lookup"><span data-stu-id="9a1a0-147">message</span></span>](../resources/message.md) | <span data-ttu-id="9a1a0-148">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="9a1a0-148">Mail.Read</span></span> | <span data-ttu-id="9a1a0-149">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="9a1a0-149">Mail.Read</span></span> | <span data-ttu-id="9a1a0-150">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="9a1a0-150">Mail.Read</span></span> | 
| [<span data-ttu-id="9a1a0-151">organization</span><span class="sxs-lookup"><span data-stu-id="9a1a0-151">organization</span></span>](../resources/organization.md) | <span data-ttu-id="9a1a0-152">User.Read</span><span class="sxs-lookup"><span data-stu-id="9a1a0-152">User.Read</span></span> | <span data-ttu-id="9a1a0-153">使用不可</span><span class="sxs-lookup"><span data-stu-id="9a1a0-153">Not supported</span></span> | <span data-ttu-id="9a1a0-154">使用不可</span><span class="sxs-lookup"><span data-stu-id="9a1a0-154">Not supported</span></span> |
| [<span data-ttu-id="9a1a0-155">個人用連絡先</span><span class="sxs-lookup"><span data-stu-id="9a1a0-155">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="9a1a0-156">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="9a1a0-156">Contacts.Read</span></span> | <span data-ttu-id="9a1a0-157">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="9a1a0-157">Contacts.Read</span></span> | <span data-ttu-id="9a1a0-158">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="9a1a0-158">Contacts.Read</span></span> |
| [<span data-ttu-id="9a1a0-159">user</span><span class="sxs-lookup"><span data-stu-id="9a1a0-159">user</span></span>](../resources/user.md) | <span data-ttu-id="9a1a0-160">User.Read</span><span class="sxs-lookup"><span data-stu-id="9a1a0-160">User.Read</span></span> | <span data-ttu-id="9a1a0-161">User.Read</span><span class="sxs-lookup"><span data-stu-id="9a1a0-161">User.Read</span></span> | <span data-ttu-id="9a1a0-162">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="9a1a0-162">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a1a0-163">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9a1a0-163">HTTP request</span></span>

<span data-ttu-id="9a1a0-164">このセクションでは、前述の 3 つの `GET` シナリオの構文について説明します。</span><span class="sxs-lookup"><span data-stu-id="9a1a0-164">This section lists the syntax for each of the three `GET` scenarios described above.</span></span>

### <a name="get-a-specific-extension-in-a-known-resource-instance"></a><span data-ttu-id="9a1a0-165">既知のリソース インスタンス内の特定の拡張機能を取得する</span><span class="sxs-lookup"><span data-stu-id="9a1a0-165">Get a specific extension in a known resource instance</span></span>

<span data-ttu-id="9a1a0-166">リソース インスタンスを取得するのと同じ REST 要求を使用し、そのインスタンスの **extensions** ナビゲーション プロパティを使用して拡張機能を識別します。</span><span class="sxs-lookup"><span data-stu-id="9a1a0-166">Use the same REST request as getting the resource instance, and identify the extension using the **extensions** navigation property of that instance.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /administrativeUnits/{Id}/extensions/{extensionId}
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

### <a name="get-a-known-resource-instance-expanded-with-a-matching-extension"></a><span data-ttu-id="9a1a0-167">一致する拡張機能で展開された既知のリソース インスタンスを取得する</span><span class="sxs-lookup"><span data-stu-id="9a1a0-167">Get a known resource instance expanded with a matching extension</span></span> 

<span data-ttu-id="9a1a0-p103">イベント、グループ イベント、グループの投稿、メッセージ、個人用連絡先のリソースの種類に関しては、リソース インスタンスを取得するのと同じ REST 要求を使用して、そのインスタンスの **id** プロパティのフィルターに一致する拡張機能を検索し、拡張機能でインスタンスを展開できます。応答には、リソース プロパティのほとんどが含まれています。</span><span class="sxs-lookup"><span data-stu-id="9a1a0-p103">For the event, group event, group post, message, personal contact resource types, you can use the same REST request as getting the resource instance, look for an extension that matches a filter on its **id** property, and expand the instance with the extension. The response includes most of the resource properties.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Id|userPrincipalName}/events/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /groups/{Id}/events/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /groups/{Id}/threads/{Id}/posts/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/messages/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/contacts/{Id}?$expand=extensions($filter=id eq '{extensionId}')
```


<span data-ttu-id="9a1a0-170">デバイス、グループ、組織、ユーザーのリソースの種類に関しては、リソース インスタンスから **id** プロパティやその他のプロパティを含めるために、`$select` パラメーターを使用する必要もあります。</span><span class="sxs-lookup"><span data-stu-id="9a1a0-170">For the device, group, organization, and user resource types, you must also use a `$select` parameter to include the **id** property and any other properties you want from the resource instance:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /devices/{Id}?$expand=extensions($filter=id eq '{extensionId}')&$select=id,{property_1},{property_n}
GET /groups/{Id}?$expand=extensions($filter=id eq '{extensionId}')&$select=id,{property_1},{property_n}
GET /organization/{Id}?$expand=extensions($filter=id eq '{extensionId}')&$select=id,{property_1},{property_n}
GET /users/{Id|userPrincipalName}?$expand=extensions($filter=id eq '{extensionId}')&$select=id,{property_1},{property_n}
```


### <a name="filter-for-resource-instances-expanded-with-a-matching-extension"></a><span data-ttu-id="9a1a0-171">一致する拡張機能で展開されたリソース インスタンスにフィルターをかける</span><span class="sxs-lookup"><span data-stu-id="9a1a0-171">Filter for resource instances expanded with a matching extension</span></span> 

<span data-ttu-id="9a1a0-172">サポートされているリソースのコレクションを取得するのと同じ REST 要求を使用して、対応する **id** プロパティの拡張機能を含むインスタンスのコレクションにフィルターをかけ、拡張機能でこれらのインスタンスを展開します。</span><span class="sxs-lookup"><span data-stu-id="9a1a0-172">Use the same REST request as getting a collection of the supported resource, filter the collection for instances that contain an extension with a matching **id** property, and expand these instances with the extension.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Id|userPrincipalName}/events?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
GET /groups/{Id}/events?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
GET /groups/{Id}/threads/{Id}/posts?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/messages?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/contacts?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
```

><span data-ttu-id="9a1a0-p104">**注:** 上記の構文は、拡張機能の取得元となるリソース インスタンスまたはコレクションを特定する一般的な方法を示しています。こうしたリソース インスタンスまたはコレクションを特定するために使用できる他の構文すべても、同様の方法でオープン拡張機能を取得できます。</span><span class="sxs-lookup"><span data-stu-id="9a1a0-p104">**Note:** The above syntax shows some common ways to identify a resource instance or collection, in order to get an extension from it. All other syntax that allows you to identify these resource instances or collections supports getting open extensions from them in a similar way.</span></span>


## <a name="path-parameters"></a><span data-ttu-id="9a1a0-175">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="9a1a0-175">Path parameters</span></span>
|<span data-ttu-id="9a1a0-176">**パラメーター**</span><span class="sxs-lookup"><span data-stu-id="9a1a0-176">**Parameter**</span></span>|<span data-ttu-id="9a1a0-177">**型**</span><span class="sxs-lookup"><span data-stu-id="9a1a0-177">**Type**</span></span>|<span data-ttu-id="9a1a0-178">**説明**</span><span class="sxs-lookup"><span data-stu-id="9a1a0-178">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="9a1a0-179">Id</span><span class="sxs-lookup"><span data-stu-id="9a1a0-179">Id</span></span>|<span data-ttu-id="9a1a0-180">文字列</span><span class="sxs-lookup"><span data-stu-id="9a1a0-180">string</span></span>|<span data-ttu-id="9a1a0-p105">メッセージ、イベント、連絡先などの対応するコレクションに含まれるオブジェクトの一意識別子を格納するプレースホルダー。必須。**openTypeExtension** の **id** プロパティと混同しないこと。</span><span class="sxs-lookup"><span data-stu-id="9a1a0-p105">Placeholder for a unique identifier for an object in the corresponding collection such as messages, events, contacts. Required. Not to be confused with the **id** property of an **openTypeExtension**.</span></span>|
|<span data-ttu-id="9a1a0-184">extensionId</span><span class="sxs-lookup"><span data-stu-id="9a1a0-184">extensionId</span></span>|<span data-ttu-id="9a1a0-185">文字列</span><span class="sxs-lookup"><span data-stu-id="9a1a0-185">string</span></span>|<span data-ttu-id="9a1a0-p106">拡張情報名を表すプレースホルダー。これは、拡張情報の一意のテキスト識別子であるか、拡張情報の種類と一意のテキスト識別子を連結した完全修飾名のいずれかです。完全修飾名は、拡張情報の作成時に **id** プロパティに入れて返されます。必須。</span><span class="sxs-lookup"><span data-stu-id="9a1a0-p106">Placeholder for an extension name which is a unique text identifier for an extension, or a fully qualified name which concatenates the extension type and unique text identifier. The fully qualified name is returned in the **id** property when you create the extension. Required.</span></span>|

## <a name="optional-query-parameters"></a><span data-ttu-id="9a1a0-189">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="9a1a0-189">Optional query parameters</span></span>

<span data-ttu-id="9a1a0-190">`$filter` 文字列内のスペース文字には必ず [URL エンコード](https://www.w3schools.com/tags/ref_urlencode.asp)を適用してください。</span><span class="sxs-lookup"><span data-stu-id="9a1a0-190">Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the `$filter` string.</span></span>

|<span data-ttu-id="9a1a0-191">**名前**</span><span class="sxs-lookup"><span data-stu-id="9a1a0-191">**Name**</span></span>|<span data-ttu-id="9a1a0-192">**値**</span><span class="sxs-lookup"><span data-stu-id="9a1a0-192">**Value**</span></span>|<span data-ttu-id="9a1a0-193">**説明**</span><span class="sxs-lookup"><span data-stu-id="9a1a0-193">**Description**</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="9a1a0-194">$filter</span><span class="sxs-lookup"><span data-stu-id="9a1a0-194">$filter</span></span>|<span data-ttu-id="9a1a0-195">文字列</span><span class="sxs-lookup"><span data-stu-id="9a1a0-195">string</span></span>|<span data-ttu-id="9a1a0-196">**id** が `extensionId` パラメーターの値と一致する拡張情報を返します。</span><span class="sxs-lookup"><span data-stu-id="9a1a0-196">Returns an extension with its **id** matching the `extensionId` parameter value.</span></span>|
|<span data-ttu-id="9a1a0-197">$filter with **any** operator</span><span class="sxs-lookup"><span data-stu-id="9a1a0-197">$filter with **any** operator</span></span>|<span data-ttu-id="9a1a0-198">文字列</span><span class="sxs-lookup"><span data-stu-id="9a1a0-198">string</span></span>|<span data-ttu-id="9a1a0-199">**id** が `extensionId` パラメーターの値と一致する拡張情報を含むリソース コレクションのインスタンスを返します。</span><span class="sxs-lookup"><span data-stu-id="9a1a0-199">Returns instances of a resource collection that contain an extension with its **id** matching the `extensionId` parameter value.</span></span>|
|<span data-ttu-id="9a1a0-200">$expand</span><span class="sxs-lookup"><span data-stu-id="9a1a0-200">$expand</span></span>|<span data-ttu-id="9a1a0-201">文字列</span><span class="sxs-lookup"><span data-stu-id="9a1a0-201">string</span></span>|<span data-ttu-id="9a1a0-202">リソース インスタンスを展開して、拡張情報を組み込みます。</span><span class="sxs-lookup"><span data-stu-id="9a1a0-202">Expands a resource instance to include an extension.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="9a1a0-203">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9a1a0-203">Request headers</span></span>
| <span data-ttu-id="9a1a0-204">名前</span><span class="sxs-lookup"><span data-stu-id="9a1a0-204">Name</span></span>       | <span data-ttu-id="9a1a0-205">値</span><span class="sxs-lookup"><span data-stu-id="9a1a0-205">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="9a1a0-206">Authorization</span><span class="sxs-lookup"><span data-stu-id="9a1a0-206">Authorization</span></span> | <span data-ttu-id="9a1a0-p107">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9a1a0-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9a1a0-209">要求本文</span><span class="sxs-lookup"><span data-stu-id="9a1a0-209">Request body</span></span>
<span data-ttu-id="9a1a0-210">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="9a1a0-210">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9a1a0-211">応答</span><span class="sxs-lookup"><span data-stu-id="9a1a0-211">Response</span></span>

<span data-ttu-id="9a1a0-p108">成功した場合、このメソッドは応答本文で `200 OK` 応答コードと [openTypeExtension](../resources/opentypeextension.md) オブジェクトを返します。GET クエリに応じて、厳密な応答の本体は異なります。</span><span class="sxs-lookup"><span data-stu-id="9a1a0-p108">If successful, this method returns a `200 OK` response code and [openTypeExtension](../resources/opentypeextension.md) object in the response body. Depending on the GET query, the exact response body differs.</span></span>
## <a name="example"></a><span data-ttu-id="9a1a0-214">例</span><span class="sxs-lookup"><span data-stu-id="9a1a0-214">Example</span></span>

#### <a name="request-1"></a><span data-ttu-id="9a1a0-215">要求 1</span><span class="sxs-lookup"><span data-stu-id="9a1a0-215">Request 1</span></span>

<span data-ttu-id="9a1a0-p109">最初の例では、拡張情報を参照する 2 通りの方法を示し、指定されたメッセージ内の拡張情報を取得します。応答は、拡張情報を参照するために使用する方法に関係なく、同じです。</span><span class="sxs-lookup"><span data-stu-id="9a1a0-p109">The first example shows 2 ways of referencing an extension and gets the extension in the specified message. The response is the same regardless of the way used to reference the extension.</span></span>

<span data-ttu-id="9a1a0-218">最初は、名前で参照します。</span><span class="sxs-lookup"><span data-stu-id="9a1a0-218">First, by its name:</span></span> 

<!-- {
  "blockType": "request",
  "name": "get_opentypeextension_1"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions('Com.Contoso.Referral')
```

<span data-ttu-id="9a1a0-219">次に、ID (完全修飾名) で参照します。</span><span class="sxs-lookup"><span data-stu-id="9a1a0-219">Second, by its ID (fully qualified name):</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')
```

#### <a name="response-1"></a><span data-ttu-id="9a1a0-220">応答 1</span><span class="sxs-lookup"><span data-stu-id="9a1a0-220">Response 1</span></span>
<span data-ttu-id="9a1a0-221">最初の例の応答を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9a1a0-221">Here is the response for the first example.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.opentypeextension"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions/$entity",
    "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
    "@odata.id": "https://graph.microsoft.com/beta/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions
('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
    "extensionName": "Com.Contoso.Referral",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
    "companyName": "Wingtip Toys",
    "dealValue": 500050,
    "expirationDate": "2015-12-03T10:00:00Z"
}
```

****


#### <a name="request-2"></a><span data-ttu-id="9a1a0-222">要求 2</span><span class="sxs-lookup"><span data-stu-id="9a1a0-222">Request 2</span></span>

<span data-ttu-id="9a1a0-223">2 番目の例では、名前で拡張情報を参照し、指定されたグループ イベント内の拡張情報を取得します。</span><span class="sxs-lookup"><span data-stu-id="9a1a0-223">The second example references an extension by its name and gets the extension in the specified group event.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_opentypeextension_2"
}-->
```http
GET https://graph.microsoft.com/beta/groups('f5480dfd-7d77-4d0b-ba2e-3391953cc74a')/events('AAMkADVl17IsAAA=')/extensions('Com.Contoso.Deal') 
```

#### <a name="response-2"></a><span data-ttu-id="9a1a0-224">応答 2</span><span class="sxs-lookup"><span data-stu-id="9a1a0-224">Response 2</span></span>

<span data-ttu-id="9a1a0-225">2 番目の例の応答を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9a1a0-225">Here is the response from the second example.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.opentypeextension"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups('f5480dfd-7d77-4d0b-ba2e-3391953cc74a')/events('AAMkADVl7IsAAA%3D')/extensions/$entity",
    "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Deal",
    "extensionName": "Com.Contoso.Deal",
    "companyName": "Alpine Skis",
    "dealValue": 1010100,
    "expirationDate": "2015-07-03T13:04:00Z"
}
```

****

#### <a name="request-3"></a><span data-ttu-id="9a1a0-226">要求 3</span><span class="sxs-lookup"><span data-stu-id="9a1a0-226">Request 3</span></span>

<span data-ttu-id="9a1a0-p110">3 番目の例では、指定されたメッセージを取得し、フィルターから返された拡張情報を組み込んで展開します。このフィルターは、**id** が完全修飾名と一致する拡張情報を返します。</span><span class="sxs-lookup"><span data-stu-id="9a1a0-p110">The third example gets and expands the specified message by including the extension returned from a filter. The filter returns the extension that has its **id** matching a fully qualified name.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_opentypeextension_3"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')?$expand=extensions($filter=id%20eq%20'Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')
```


#### <a name="response-3"></a><span data-ttu-id="9a1a0-229">応答 3</span><span class="sxs-lookup"><span data-stu-id="9a1a0-229">Response 3</span></span>

<span data-ttu-id="9a1a0-p111">3 番目の例の応答を次に示します。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="9a1a0-p111">And here is the response from the third example. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
    "@odata.id": "https://graph.microsoft.com/beta/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')",
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
    "extensions@odata.context": "https://graph.microsoft.com/beta/$metadata#users('desmond40contoso.com')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions", 
    "extensions": [ 
      { 
        "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
        "@odata.id": "https://graph.microsoft.com/beta/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
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

#### <a name="request-4"></a><span data-ttu-id="9a1a0-233">要求 4</span><span class="sxs-lookup"><span data-stu-id="9a1a0-233">Request 4</span></span>

<span data-ttu-id="9a1a0-234">4 番目の例では、完全修飾名で拡張情報を参照し、指定されたグループ投稿内の拡張情報を取得します。</span><span class="sxs-lookup"><span data-stu-id="9a1a0-234">The fourth example references an extension by its fully qualified name and gets the extension in the specified group post.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_opentypeextension_4"
}-->
```http
GET https://graph.microsoft.com/beta/groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/threads('AAQkADJizZJpEWwqDHsEpV_KA==')/posts('AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA=')/extensions('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate') 
```

#### <a name="response-4"></a><span data-ttu-id="9a1a0-235">応答 4</span><span class="sxs-lookup"><span data-stu-id="9a1a0-235">Response 4</span></span>

<span data-ttu-id="9a1a0-236">4 番目の例の応答を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9a1a0-236">Here is the response from the fourth example.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.opentypeextension"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/threads('AAQkADJizZJpEWwqDHsEpV_KA%3D%3D')/posts('AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA%3D')/extensions/$entity",
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


#### <a name="request-5"></a><span data-ttu-id="9a1a0-237">要求 5</span><span class="sxs-lookup"><span data-stu-id="9a1a0-237">Request 5</span></span>

<span data-ttu-id="9a1a0-p112">5 番目の例では、サインインしているユーザーのメールボックス内のすべてのメッセージを参照して、フィルターと一致する拡張情報が含まれているメッセージを検出し、拡張情報を組み込んでそれらのメッセージを展開します。このフィルターは、拡張情報名 `Com.Contoso.Referral` と一致する **id** プロパティを持つ拡張情報を返します。</span><span class="sxs-lookup"><span data-stu-id="9a1a0-p112">The fifth example looks at all messages in the signed-in user's mailbox to find those that contain an extension matching a filter, and expands them by including the extension. The filter returns extensions that has the **id** property matching the extension name `Com.Contoso.Referral`.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_opentypeextension_5"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages?$filter=Extensions/any(f:f/id%20eq%20'Com.Contoso.Referral')&$expand=Extensions($filter=id%20eq%20'Com.Contoso.Referral')
```


####<a name="response-5"></a><span data-ttu-id="9a1a0-240">応答 5</span><span class="sxs-lookup"><span data-stu-id="9a1a0-240">Response 5</span></span>

<span data-ttu-id="9a1a0-241">5 番目の例のこの応答では、**id** が `Com.Contoso.Referral` である拡張情報が含まれているメッセージがユーザーのメールボックスに 1 つだけ存在します。</span><span class="sxs-lookup"><span data-stu-id="9a1a0-241">In this response for the fifth example, there is only one message in the user's mailbox that has an extension with its **id** equal to `Com.Contoso.Referral`.</span></span>

<span data-ttu-id="9a1a0-p113">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="9a1a0-p113">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages",
  "value": [
  {

    "@odata.id": "https://graph.microsoft.com/beta/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')",
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
    "extensions@odata.context": "https://graph.microsoft.com/beta/$metadata#users('desmond40contoso.com')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions", 
    "extensions": [ 
      { 
        "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
        "@odata.id": "https://graph.microsoft.com/beta/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
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
  "tocPath": ""
}-->