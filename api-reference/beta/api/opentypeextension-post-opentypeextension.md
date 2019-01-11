---
title: オープン拡張機能を作成する
description: オープン拡張機能 (openTypeExtension オブジェクト) を作成し、カスタム プロパティを追加
localization_priority: Normal
ms.openlocfilehash: 363bd629b5b7c9041f36ce039403717f715e202c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863036"
---
# <a name="create-open-extension"></a><span data-ttu-id="5a9f3-103">オープン拡張機能を作成する</span><span class="sxs-lookup"><span data-stu-id="5a9f3-103">Create open extension</span></span>

> <span data-ttu-id="5a9f3-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5a9f3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5a9f3-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5a9f3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5a9f3-106">オープン拡張機能 ([openTypeExtension](../resources/opentypeextension.md)オブジェクト) を作成し、新規または既存のインスタンスは、サポートされているリソースのカスタム プロパティを追加します。</span><span class="sxs-lookup"><span data-stu-id="5a9f3-106">Create an open extension ([openTypeExtension](../resources/opentypeextension.md) object) and add custom properties in a new or existing instance of a supported resource.</span></span>

> <span data-ttu-id="5a9f3-107">**注:** Outlook のリソースを開いている拡張機能を作成する場合は、 [openTypeExtension のリソースの種類](../resources/opentypeextension.md#outlook-specific-considerations)の**Outlook に固有の考慮事項**を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5a9f3-107">**Note:** If you're creating open extensions on Outlook resources, see **Outlook-specific considerations** in [openTypeExtension resource type](../resources/opentypeextension.md#outlook-specific-considerations).</span></span>

## <a name="permissions"></a><span data-ttu-id="5a9f3-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="5a9f3-108">Permissions</span></span>

<span data-ttu-id="5a9f3-109">拡張機能を作成するリソースとアクセス許可によって委任された (アプリケーション) の種類を要求、次の表で指定されたアクセス許可は、この API を呼び出すために必要最低限の特権。</span><span class="sxs-lookup"><span data-stu-id="5a9f3-109">Depending on the resource you're creating the extension in and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="5a9f3-110">アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5a9f3-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5a9f3-111">サポートされているリソース</span><span class="sxs-lookup"><span data-stu-id="5a9f3-111">Supported resource</span></span> | <span data-ttu-id="5a9f3-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5a9f3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5a9f3-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5a9f3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5a9f3-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5a9f3-114">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="5a9f3-115">device</span><span class="sxs-lookup"><span data-stu-id="5a9f3-115">device</span></span>](../resources/device.md) | <span data-ttu-id="5a9f3-116">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5a9f3-116">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="5a9f3-117">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="5a9f3-117">Not supported</span></span> | <span data-ttu-id="5a9f3-118">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a9f3-118">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="5a9f3-119">イベント</span><span class="sxs-lookup"><span data-stu-id="5a9f3-119">event</span></span>](../resources/event.md) | <span data-ttu-id="5a9f3-120">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a9f3-120">Calendars.ReadWrite</span></span> | <span data-ttu-id="5a9f3-121">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a9f3-121">Calendars.ReadWrite</span></span> | <span data-ttu-id="5a9f3-122">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a9f3-122">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="5a9f3-123">グループ</span><span class="sxs-lookup"><span data-stu-id="5a9f3-123">group</span></span>](../resources/group.md) | <span data-ttu-id="5a9f3-124">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a9f3-124">Group.ReadWrite.All</span></span> | <span data-ttu-id="5a9f3-125">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="5a9f3-125">Not supported</span></span> | <span data-ttu-id="5a9f3-126">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a9f3-126">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="5a9f3-127">グループ イベント</span><span class="sxs-lookup"><span data-stu-id="5a9f3-127">group event</span></span>](../resources/event.md) | <span data-ttu-id="5a9f3-128">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a9f3-128">Group.ReadWrite.All</span></span> | <span data-ttu-id="5a9f3-129">使用不可</span><span class="sxs-lookup"><span data-stu-id="5a9f3-129">Not supported</span></span> | <span data-ttu-id="5a9f3-130">使用不可</span><span class="sxs-lookup"><span data-stu-id="5a9f3-130">Not supported</span></span> |
| [<span data-ttu-id="5a9f3-131">グループの投稿</span><span class="sxs-lookup"><span data-stu-id="5a9f3-131">group post</span></span>](../resources/post.md) | <span data-ttu-id="5a9f3-132">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a9f3-132">Group.ReadWrite.All</span></span> | <span data-ttu-id="5a9f3-133">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="5a9f3-133">Not supported</span></span> | <span data-ttu-id="5a9f3-134">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a9f3-134">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="5a9f3-135">メッセージ</span><span class="sxs-lookup"><span data-stu-id="5a9f3-135">message</span></span>](../resources/message.md) | <span data-ttu-id="5a9f3-136">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a9f3-136">Mail.ReadWrite</span></span> | <span data-ttu-id="5a9f3-137">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a9f3-137">Mail.ReadWrite</span></span> | <span data-ttu-id="5a9f3-138">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a9f3-138">Mail.ReadWrite</span></span> | 
| [<span data-ttu-id="5a9f3-139">組織</span><span class="sxs-lookup"><span data-stu-id="5a9f3-139">organization</span></span>](../resources/organization.md) | <span data-ttu-id="5a9f3-140">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5a9f3-140">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="5a9f3-141">使用不可</span><span class="sxs-lookup"><span data-stu-id="5a9f3-141">Not supported</span></span> | <span data-ttu-id="5a9f3-142">使用不可</span><span class="sxs-lookup"><span data-stu-id="5a9f3-142">Not supported</span></span> |
| [<span data-ttu-id="5a9f3-143">個人用連絡先</span><span class="sxs-lookup"><span data-stu-id="5a9f3-143">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="5a9f3-144">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a9f3-144">Contacts.ReadWrite</span></span> | <span data-ttu-id="5a9f3-145">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a9f3-145">Contacts.ReadWrite</span></span> | <span data-ttu-id="5a9f3-146">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a9f3-146">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="5a9f3-147">ユーザー</span><span class="sxs-lookup"><span data-stu-id="5a9f3-147">user</span></span>](../resources/user.md) | <span data-ttu-id="5a9f3-148">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a9f3-148">User.ReadWrite.All</span></span> | <span data-ttu-id="5a9f3-149">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a9f3-149">User.ReadWrite</span></span> | <span data-ttu-id="5a9f3-150">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a9f3-150">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5a9f3-151">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5a9f3-151">HTTP request</span></span>

### <a name="create-an-extension-in-a-new-resource-instance"></a><span data-ttu-id="5a9f3-152">新規のリソース インスタンスに拡張機能を作成する</span><span class="sxs-lookup"><span data-stu-id="5a9f3-152">Create an extension in a new resource instance</span></span>

<span data-ttu-id="5a9f3-153">インスタンスを作成するために使用同じ残りの要求を使用します。</span><span class="sxs-lookup"><span data-stu-id="5a9f3-153">Use the same REST request that you use to create the instance.</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/events
POST /users/{id|userPrincipalName}/messages
POST /groups/{id}/events
POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /users/{id|userPrincipalName}/contacts
```

><span data-ttu-id="5a9f3-154">**注:** この構文は、サポートされているリソースのインスタンスを作成する一般的な方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="5a9f3-154">**Note:** This syntax shows some common ways to create the supported resource instances.</span></span> <span data-ttu-id="5a9f3-155">これらのリソースのインスタンスを作成することを可能にするその他のすべてのポスト構文には、同様の方法でに開いている拡張機能の作成がサポートされています。</span><span class="sxs-lookup"><span data-stu-id="5a9f3-155">All other POST syntaxes that allows you to create these resource instances supports creating open extensions in them in a similar way.</span></span>

<span data-ttu-id="5a9f3-156">要求本文に、新規のリソース インスタンスのプロパティおよび_拡張機能_を含める方法については、[要求本文](#request-body)のセクションをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="5a9f3-156">See the [Request body](#request-body) section about including the properties of the new resource instance _and the extension_ in the request body.</span></span>

### <a name="create-an-extension-in-an-existing-resource-instance"></a><span data-ttu-id="5a9f3-157">既存のリソース インスタンスに拡張機能を作成する</span><span class="sxs-lookup"><span data-stu-id="5a9f3-157">Create an extension in an existing resource instance</span></span>

<span data-ttu-id="5a9f3-158">要求でリソース インスタンスを識別し、**extensions** ナビゲーション プロパティで `POST` を行います。</span><span class="sxs-lookup"><span data-stu-id="5a9f3-158">Identify the resource instance in the request and do a `POST` to the **extensions** navigation property.</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /administrativeunits/{id}/extensions
POST /devices/{id}/extensions
POST /users/{id|userPrincipalName}/events/{id}/extensions
POST /groups/{id}/extensions
POST /groups/{id}/events/{id}/extensions
POST /groups/{id}/threads/{id}/posts/{id}/extensions
POST /users/{id|userPrincipalName}/messages/{id}/extensions
POST /organization/{id}/extensions
POST /users/{id|userPrincipalName}/contacts/{id}/extensions
POST /users/{id|userPrincipalName}/extensions
```

><span data-ttu-id="5a9f3-159">**注:** この構文は、その中の拡張機能を作成するために、リソースのインスタンスを識別する一般的な方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="5a9f3-159">**Note:** This syntax shows some common ways to identify a resource instance, in order to create an extension in it.</span></span> <span data-ttu-id="5a9f3-160">同様の方法で開いている拡張機能を作成するこれらのリソースのインスタンスを識別することができるその他のすべての構文をサポートします。</span><span class="sxs-lookup"><span data-stu-id="5a9f3-160">All other syntaxes that allows you to identify these resource instances supports creating open extensions in them in a similar way.</span></span>

<span data-ttu-id="5a9f3-161">要求本文に_拡張機能_を含める方法については、[要求本文](#request-body)のセクションをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="5a9f3-161">See the [Request body](#request-body) section about including _the extension_ in the request body.</span></span>

## <a name="path-parameters"></a><span data-ttu-id="5a9f3-162">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="5a9f3-162">Path parameters</span></span>

|<span data-ttu-id="5a9f3-163">**パラメーター**</span><span class="sxs-lookup"><span data-stu-id="5a9f3-163">**Parameter**</span></span>|<span data-ttu-id="5a9f3-164">**型**</span><span class="sxs-lookup"><span data-stu-id="5a9f3-164">**Type**</span></span>|<span data-ttu-id="5a9f3-165">**説明**</span><span class="sxs-lookup"><span data-stu-id="5a9f3-165">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="5a9f3-166">ID</span><span class="sxs-lookup"><span data-stu-id="5a9f3-166">id</span></span>|<span data-ttu-id="5a9f3-167">文字列</span><span class="sxs-lookup"><span data-stu-id="5a9f3-167">string</span></span>|<span data-ttu-id="5a9f3-p105">該当するコレクション内のオブジェクトの一意識別子。必須。</span><span class="sxs-lookup"><span data-stu-id="5a9f3-p105">A unique identifier for an object in the corresponding collection. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="5a9f3-170">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5a9f3-170">Request headers</span></span>

| <span data-ttu-id="5a9f3-171">名前</span><span class="sxs-lookup"><span data-stu-id="5a9f3-171">Name</span></span>       | <span data-ttu-id="5a9f3-172">値</span><span class="sxs-lookup"><span data-stu-id="5a9f3-172">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="5a9f3-173">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a9f3-173">Authorization</span></span> | <span data-ttu-id="5a9f3-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5a9f3-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5a9f3-176">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5a9f3-176">Content-Type</span></span> | <span data-ttu-id="5a9f3-177">application/json</span><span class="sxs-lookup"><span data-stu-id="5a9f3-177">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="5a9f3-178">要求本文</span><span class="sxs-lookup"><span data-stu-id="5a9f3-178">Request body</span></span>

<span data-ttu-id="5a9f3-179">次の必要な名前/値ペアとその他のカスタム データの[openTypeExtension](../resources/opentypeextension.md)の場合、JSON の本体を提供します。</span><span class="sxs-lookup"><span data-stu-id="5a9f3-179">Provide a JSON body of an [openTypeExtension](../resources/opentypeextension.md), with the following required name-value pairs and any additional custom data.</span></span> <span data-ttu-id="5a9f3-180">JSON ペイロード内のデータは、プリミティブ型か、プリミティブ型の配列にすることができます。</span><span class="sxs-lookup"><span data-stu-id="5a9f3-180">The data in the JSON payload can be primitive types, or arrays of primitive types.</span></span>

| <span data-ttu-id="5a9f3-181">名前</span><span class="sxs-lookup"><span data-stu-id="5a9f3-181">Name</span></span>       | <span data-ttu-id="5a9f3-182">値</span><span class="sxs-lookup"><span data-stu-id="5a9f3-182">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="5a9f3-183">@odata.type</span><span class="sxs-lookup"><span data-stu-id="5a9f3-183">@odata.type</span></span> | <span data-ttu-id="5a9f3-184">Microsoft.Graph.OpenTypeExtension</span><span class="sxs-lookup"><span data-stu-id="5a9f3-184">Microsoft.Graph.OpenTypeExtension</span></span> |
| <span data-ttu-id="5a9f3-185">extensionName</span><span class="sxs-lookup"><span data-stu-id="5a9f3-185">extensionName</span></span> | <span data-ttu-id="5a9f3-186">%unique_string%</span><span class="sxs-lookup"><span data-stu-id="5a9f3-186">%unique_string%</span></span> |

<span data-ttu-id="5a9f3-187">_新しい_リソース インスタンスに拡張機能を作成するときは、新しい **openTypeExtension** オブジェクトに加えて、関連するプロパティの JSON 表現を指定して、このようなリソース インスタンスを作成します。</span><span class="sxs-lookup"><span data-stu-id="5a9f3-187">When creating an extension in a _new_ resource instance, in addition to the new **openTypeExtension** object, provide a JSON representation of the relevant properties to create such a resource instance.</span></span>

## <a name="response"></a><span data-ttu-id="5a9f3-188">応答</span><span class="sxs-lookup"><span data-stu-id="5a9f3-188">Response</span></span>

### <a name="response-code"></a><span data-ttu-id="5a9f3-189">応答コード</span><span class="sxs-lookup"><span data-stu-id="5a9f3-189">Response code</span></span>

<span data-ttu-id="5a9f3-190">応答コードは、操作によって `201 Created` または `202 Accepted` になります。</span><span class="sxs-lookup"><span data-stu-id="5a9f3-190">Depending on the operation, the response code can be `201 Created` or `202 Accepted`.</span></span>

<span data-ttu-id="5a9f3-191">リソース インスタンスを作成するために使用同じ操作を使用して拡張機能を作成する操作は、同じ操作を使用して、拡張子のないリソースのインスタンスを作成するときに返される応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="5a9f3-191">When you create an extension using the same operation that you use to create a resource instance, the operation returns the same response code that it returns when you use the operation to create the resource instance without the extension.</span></span>
<span data-ttu-id="5a9f3-192">として一覧表示されている[上](#create-an-extension-in-a-new-resource-instance)インスタンスを作成するための対応するトピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="5a9f3-192">Refer to the corresponding topics for creating the instance, as listed [above](#create-an-extension-in-a-new-resource-instance).</span></span>

### <a name="response-body"></a><span data-ttu-id="5a9f3-193">応答本文</span><span class="sxs-lookup"><span data-stu-id="5a9f3-193">Response body</span></span>

| <span data-ttu-id="5a9f3-194">シナリオ</span><span class="sxs-lookup"><span data-stu-id="5a9f3-194">Scenario</span></span>       | <span data-ttu-id="5a9f3-195">リソース</span><span class="sxs-lookup"><span data-stu-id="5a9f3-195">Resource</span></span>  | <span data-ttu-id="5a9f3-196">応答本文</span><span class="sxs-lookup"><span data-stu-id="5a9f3-196">Response body</span></span> |
|:---------------|:----------|:--------------|
| <span data-ttu-id="5a9f3-197">_新しい_リソース インスタンスを明示的に作成しながら、拡張機能を作成する</span><span class="sxs-lookup"><span data-stu-id="5a9f3-197">Creating an extension while explicitly creating a _new_ resource instance</span></span> | <span data-ttu-id="5a9f3-198">[連絡先](../resources/contact.md)、[イベント](../resources/event.md)、[メッセージ](../resources/message.md)</span><span class="sxs-lookup"><span data-stu-id="5a9f3-198">[contact](../resources/contact.md), [event](../resources/event.md), [message](../resources/message.md)</span></span> | <span data-ttu-id="5a9f3-199">[openTypeExtension](../resources/opentypeextension.md) オブジェクトで展開した新しいインスタンスを含みます。</span><span class="sxs-lookup"><span data-stu-id="5a9f3-199">Includes the new instance expanded with the [openTypeExtension](../resources/opentypeextension.md) object.</span></span> |
| <span data-ttu-id="5a9f3-200">新しいリソース インスタンスを暗示的に作成しながら、拡張機能を作成する</span><span class="sxs-lookup"><span data-stu-id="5a9f3-200">Creating an extension while implicitly creating a resource instance</span></span> | [<span data-ttu-id="5a9f3-201">post</span><span class="sxs-lookup"><span data-stu-id="5a9f3-201">post</span></span>](../resources/post.md) | <span data-ttu-id="5a9f3-202">応答には、応答コードだけが含まれ、応答本体は含まれません。</span><span class="sxs-lookup"><span data-stu-id="5a9f3-202">The response includes only a response code but not a response body.</span></span> |
| <span data-ttu-id="5a9f3-203">_既存_のリソース インスタンスに拡張機能を作成する</span><span class="sxs-lookup"><span data-stu-id="5a9f3-203">Creating an extension in an _existing_ resource instance</span></span> | <span data-ttu-id="5a9f3-204">サポートされているすべてのリソース</span><span class="sxs-lookup"><span data-stu-id="5a9f3-204">All supported resources</span></span> | <span data-ttu-id="5a9f3-205">**openTypeExtension** オブジェクトが含まれます。</span><span class="sxs-lookup"><span data-stu-id="5a9f3-205">Includes the **openTypeExtension** object.</span></span> |

## <a name="example"></a><span data-ttu-id="5a9f3-206">例</span><span class="sxs-lookup"><span data-stu-id="5a9f3-206">Example</span></span>

### <a name="request-1"></a><span data-ttu-id="5a9f3-207">要求 1</span><span class="sxs-lookup"><span data-stu-id="5a9f3-207">Request 1</span></span>

<span data-ttu-id="5a9f3-p109">最初の例では、同一の呼び出しでメッセージと拡張情報を作成します。要求本文には、次のものが含まれます。</span><span class="sxs-lookup"><span data-stu-id="5a9f3-p109">The first example creates a message and an extension in the same call. The request body includes the following:</span></span>

- <span data-ttu-id="5a9f3-210">新しいメッセージ固有の **subject**、**body**、**toRecipients** プロパティ。</span><span class="sxs-lookup"><span data-stu-id="5a9f3-210">The **subject**, **body**, and **toRecipients** properties typical of a new message.</span></span>
- <span data-ttu-id="5a9f3-211">拡張情報に関する次のもの。</span><span class="sxs-lookup"><span data-stu-id="5a9f3-211">And for the extension:</span></span>

  - <span data-ttu-id="5a9f3-212">型 `Microsoft.Graph.OpenTypeExtension`。</span><span class="sxs-lookup"><span data-stu-id="5a9f3-212">The type `Microsoft.Graph.OpenTypeExtension`.</span></span>
  - <span data-ttu-id="5a9f3-213">拡張情報名 "Com.Contoso.Referral"。</span><span class="sxs-lookup"><span data-stu-id="5a9f3-213">The extension name "Com.Contoso.Referral".</span></span>
  - <span data-ttu-id="5a9f3-214">JSON ペイロード内の 3 つのカスタム プロパティとして格納される追加のデータ: `companyName`、`expirationDate`と`dealValue`。</span><span class="sxs-lookup"><span data-stu-id="5a9f3-214">Additional data to be stored as three custom properties in the JSON payload: `companyName`, `expirationDate`, and `dealValue`.</span></span>

<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_1"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages

{
  "subject": "Annual review",
  "body": {
    "contentType": "HTML",
    "content": "You should be proud!"
  },
  "toRecipients": [
    {
      "emailAddress": {
        "address": "rufus@contoso.com"
      }
    }
  ],
  "extensions": [
    {
      "@odata.type": "Microsoft.Graph.OpenTypeExtension",
      "extensionName": "Com.Contoso.Referral",
      "companyName": "Wingtip Toys",
      "expirationDate": "2015-12-30T11:00:00.000Z",
      "dealValue": 10000
    }
  ]
}
```

### <a name="response-1"></a><span data-ttu-id="5a9f3-215">応答 1</span><span class="sxs-lookup"><span data-stu-id="5a9f3-215">Response 1</span></span>

<span data-ttu-id="5a9f3-p110">最初の例の応答を次に示します。応答本文には、新しいメッセージのプロパティと、新しい拡張情報に関する次のものが含まれています。</span><span class="sxs-lookup"><span data-stu-id="5a9f3-p110">Here is the response for the first example. The response body includes properties of the new message, and the following for the new extension:</span></span>

- <span data-ttu-id="5a9f3-218">**id** プロパティと `Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral` の完全修飾名。</span><span class="sxs-lookup"><span data-stu-id="5a9f3-218">The **id** property with the fully qualified name of `Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral`.</span></span>
- <span data-ttu-id="5a9f3-219">要求で指定されている既定のプロパティ **extensionName**。</span><span class="sxs-lookup"><span data-stu-id="5a9f3-219">The default property **extensionName** specified in the request.</span></span>
- <span data-ttu-id="5a9f3-220">要求で指定されている、3 つのカスタム プロパティとして格納されるカスタム データ。</span><span class="sxs-lookup"><span data-stu-id="5a9f3-220">The custom data specified in the request stored as 3 custom properties.</span></span>

<span data-ttu-id="5a9f3-p111">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="5a9f3-p111">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages/$entity",
  "@odata.id": "https://graph.microsoft.com/beta/users('ddfc984d-b826-40d7-b48b-57002df800e5@1717f226-49d1-4d0c-9d74-709fad664b77')/messages
('AAMkAGEbs88AAB84uLuAAA=')",
  "@odata.etag": "W/\"CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AAB88LOj\"",
  "id": "AAMkAGEbs88AAB84uLuAAA=",
  "createdDateTime": "2015-10-30T03:03:43Z",
  "lastModifiedDateTime": "2015-10-30T03:03:43Z",
  "changeKey": "CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AAB88LOj",
  "categories": [ ],
  "receivedDateTime": "2015-10-30T03:03:43Z",
  "sentDateTime": "2015-10-30T03:03:43Z",
  "hasAttachments": false,
  "subject": "Annual review",
  "body": {
    "contentType": "HTML",
    "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r
\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nYou should be proud!\r\n</body>\r
\n</html>\r\n"
  },
  "bodyPreview": "You should be proud!",
  "importance": "Normal",
  "parentFolderId": "AQMkAGEwAAAIBDwAAAA==",
  "sender": null,
  "from": null,
  "toRecipients": [
    {
      "emailAddress": {
        "address": "rufus@contoso.com",
        "name": "John Doe"
      }
    }
  ],
  "ccRecipients": [ ],
  "bccRecipients": [ ],
  "replyTo": [ ],
  "conversationId": "AAQkAGEFGugh3SVdMzzc=",
  "isDeliveryReceiptRequested": false,
  "isReadReceiptRequested": false,
  "isRead": true,
  "isDraft": true,
  "webLink": "https://outlook.office.com/owa/?
ItemID=AAMkAGEbs88AAB84uLuAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
  "inferenceClassification": "Focused",
  "extensions@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages
('AAMkAGEbs88AAB84uLuAAA%3D')/extensions",
  "extensions": [
    {
      "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
      "@odata.id": "https://graph.microsoft.com/beta/users('ddfc984d-b826-40d7-b48b-57002df800e5@1717f226-49d1-4d0c-9d74-709fad664b77')/messages
('AAMkAGEbs88AAB84uLuAAA=')/extensions('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
      "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
      "extensionName": "Com.Contoso.Referral",
      "companyName": "Wingtip Toys",
      "expirationDate": "2015-12-30T11:00:00.000Z",
      "dealValue": 10000
    }
  ]
}
```

****

### <a name="request-2"></a><span data-ttu-id="5a9f3-223">要求 2</span><span class="sxs-lookup"><span data-stu-id="5a9f3-223">Request 2</span></span>

<span data-ttu-id="5a9f3-p112">2 番目の例では、指定されたメッセージに拡張情報を作成します。要求本文には、拡張情報に関する次のものが含まれます。</span><span class="sxs-lookup"><span data-stu-id="5a9f3-p112">The second example creates an extension in the specified message. The request body includes the following for the extension:</span></span>

- <span data-ttu-id="5a9f3-226">型 `Microsoft.Graph.OpenTypeExtension`。</span><span class="sxs-lookup"><span data-stu-id="5a9f3-226">The type `Microsoft.Graph.OpenTypeExtension`.</span></span>
- <span data-ttu-id="5a9f3-227">拡張情報名 "Com.Contoso.Referral"。</span><span class="sxs-lookup"><span data-stu-id="5a9f3-227">The extension name "Com.Contoso.Referral".</span></span>
- <span data-ttu-id="5a9f3-228">JSON ペイロードに 3 つのカスタム プロパティとして格納される追加のデータ: `companyName`、`dealValue`、`expirationDate`。</span><span class="sxs-lookup"><span data-stu-id="5a9f3-228">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `dealValue`, and `expirationDate`.</span></span>

<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_2"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions

{
  "@odata.type" : "Microsoft.Graph.OpenTypeExtension",
  "extensionName" : "Com.Contoso.Referral",
  "companyName" : "Wingtip Toys",
  "dealValue" : 500050,
  "expirationDate" : "2015-12-03T10:00:00.000Z"
}
```

### <a name="response-2"></a><span data-ttu-id="5a9f3-229">応答 2</span><span class="sxs-lookup"><span data-stu-id="5a9f3-229">Response 2</span></span>

<span data-ttu-id="5a9f3-p113">2 番目の例の応答を次に示します。応答本文には、新しい拡張情報に関する次のものが含まれています。</span><span class="sxs-lookup"><span data-stu-id="5a9f3-p113">Here is the response for the second example. The response body includes the following for the new extension:</span></span>

- <span data-ttu-id="5a9f3-232">既定のプロパティ **extensionName**。</span><span class="sxs-lookup"><span data-stu-id="5a9f3-232">The default property **extensionName**.</span></span>
- <span data-ttu-id="5a9f3-233">**id** プロパティと `Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral` の完全修飾名。</span><span class="sxs-lookup"><span data-stu-id="5a9f3-233">The **id** property with the fully qualified name of `Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral`.</span></span>
- <span data-ttu-id="5a9f3-234">格納されるカスタム データ。</span><span class="sxs-lookup"><span data-stu-id="5a9f3-234">The custom data to be stored.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.opentypeextension"
} -->
```http
HTTP/1.1 201 Created
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
    "expirationDate": "2015-12-03T10:00:00.000Z"
}
```

****

### <a name="request-3"></a><span data-ttu-id="5a9f3-235">要求 3</span><span class="sxs-lookup"><span data-stu-id="5a9f3-235">Request 3</span></span>

<span data-ttu-id="5a9f3-p114">3 番目の例では、指定されたグループ イベントに拡張情報を作成します。要求本文には、拡張情報に関する次のものが含まれます。</span><span class="sxs-lookup"><span data-stu-id="5a9f3-p114">The third example creates an extension in the specified group event. The request body includes the following for the extension:</span></span>

- <span data-ttu-id="5a9f3-238">型 `Microsoft.Graph.OpenTypeExtension`。</span><span class="sxs-lookup"><span data-stu-id="5a9f3-238">The type `Microsoft.Graph.OpenTypeExtension`.</span></span>
- <span data-ttu-id="5a9f3-239">拡張情報名 "Com.Contoso.Deal"。</span><span class="sxs-lookup"><span data-stu-id="5a9f3-239">The extension name "Com.Contoso.Deal".</span></span>
- <span data-ttu-id="5a9f3-240">JSON ペイロードに 3 つのカスタム プロパティとして格納される追加のデータ: `companyName`、`dealValue`、`expirationDate`。</span><span class="sxs-lookup"><span data-stu-id="5a9f3-240">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `dealValue`, and `expirationDate`.</span></span>

<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_3"
}-->
```http
POST https://graph.microsoft.com/beta/groups('f5480dfd-7d77-4d0b-ba2e-3391953cc74a')/events('AAMkADVl17IsAAA=')/extensions

{
  "@odata.type" : "Microsoft.Graph.OpenTypeExtension",
  "extensionName" : "Com.Contoso.Deal",
  "companyName" : "Alpine Skis",
  "dealValue" : 1010100,
  "expirationDate" : "2015-07-03T13:04:00.000Z"
}
```

### <a name="response-3"></a><span data-ttu-id="5a9f3-241">応答 3</span><span class="sxs-lookup"><span data-stu-id="5a9f3-241">Response 3</span></span>

<span data-ttu-id="5a9f3-242">3 番目の例の要求からの応答を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5a9f3-242">Here is the response from the third example request.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.opentypeextension"
} -->
```http
HTTP/1.1 201 Created
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

### <a name="request-4"></a><span data-ttu-id="5a9f3-243">要求 4</span><span class="sxs-lookup"><span data-stu-id="5a9f3-243">Request 4</span></span>

<span data-ttu-id="5a9f3-p115">4 番目の例では、既存のグループ投稿に対する **reply** アクション呼び出しと同じ呼び出しを使用して、新しいグループ投稿に拡張情報を作成します。**reply** アクションは、新しい投稿と、投稿に埋め込まれる新しい拡張情報を作成します。要求本文には **post** プロパティが含まれます。そのプロパティには新しい投稿の **body** が含まれ、さらに新しい拡張情報の次のデータが含まれます。</span><span class="sxs-lookup"><span data-stu-id="5a9f3-p115">The fourth example creates an extension in a new group post, using the same **reply** action call to an existing group post. The **reply** action creates a new post, and a new extension embedded in the post. The request body includes a **post** property, which in turn contains the **body** of the new post, and the following data for the new extension:</span></span>

- <span data-ttu-id="5a9f3-247">型 `Microsoft.Graph.OpenTypeExtension`。</span><span class="sxs-lookup"><span data-stu-id="5a9f3-247">The type `Microsoft.Graph.OpenTypeExtension`.</span></span>
- <span data-ttu-id="5a9f3-248">拡張情報名 "Com.Contoso.HR"。</span><span class="sxs-lookup"><span data-stu-id="5a9f3-248">The extension name "Com.Contoso.HR".</span></span>
- <span data-ttu-id="5a9f3-249">JSON ペイロードに 3 つのカスタム プロパティとして格納される追加のデータ: `companyName`、`expirationDate`、文字列 `topPicks` の配列。</span><span class="sxs-lookup"><span data-stu-id="5a9f3-249">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `expirationDate`, and the array of strings `topPicks`.</span></span>

<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_4"
}-->
```http
POST https://graph.microsoft.com/beta/groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/threads('AAQkADJizZJpEWwqDHsEpV_KA==')/posts('AAMkADJiUg96QZUkA-ICwMubAAC1heiSAAA=')/reply

{
  "post": {
    "body": {
      "contentType": "html",
      "content": "<html><body><div><div><div><div>When and where? </div></div></div></div></body></html>"
    },
  "extensions": [
    {
      "@odata.type": "Microsoft.OutlookServices.OpenTypeExtension",
      "extensionName": "Com.Contoso.HR",
      "companyName": "Contoso",
      "expirationDate": "2015-07-03T13:04:00.000Z",
      "topPicks": [
        "Employees only",
        "Add spouse or guest",
        "Add family"
      ]
    }
  ]
  }
}
```

### <a name="response-4"></a><span data-ttu-id="5a9f3-250">応答 4</span><span class="sxs-lookup"><span data-stu-id="5a9f3-250">Response 4</span></span>

<span data-ttu-id="5a9f3-p116">4 番目の例の応答を次に示します。新しいグループ投稿に正常に拡張情報を作成できた場合は、HTTP 202 応答コードのみが生成されます。</span><span class="sxs-lookup"><span data-stu-id="5a9f3-p116">Here is the response from the fourth example. Successfully creating an extension in a new group post results in only the HTTP 202 response code.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
Content-type: text/plain
Content-Length: 0
```

****

### <a name="request-5"></a><span data-ttu-id="5a9f3-253">要求 5</span><span class="sxs-lookup"><span data-stu-id="5a9f3-253">Request 5</span></span>

<span data-ttu-id="5a9f3-p117">5 番目の例では、会話を作成するための同じ POST 操作を使用して、新しいグループ投稿に拡張情報を作成します。POST 操作は、新しい会話、スレッドと投稿、投稿に埋め込まれた新しい拡張情報を作成します。要求本文には、**Topic** プロパティと **Threads** プロパティや、新しい会話の子 **post** オブジェクトが含まれます。次いで、その **post** オブジェクトには、新しい投稿の **body** と、拡張情報の次のデータが含まれます。</span><span class="sxs-lookup"><span data-stu-id="5a9f3-p117">The fifth example creates an extension in a new group post using the same POST operation to create a conversation. The POST operation creates a new conversation, thread and post, and a new extension embedded in the post. The request body includes the **Topic** and **Threads** properties, and a child **post** object for the new conversation. The **post** object in turn contains the **body** of the new post, and the following data for the extension:</span></span>

- <span data-ttu-id="5a9f3-258">型 `Microsoft.Graph.OpenTypeExtension`。</span><span class="sxs-lookup"><span data-stu-id="5a9f3-258">The type `Microsoft.Graph.OpenTypeExtension`.</span></span>
- <span data-ttu-id="5a9f3-259">拡張情報名 "Com.Contoso.HR"。</span><span class="sxs-lookup"><span data-stu-id="5a9f3-259">The extension name "Com.Contoso.HR".</span></span>
- <span data-ttu-id="5a9f3-260">JSON ペイロードに 3 つのカスタム プロパティとして格納される追加のデータ: `companyName`、`expirationDate`、文字列 `topPicks` の配列。</span><span class="sxs-lookup"><span data-stu-id="5a9f3-260">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `expirationDate`, and the array of strings `topPicks`.</span></span>

<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_5"
}-->
```http
POST https://graph.microsoft.com/beta/groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/conversations

{
  "Topic": "Does anyone have a second?",
  "Threads": [
    {
      "Posts": [
        {
          "Body": {
            "ContentType": "HTML",
            "Content": "This is urgent!"
          },
          "Extensions": [
            {
              "@odata.type": "Microsoft.OutlookServices.OpenTypeExtension",
              "extensionName": "Com.Contoso.Benefits",
              "companyName": "Contoso",
              "expirationDate": "2016-08-03T11:00:00.000Z",
              "topPicks": [
                "Employees only",
                "Add spouse or guest",
                "Add family"
              ]
            }
          ]
        }
      ]
    }
  ]
}
```

### <a name="response-5"></a><span data-ttu-id="5a9f3-261">応答 5</span><span class="sxs-lookup"><span data-stu-id="5a9f3-261">Response 5</span></span>

<span data-ttu-id="5a9f3-p118">5 番目の例の応答を次に示します。この応答には、新しい会話とスレッド ID が含まれています。この新しいスレッドには、自動的に作成された投稿が含まれ、その投稿に新しい拡張情報が含まれます。</span><span class="sxs-lookup"><span data-stu-id="5a9f3-p118">Here is the response from the fifth example which contains the new conversation and a thread ID. This new thread contains an automatically created post, which in turn contains the new extension.</span></span>

<span data-ttu-id="5a9f3-p119">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="5a9f3-p119">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<span data-ttu-id="5a9f3-p120">新しい拡張情報を取得するには、まずこのスレッド内の[すべての投稿を取得](../api/conversationthread-list-posts.md)します。投稿は最初は 1 つしかありません。その後、投稿 ID と拡張情報名 `Com.Contoso.Benefits` を適用して、[拡張情報を取得](../api/opentypeextension-get.md)します。</span><span class="sxs-lookup"><span data-stu-id="5a9f3-p120">To get the new extension, first [get all the posts](../api/conversationthread-list-posts.md) in this thread, and initially there should be only one. Then apply the post ID and the extension name `Com.Contoso.Benefits` to [get the extension](../api/opentypeextension-get.md).</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/conversations/$entity",
    "id": "AAQkADJToRlbJ5Mg7TFM7H-j3Y=",
    "threads@odata.context": "https://graph.microsoft.com/beta/$metadata#groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/conversations('AAQkADJToRlbJ5Mg7TFM7H-j3Y%3D')/threads",
    "threads": [
        {
            "id": "AAQkADJDtMUzsf_PdhAAswJOhGVsnkyDtMUzsf_Pdg=="
        }
    ]
}

```

<!-- This page was manually created. -->
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create extension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
