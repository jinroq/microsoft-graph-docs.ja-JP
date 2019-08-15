---
title: オープン拡張機能を作成する
description: オープン拡張機能 (openTypeExtension オブジェクト) を作成し、カスタムプロパティを追加する
localization_priority: Normal
author: dkershaw10
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 5069a6486ba36ced8a961887f6ecff16dc740114
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36414414"
---
# <a name="create-open-extension"></a><span data-ttu-id="2aa7a-103">オープン拡張機能を作成する</span><span class="sxs-lookup"><span data-stu-id="2aa7a-103">Create open extension</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2aa7a-104">オープン拡張機能 ([Opentypeextension](../resources/opentypeextension.md)オブジェクト) を作成し、サポートされているリソースの新規または既存のインスタンスにカスタムプロパティを追加します。</span><span class="sxs-lookup"><span data-stu-id="2aa7a-104">Create an open extension ([openTypeExtension](../resources/opentypeextension.md) object) and add custom properties in a new or existing instance of a supported resource.</span></span>

> <span data-ttu-id="2aa7a-105">**注:** Outlook リソースでオープン拡張機能を作成する場合は、[openTypeExtension リソースの種類](../resources/opentypeextension.md#outlook-specific-considerations)にある**Outlook-固有の考慮事項** を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2aa7a-105">**Note:** If you're creating open extensions on Outlook resources, see **Outlook-specific considerations** in [openTypeExtension resource type](../resources/opentypeextension.md#outlook-specific-considerations).</span></span>

## <a name="permissions"></a><span data-ttu-id="2aa7a-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2aa7a-106">Permissions</span></span>

<span data-ttu-id="2aa7a-107">拡張機能を含むリソースおよび要求されたアクセス許可の種類（代理またはアプリケーション）に応じて、以下の表で指定されているアクセス許可が、このAPIを呼び出すために最低限必要な特権になります。</span><span class="sxs-lookup"><span data-stu-id="2aa7a-107">Depending on the resource you're creating the extension in and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="2aa7a-108">アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2aa7a-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2aa7a-109">サポートされているリソース</span><span class="sxs-lookup"><span data-stu-id="2aa7a-109">Supported resource</span></span> | <span data-ttu-id="2aa7a-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2aa7a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2aa7a-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2aa7a-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2aa7a-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2aa7a-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="2aa7a-113">device</span><span class="sxs-lookup"><span data-stu-id="2aa7a-113">device</span></span>](../resources/device.md) | <span data-ttu-id="2aa7a-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2aa7a-114">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="2aa7a-115">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="2aa7a-115">Not supported</span></span> | <span data-ttu-id="2aa7a-116">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2aa7a-116">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="2aa7a-117">イベント</span><span class="sxs-lookup"><span data-stu-id="2aa7a-117">event</span></span>](../resources/event.md) | <span data-ttu-id="2aa7a-118">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2aa7a-118">Calendars.ReadWrite</span></span> | <span data-ttu-id="2aa7a-119">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2aa7a-119">Calendars.ReadWrite</span></span> | <span data-ttu-id="2aa7a-120">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2aa7a-120">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="2aa7a-121">グループ</span><span class="sxs-lookup"><span data-stu-id="2aa7a-121">group</span></span>](../resources/group.md) | <span data-ttu-id="2aa7a-122">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2aa7a-122">Group.ReadWrite.All</span></span> | <span data-ttu-id="2aa7a-123">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="2aa7a-123">Not supported</span></span> | <span data-ttu-id="2aa7a-124">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2aa7a-124">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="2aa7a-125">グループ イベント</span><span class="sxs-lookup"><span data-stu-id="2aa7a-125">group event</span></span>](../resources/event.md) | <span data-ttu-id="2aa7a-126">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2aa7a-126">Group.ReadWrite.All</span></span> | <span data-ttu-id="2aa7a-127">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="2aa7a-127">Not supported</span></span> | <span data-ttu-id="2aa7a-128">非サポート</span><span class="sxs-lookup"><span data-stu-id="2aa7a-128">Not supported</span></span> |
| [<span data-ttu-id="2aa7a-129">グループの投稿</span><span class="sxs-lookup"><span data-stu-id="2aa7a-129">group post</span></span>](../resources/post.md) | <span data-ttu-id="2aa7a-130">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2aa7a-130">Group.ReadWrite.All</span></span> | <span data-ttu-id="2aa7a-131">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="2aa7a-131">Not supported</span></span> | <span data-ttu-id="2aa7a-132">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2aa7a-132">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="2aa7a-133">メッセージ</span><span class="sxs-lookup"><span data-stu-id="2aa7a-133">message</span></span>](../resources/message.md) | <span data-ttu-id="2aa7a-134">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2aa7a-134">Mail.ReadWrite</span></span> | <span data-ttu-id="2aa7a-135">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2aa7a-135">Mail.ReadWrite</span></span> | <span data-ttu-id="2aa7a-136">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2aa7a-136">Mail.ReadWrite</span></span> | 
| [<span data-ttu-id="2aa7a-137">組織</span><span class="sxs-lookup"><span data-stu-id="2aa7a-137">organization</span></span>](../resources/organization.md) | <span data-ttu-id="2aa7a-138">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2aa7a-138">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="2aa7a-139">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="2aa7a-139">Not supported</span></span> | <span data-ttu-id="2aa7a-140">非サポート</span><span class="sxs-lookup"><span data-stu-id="2aa7a-140">Not supported</span></span> |
| [<span data-ttu-id="2aa7a-141">個人用連絡先</span><span class="sxs-lookup"><span data-stu-id="2aa7a-141">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="2aa7a-142">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2aa7a-142">Contacts.ReadWrite</span></span> | <span data-ttu-id="2aa7a-143">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2aa7a-143">Contacts.ReadWrite</span></span> | <span data-ttu-id="2aa7a-144">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2aa7a-144">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="2aa7a-145">user</span><span class="sxs-lookup"><span data-stu-id="2aa7a-145">user</span></span>](../resources/user.md) | <span data-ttu-id="2aa7a-146">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2aa7a-146">User.ReadWrite.All</span></span> | <span data-ttu-id="2aa7a-147">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2aa7a-147">User.ReadWrite</span></span> | <span data-ttu-id="2aa7a-148">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2aa7a-148">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2aa7a-149">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2aa7a-149">HTTP request</span></span>

### <a name="create-an-extension-in-a-new-resource-instance"></a><span data-ttu-id="2aa7a-150">新規のリソース インスタンスに拡張機能を作成する</span><span class="sxs-lookup"><span data-stu-id="2aa7a-150">Create an extension in a new resource instance</span></span>

<span data-ttu-id="2aa7a-151">インスタンスを作成するには、同じ REST 要求を使います。</span><span class="sxs-lookup"><span data-stu-id="2aa7a-151">Use the same REST request that you use to create the instance.</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/events
POST /users/{id|userPrincipalName}/messages
POST /groups/{id}/events
POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /users/{id|userPrincipalName}/contacts
```

><span data-ttu-id="2aa7a-152">**注:** この構文は、サポートされているリソース インスタンスを作成する一般的な方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="2aa7a-152">**Note:** This syntax shows some common ways to create the supported resource instances.</span></span> <span data-ttu-id="2aa7a-153">こうしたリソース インスタンスを作成するために使用できる他の POST 構文すべても、同様の方法でオープン拡張機能を作成できます。</span><span class="sxs-lookup"><span data-stu-id="2aa7a-153">All other POST syntaxes that allows you to create these resource instances supports creating open extensions in them in a similar way.</span></span>

<span data-ttu-id="2aa7a-154">要求本文に、新規のリソース インスタンスのプロパティおよび_拡張機能_を含める方法については、[要求本文](#request-body)のセクションをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="2aa7a-154">See the [Request body](#request-body) section about including the properties of the new resource instance _and the extension_ in the request body.</span></span>

### <a name="create-an-extension-in-an-existing-resource-instance"></a><span data-ttu-id="2aa7a-155">既存のリソース インスタンスに拡張機能を作成する</span><span class="sxs-lookup"><span data-stu-id="2aa7a-155">Create an extension in an existing resource instance</span></span>

<span data-ttu-id="2aa7a-156">その要求でリソース インスタンスを識別し、**機能拡張** ナビゲーション プロパティで `POST` を行います。</span><span class="sxs-lookup"><span data-stu-id="2aa7a-156">Identify the resource instance in the request and do a `POST` to the **extensions** navigation property.</span></span>

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

><span data-ttu-id="2aa7a-157">**注:** 上記の構文は、拡張機能をその中に作成するリソース インスタンスを特定する一般的な方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="2aa7a-157">**Note:** This syntax shows some common ways to identify a resource instance, in order to create an extension in it.</span></span> <span data-ttu-id="2aa7a-158">こうしたリソース インスタンスを特定するために使用できる他の構文すべても、同様の方法でオープン拡張機能を作成できます。</span><span class="sxs-lookup"><span data-stu-id="2aa7a-158">All other syntaxes that allows you to identify these resource instances supports creating open extensions in them in a similar way.</span></span>

<span data-ttu-id="2aa7a-159">要求本文にある_拡張機能_を含めた[要求本文](#request-body)のセクションを参照してください。</span><span class="sxs-lookup"><span data-stu-id="2aa7a-159">See the [Request body](#request-body) section about including _the extension_ in the request body.</span></span>

## <a name="path-parameters"></a><span data-ttu-id="2aa7a-160">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="2aa7a-160">Path parameters</span></span>

|<span data-ttu-id="2aa7a-161">**パラメーター**</span><span class="sxs-lookup"><span data-stu-id="2aa7a-161">**Parameter**</span></span>|<span data-ttu-id="2aa7a-162">**型**</span><span class="sxs-lookup"><span data-stu-id="2aa7a-162">**Type**</span></span>|<span data-ttu-id="2aa7a-163">**説明**</span><span class="sxs-lookup"><span data-stu-id="2aa7a-163">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="2aa7a-164">id</span><span class="sxs-lookup"><span data-stu-id="2aa7a-164">id</span></span>|<span data-ttu-id="2aa7a-165">string</span><span class="sxs-lookup"><span data-stu-id="2aa7a-165">string</span></span>|<span data-ttu-id="2aa7a-p104">該当するコレクション内のオブジェクトの一意識別子。必須。</span><span class="sxs-lookup"><span data-stu-id="2aa7a-p104">A unique identifier for an object in the corresponding collection. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="2aa7a-168">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2aa7a-168">Request headers</span></span>

| <span data-ttu-id="2aa7a-169">名前</span><span class="sxs-lookup"><span data-stu-id="2aa7a-169">Name</span></span>       | <span data-ttu-id="2aa7a-170">値</span><span class="sxs-lookup"><span data-stu-id="2aa7a-170">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="2aa7a-171">Authorization</span><span class="sxs-lookup"><span data-stu-id="2aa7a-171">Authorization</span></span> | <span data-ttu-id="2aa7a-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2aa7a-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2aa7a-174">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2aa7a-174">Content-Type</span></span> | <span data-ttu-id="2aa7a-175">application/json</span><span class="sxs-lookup"><span data-stu-id="2aa7a-175">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="2aa7a-176">要求本文</span><span class="sxs-lookup"><span data-stu-id="2aa7a-176">Request body</span></span>

<span data-ttu-id="2aa7a-p106">次の必須の名前と値のペアと追加のカスタムデータを使用して、 [Opentypeextension](../resources/opentypeextension.md)の JSON 本文を指定します。JSON ペイロードのデータは、プリミティブ型、またはプリミティブ型の配列にすることができます。</span><span class="sxs-lookup"><span data-stu-id="2aa7a-p106">Provide a JSON body of an [openTypeExtension](../resources/opentypeextension.md), with the following required name-value pairs and any additional custom data. The data in the JSON payload can be primitive types, or arrays of primitive types.</span></span>

| <span data-ttu-id="2aa7a-179">名前</span><span class="sxs-lookup"><span data-stu-id="2aa7a-179">Name</span></span>       | <span data-ttu-id="2aa7a-180">値</span><span class="sxs-lookup"><span data-stu-id="2aa7a-180">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="2aa7a-181">@odata.type</span><span class="sxs-lookup"><span data-stu-id="2aa7a-181">@odata.type</span></span> | <span data-ttu-id="2aa7a-182">microsoft.graph.openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="2aa7a-182">microsoft.graph.openTypeExtension</span></span> |
| <span data-ttu-id="2aa7a-183">extensionName</span><span class="sxs-lookup"><span data-stu-id="2aa7a-183">extensionName</span></span> | <span data-ttu-id="2aa7a-184">%unique_string%</span><span class="sxs-lookup"><span data-stu-id="2aa7a-184">%unique_string%</span></span> |

<span data-ttu-id="2aa7a-185">_新しい_リソース インスタンスに拡張機能を作成するときは、新しい **openTypeExtension** オブジェクトに加えて、関連するプロパティの JSON 表現を指定して、このようなリソース インスタンスを作成します。</span><span class="sxs-lookup"><span data-stu-id="2aa7a-185">When creating an extension in a _new_ resource instance, in addition to the new **openTypeExtension** object, provide a JSON representation of the relevant properties to create such a resource instance.</span></span>

## <a name="response"></a><span data-ttu-id="2aa7a-186">応答</span><span class="sxs-lookup"><span data-stu-id="2aa7a-186">Response</span></span>

### <a name="response-code"></a><span data-ttu-id="2aa7a-187">応答コード</span><span class="sxs-lookup"><span data-stu-id="2aa7a-187">Response code</span></span>

<span data-ttu-id="2aa7a-188">操作によって、応答コードは `201 Created` または `202 Accepted` になります。</span><span class="sxs-lookup"><span data-stu-id="2aa7a-188">Depending on the operation, the response code can be `201 Created` or `202 Accepted`.</span></span>

<span data-ttu-id="2aa7a-189">リソース インスタンスを作成するために使用するのと同じ操作を使用して、拡張子を作成すると、操作は拡張子なしのリソースのインスタンスの作成時に返される同じ応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="2aa7a-189">When you create an extension using the same operation that you use to create a resource instance, the operation returns the same response code that it returns when you use the operation to create the resource instance without the extension.</span></span>
<span data-ttu-id="2aa7a-190">それぞれ対応するインスタンスの作成については[上記](#create-an-extension-in-a-new-resource-instance)の一覧を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2aa7a-190">Refer to the corresponding topics for creating the instance, as listed [above](#create-an-extension-in-a-new-resource-instance).</span></span>

### <a name="response-body"></a><span data-ttu-id="2aa7a-191">応答本文</span><span class="sxs-lookup"><span data-stu-id="2aa7a-191">Response body</span></span>

| <span data-ttu-id="2aa7a-192">シナリオ</span><span class="sxs-lookup"><span data-stu-id="2aa7a-192">Scenario</span></span>       | <span data-ttu-id="2aa7a-193">リソース</span><span class="sxs-lookup"><span data-stu-id="2aa7a-193">Resource</span></span>  | <span data-ttu-id="2aa7a-194">応答本文</span><span class="sxs-lookup"><span data-stu-id="2aa7a-194">Response body</span></span> |
|:---------------|:----------|:--------------|
| <span data-ttu-id="2aa7a-195">_新しい_リソース インスタンスを明示的に作成しながら、拡張機能を作成する</span><span class="sxs-lookup"><span data-stu-id="2aa7a-195">Creating an extension while explicitly creating a _new_ resource instance</span></span> | <span data-ttu-id="2aa7a-196">[連絡先](../resources/contact.md)、[イベント](../resources/event.md)、[メッセージ](../resources/message.md)</span><span class="sxs-lookup"><span data-stu-id="2aa7a-196">[contact](../resources/contact.md), [event](../resources/event.md), [message](../resources/message.md)</span></span> | <span data-ttu-id="2aa7a-197">[openTypeExtension](../resources/opentypeextension.md) オブジェクトで展開した新しいインスタンスを含みます。</span><span class="sxs-lookup"><span data-stu-id="2aa7a-197">Includes the new instance expanded with the [openTypeExtension](../resources/opentypeextension.md) object.</span></span> |
| <span data-ttu-id="2aa7a-198">新しいリソース インスタンスを暗示的に作成しながら、拡張機能を作成する</span><span class="sxs-lookup"><span data-stu-id="2aa7a-198">Creating an extension while implicitly creating a resource instance</span></span> | [<span data-ttu-id="2aa7a-199">post</span><span class="sxs-lookup"><span data-stu-id="2aa7a-199">post</span></span>](../resources/post.md) | <span data-ttu-id="2aa7a-200">応答には、応答コードだけが含まれ、応答本体は含まれません。</span><span class="sxs-lookup"><span data-stu-id="2aa7a-200">The response includes only a response code but not a response body.</span></span> |
| <span data-ttu-id="2aa7a-201">_既存_のリソース インスタンスに拡張機能を作成する</span><span class="sxs-lookup"><span data-stu-id="2aa7a-201">Creating an extension in an _existing_ resource instance</span></span> | <span data-ttu-id="2aa7a-202">サポートされているすべてのリソース</span><span class="sxs-lookup"><span data-stu-id="2aa7a-202">All supported resources</span></span> | <span data-ttu-id="2aa7a-203">**openTypeExtension** オブジェクトが含まれます。</span><span class="sxs-lookup"><span data-stu-id="2aa7a-203">Includes the **openTypeExtension** object.</span></span> |

## <a name="example"></a><span data-ttu-id="2aa7a-204">例</span><span class="sxs-lookup"><span data-stu-id="2aa7a-204">Example</span></span>

### <a name="request-1"></a><span data-ttu-id="2aa7a-205">要求 1</span><span class="sxs-lookup"><span data-stu-id="2aa7a-205">Request 1</span></span>

<span data-ttu-id="2aa7a-p108">最初の例では、同一の呼び出しでメッセージと拡張情報を作成します。要求本文には、次のものが含まれます。</span><span class="sxs-lookup"><span data-stu-id="2aa7a-p108">The first example creates a message and an extension in the same call. The request body includes the following:</span></span>

- <span data-ttu-id="2aa7a-208">新しいメッセージ固有の **subject**、**body**、**toRecipients** プロパティ。</span><span class="sxs-lookup"><span data-stu-id="2aa7a-208">The **subject**, **body**, and **toRecipients** properties typical of a new message.</span></span>
- <span data-ttu-id="2aa7a-209">拡張情報に関する次のもの。</span><span class="sxs-lookup"><span data-stu-id="2aa7a-209">And for the extension:</span></span>

  - <span data-ttu-id="2aa7a-210">型 `microsoft.graph.openTypeExtension`。</span><span class="sxs-lookup"><span data-stu-id="2aa7a-210">The type `microsoft.graph.openTypeExtension`.</span></span>
  - <span data-ttu-id="2aa7a-211">拡張情報名 "Com.Contoso.Referral"。</span><span class="sxs-lookup"><span data-stu-id="2aa7a-211">The extension name "Com.Contoso.Referral".</span></span>
  - <span data-ttu-id="2aa7a-212">JSON ペイロードに 3 つのカスタム プロパティとして格納される追加のデータ: `companyName`、`expirationDate`、`dealValue`。</span><span class="sxs-lookup"><span data-stu-id="2aa7a-212">Additional data to be stored as three custom properties in the JSON payload: `companyName`, `expirationDate`, and `dealValue`.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="2aa7a-213">プロトコル</span><span class="sxs-lookup"><span data-stu-id="2aa7a-213">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_1"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages
Content-Type: application/json

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
      "@odata.type": "microsoft.graph.openTypeExtension",
      "extensionName": "Com.Contoso.Referral",
      "companyName": "Wingtip Toys",
      "expirationDate": "2015-12-30T11:00:00.000Z",
      "dealValue": 10000
    }
  ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2aa7a-214">C#</span><span class="sxs-lookup"><span data-stu-id="2aa7a-214">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-opentypeextension-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2aa7a-215">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2aa7a-215">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-opentypeextension-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2aa7a-216">目的-C</span><span class="sxs-lookup"><span data-stu-id="2aa7a-216">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-opentypeextension-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response-1"></a><span data-ttu-id="2aa7a-217">応答 1</span><span class="sxs-lookup"><span data-stu-id="2aa7a-217">Response 1</span></span>

<span data-ttu-id="2aa7a-p109">最初の例の応答を次に示します。応答本文には、新しいメッセージのプロパティと、新しい拡張情報に関する次のものが含まれています。</span><span class="sxs-lookup"><span data-stu-id="2aa7a-p109">Here is the response for the first example. The response body includes properties of the new message, and the following for the new extension:</span></span>

- <span data-ttu-id="2aa7a-220">**id** プロパティと `microsoft.graph.openTypeExtension.Com.Contoso.Referral` の完全修飾名。</span><span class="sxs-lookup"><span data-stu-id="2aa7a-220">The **id** property with the fully qualified name of `microsoft.graph.openTypeExtension.Com.Contoso.Referral`.</span></span>
- <span data-ttu-id="2aa7a-221">要求で指定されている既定のプロパティ **extensionName**。</span><span class="sxs-lookup"><span data-stu-id="2aa7a-221">The default property **extensionName** specified in the request.</span></span>
- <span data-ttu-id="2aa7a-222">要求で指定されている、3 つのカスタム プロパティとして格納されるカスタム データ。</span><span class="sxs-lookup"><span data-stu-id="2aa7a-222">The custom data specified in the request stored as 3 custom properties.</span></span>

<span data-ttu-id="2aa7a-p110">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2aa7a-p110">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
      "@odata.type": "#microsoft.graph.openTypeExtension",
      "@odata.id": "https://graph.microsoft.com/beta/users('ddfc984d-b826-40d7-b48b-57002df800e5@1717f226-49d1-4d0c-9d74-709fad664b77')/messages
('AAMkAGEbs88AAB84uLuAAA=')/extensions('microsoft.graph.openTypeExtension.Com.Contoso.Referral')",
      "id": "microsoft.graph.openTypeExtension.Com.Contoso.Referral",
      "extensionName": "Com.Contoso.Referral",
      "companyName": "Wingtip Toys",
      "expirationDate": "2015-12-30T11:00:00.000Z",
      "dealValue": 10000
    }
  ]
}
```

****

### <a name="request-2"></a><span data-ttu-id="2aa7a-225">要求 2</span><span class="sxs-lookup"><span data-stu-id="2aa7a-225">Request 2</span></span>

<span data-ttu-id="2aa7a-p111">2 番目の例では、指定されたメッセージに拡張情報を作成します。要求本文には、拡張情報に関する次のものが含まれます。</span><span class="sxs-lookup"><span data-stu-id="2aa7a-p111">The second example creates an extension in the specified message. The request body includes the following for the extension:</span></span>

- <span data-ttu-id="2aa7a-228">型 `microsoft.graph.openTypeExtension`。</span><span class="sxs-lookup"><span data-stu-id="2aa7a-228">The type `microsoft.graph.openTypeExtension`.</span></span>
- <span data-ttu-id="2aa7a-229">拡張情報名 "Com.Contoso.Referral"。</span><span class="sxs-lookup"><span data-stu-id="2aa7a-229">The extension name "Com.Contoso.Referral".</span></span>
- <span data-ttu-id="2aa7a-230">JSON ペイロードに 3 つのカスタム プロパティとして格納される追加のデータ: `companyName`、`dealValue`、`expirationDate`。</span><span class="sxs-lookup"><span data-stu-id="2aa7a-230">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `dealValue`, and `expirationDate`.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="2aa7a-231">プロトコル</span><span class="sxs-lookup"><span data-stu-id="2aa7a-231">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_2"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions
Content-Type: application/json

{
  "@odata.type" : "microsoft.graph.openTypeExtension",
  "extensionName" : "Com.Contoso.Referral",
  "companyName" : "Wingtip Toys",
  "dealValue" : 500050,
  "expirationDate" : "2015-12-03T10:00:00.000Z"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2aa7a-232">C#</span><span class="sxs-lookup"><span data-stu-id="2aa7a-232">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-opentypeextension-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2aa7a-233">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2aa7a-233">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-opentypeextension-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2aa7a-234">目的-C</span><span class="sxs-lookup"><span data-stu-id="2aa7a-234">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-opentypeextension-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response-2"></a><span data-ttu-id="2aa7a-235">応答 2</span><span class="sxs-lookup"><span data-stu-id="2aa7a-235">Response 2</span></span>

<span data-ttu-id="2aa7a-p112">2 番目の例の応答を次に示します。応答本文には、新しい拡張情報に関する次のものが含まれています。</span><span class="sxs-lookup"><span data-stu-id="2aa7a-p112">Here is the response for the second example. The response body includes the following for the new extension:</span></span>

- <span data-ttu-id="2aa7a-238">既定のプロパティ **extensionName**。</span><span class="sxs-lookup"><span data-stu-id="2aa7a-238">The default property **extensionName**.</span></span>
- <span data-ttu-id="2aa7a-239">**id** プロパティと `microsoft.graph.openTypeExtension.Com.Contoso.Referral` の完全修飾名。</span><span class="sxs-lookup"><span data-stu-id="2aa7a-239">The **id** property with the fully qualified name of `microsoft.graph.openTypeExtension.Com.Contoso.Referral`.</span></span>
- <span data-ttu-id="2aa7a-240">格納されるカスタム データ。</span><span class="sxs-lookup"><span data-stu-id="2aa7a-240">The custom data to be stored.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.openTypeExtension"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "@odata.id": "https://graph.microsoft.com/beta/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions
('microsoft.graph.openTypeExtension.Com.Contoso.Referral')",
    "extensionName": "Com.Contoso.Referral",
    "id": "microsoft.graph.openTypeExtension.Com.Contoso.Referral",
    "companyName": "Wingtip Toys",
    "dealValue": 500050,
    "expirationDate": "2015-12-03T10:00:00.000Z"
}
```

****

### <a name="request-3"></a><span data-ttu-id="2aa7a-241">要求 3</span><span class="sxs-lookup"><span data-stu-id="2aa7a-241">Request 3</span></span>

<span data-ttu-id="2aa7a-p113">3 番目の例では、指定されたグループ イベントに拡張情報を作成します。要求本文には、拡張情報に関する次のものが含まれます。</span><span class="sxs-lookup"><span data-stu-id="2aa7a-p113">The third example creates an extension in the specified group event. The request body includes the following for the extension:</span></span>

- <span data-ttu-id="2aa7a-244">型 `microsoft.graph.openTypeExtension`。</span><span class="sxs-lookup"><span data-stu-id="2aa7a-244">The type `microsoft.graph.openTypeExtension`.</span></span>
- <span data-ttu-id="2aa7a-245">拡張情報名 "Com.Contoso.Deal"。</span><span class="sxs-lookup"><span data-stu-id="2aa7a-245">The extension name "Com.Contoso.Deal".</span></span>
- <span data-ttu-id="2aa7a-246">JSON ペイロードに 3 つのカスタム プロパティとして格納される追加のデータ: `companyName`、`dealValue`、`expirationDate`。</span><span class="sxs-lookup"><span data-stu-id="2aa7a-246">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `dealValue`, and `expirationDate`.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="2aa7a-247">プロトコル</span><span class="sxs-lookup"><span data-stu-id="2aa7a-247">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_3"
}-->
```http
POST https://graph.microsoft.com/beta/groups/f5480dfd-7d77-4d0b-ba2e-3391953cc74a/events/AAMkADVl17IsAAA=/extensions
Content-type: application/json

{
  "@odata.type" : "microsoft.graph.openTypeExtension",
  "extensionName" : "Com.Contoso.Deal",
  "companyName" : "Alpine Skis",
  "dealValue" : 1010100,
  "expirationDate" : "2015-07-03T13:04:00.000Z"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2aa7a-248">C#</span><span class="sxs-lookup"><span data-stu-id="2aa7a-248">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-opentypeextension-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2aa7a-249">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2aa7a-249">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-opentypeextension-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2aa7a-250">目的-C</span><span class="sxs-lookup"><span data-stu-id="2aa7a-250">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-opentypeextension-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response-3"></a><span data-ttu-id="2aa7a-251">応答 3</span><span class="sxs-lookup"><span data-stu-id="2aa7a-251">Response 3</span></span>

<span data-ttu-id="2aa7a-252">3 番目の例の要求からの応答を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2aa7a-252">Here is the response from the third example request.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.openTypeExtension"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups('f5480dfd-7d77-4d0b-ba2e-3391953cc74a')/events('AAMkADVl7IsAAA%3D')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "id": "microsoft.graph.openTypeExtension.Com.Contoso.Deal",
    "extensionName": "Com.Contoso.Deal",
    "companyName": "Alpine Skis",
    "dealValue": 1010100,
    "expirationDate": "2015-07-03T13:04:00Z"
}
```

****

### <a name="request-4"></a><span data-ttu-id="2aa7a-253">要求 4</span><span class="sxs-lookup"><span data-stu-id="2aa7a-253">Request 4</span></span>

<span data-ttu-id="2aa7a-p114">4 番目の例では、既存のグループ投稿に対する **reply** アクション呼び出しと同じ呼び出しを使用して、新しいグループ投稿に拡張情報を作成します。**reply** アクションは、新しい投稿と、投稿に埋め込まれる新しい拡張情報を作成します。要求本文には **post** プロパティが含まれます。そのプロパティには新しい投稿の **body** が含まれ、さらに新しい拡張情報の次のデータが含まれます。</span><span class="sxs-lookup"><span data-stu-id="2aa7a-p114">The fourth example creates an extension in a new group post, using the same **reply** action call to an existing group post. The **reply** action creates a new post, and a new extension embedded in the post. The request body includes a **post** property, which in turn contains the **body** of the new post, and the following data for the new extension:</span></span>

- <span data-ttu-id="2aa7a-257">型 `microsoft.graph.openTypeExtension`。</span><span class="sxs-lookup"><span data-stu-id="2aa7a-257">The type `microsoft.graph.openTypeExtension`.</span></span>
- <span data-ttu-id="2aa7a-258">拡張情報名 "Com.Contoso.HR"。</span><span class="sxs-lookup"><span data-stu-id="2aa7a-258">The extension name "Com.Contoso.HR".</span></span>
- <span data-ttu-id="2aa7a-259">JSON ペイロードに 3 つのカスタム プロパティとして格納される追加のデータ: `companyName`、`expirationDate`、文字列 `topPicks` の配列。</span><span class="sxs-lookup"><span data-stu-id="2aa7a-259">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `expirationDate`, and the array of strings `topPicks`.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="2aa7a-260">プロトコル</span><span class="sxs-lookup"><span data-stu-id="2aa7a-260">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_4"
}-->
```http
POST https://graph.microsoft.com/beta/groups/37df2ff0-0de0-4c33-8aee-75289364aef6/threads/AAQkADJizZJpEWwqDHsEpV_KA==/posts/AAMkADJiUg96QZUkA-ICwMubAAC1heiSAAA=/reply
Content-type: application/json

{
  "post": {
    "body": {
      "contentType": "html",
      "content": "<html><body><div><div><div><div>When and where? </div></div></div></div></body></html>"
    },
  "extensions": [
    {
      "@odata.type": "microsoft.graph.openTypeExtension",
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="2aa7a-261">C#</span><span class="sxs-lookup"><span data-stu-id="2aa7a-261">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-opentypeextension-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2aa7a-262">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2aa7a-262">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-opentypeextension-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2aa7a-263">目的-C</span><span class="sxs-lookup"><span data-stu-id="2aa7a-263">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-opentypeextension-4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response-4"></a><span data-ttu-id="2aa7a-264">応答 4</span><span class="sxs-lookup"><span data-stu-id="2aa7a-264">Response 4</span></span>

<span data-ttu-id="2aa7a-p115">4 番目の例の応答を次に示します。新しいグループ投稿に正常に拡張情報を作成できた場合は、HTTP 202 応答コードのみが生成されます。</span><span class="sxs-lookup"><span data-stu-id="2aa7a-p115">Here is the response from the fourth example. Successfully creating an extension in a new group post results in only the HTTP 202 response code.</span></span>

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

### <a name="request-5"></a><span data-ttu-id="2aa7a-267">要求 5</span><span class="sxs-lookup"><span data-stu-id="2aa7a-267">Request 5</span></span>

<span data-ttu-id="2aa7a-p116">5 番目の例では、会話を作成するための同じ POST 操作を使用して、新しいグループ投稿に拡張情報を作成します。POST 操作は、新しい会話、スレッドと投稿、投稿に埋め込まれた新しい拡張情報を作成します。要求本文には、**Topic** プロパティと **Threads** プロパティや、新しい会話の子 **post** オブジェクトが含まれます。次いで、その **post** オブジェクトには、新しい投稿の **body** と、拡張情報の次のデータが含まれます。</span><span class="sxs-lookup"><span data-stu-id="2aa7a-p116">The fifth example creates an extension in a new group post using the same POST operation to create a conversation. The POST operation creates a new conversation, thread and post, and a new extension embedded in the post. The request body includes the **Topic** and **Threads** properties, and a child **post** object for the new conversation. The **post** object in turn contains the **body** of the new post, and the following data for the extension:</span></span>

- <span data-ttu-id="2aa7a-272">型 `microsoft.graph.openTypeExtension`。</span><span class="sxs-lookup"><span data-stu-id="2aa7a-272">The type `microsoft.graph.openTypeExtension`.</span></span>
- <span data-ttu-id="2aa7a-273">拡張情報名 "Com.Contoso.HR"。</span><span class="sxs-lookup"><span data-stu-id="2aa7a-273">The extension name "Com.Contoso.HR".</span></span>
- <span data-ttu-id="2aa7a-274">JSON ペイロードに 3 つのカスタム プロパティとして格納される追加のデータ: `companyName`、`expirationDate`、文字列 `topPicks` の配列。</span><span class="sxs-lookup"><span data-stu-id="2aa7a-274">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `expirationDate`, and the array of strings `topPicks`.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="2aa7a-275">プロトコル</span><span class="sxs-lookup"><span data-stu-id="2aa7a-275">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_5"
}-->
```http
POST https://graph.microsoft.com/beta/groups/37df2ff0-0de0-4c33-8aee-75289364aef6/conversations
Content-type: application/json

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
              "@odata.type": "microsoft.graph.openTypeExtension",
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="2aa7a-276">C#</span><span class="sxs-lookup"><span data-stu-id="2aa7a-276">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-opentypeextension-5-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2aa7a-277">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2aa7a-277">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-opentypeextension-5-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2aa7a-278">目的-C</span><span class="sxs-lookup"><span data-stu-id="2aa7a-278">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-opentypeextension-5-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response-5"></a><span data-ttu-id="2aa7a-279">応答 5</span><span class="sxs-lookup"><span data-stu-id="2aa7a-279">Response 5</span></span>

<span data-ttu-id="2aa7a-p117">5 番目の例の応答を次に示します。この応答には、新しい会話とスレッド ID が含まれています。この新しいスレッドには、自動的に作成された投稿が含まれ、その投稿に新しい拡張情報が含まれます。</span><span class="sxs-lookup"><span data-stu-id="2aa7a-p117">Here is the response from the fifth example which contains the new conversation and a thread ID. This new thread contains an automatically created post, which in turn contains the new extension.</span></span>

<span data-ttu-id="2aa7a-p118">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="2aa7a-p118">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<span data-ttu-id="2aa7a-p119">新しい拡張情報を取得するには、まずこのスレッド内の[すべての投稿を取得](../api/conversationthread-list-posts.md)します。投稿は最初は 1 つしかありません。その後、投稿 ID と拡張情報名 `Com.Contoso.Benefits` を適用して、[拡張情報を取得](../api/opentypeextension-get.md)します。</span><span class="sxs-lookup"><span data-stu-id="2aa7a-p119">To get the new extension, first [get all the posts](../api/conversationthread-list-posts.md) in this thread, and initially there should be only one. Then apply the post ID and the extension name `Com.Contoso.Benefits` to [get the extension](../api/opentypeextension-get.md).</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Create extension",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
