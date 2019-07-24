---
title: Microsoft Graph API を使用する
description: Microsoft Graph は、Microsoft Cloud サービス リソースへのアクセスを可能にする RESTful Web API です。アプリを登録 して、サービス または ユーザーの認証トークンを取得する と、Microsoft Graph API に対して要求を行うことができます。
author: jackson-woods
localization_priority: Priority
ms.openlocfilehash: 18de281cc0becfacfdabe5fb81a68358f04c3747
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/24/2019
ms.locfileid: "35840643"
---
# <a name="use-the-microsoft-graph-api"></a><span data-ttu-id="09e3d-104">Microsoft Graph API を使用する</span><span class="sxs-lookup"><span data-stu-id="09e3d-104">Use the Microsoft Graph API</span></span>

<span data-ttu-id="09e3d-p102">Microsoft Graph は、Microsoft Cloud サービス リソースへのアクセスを可能にする RESTful Web API です。[アプリを登録](auth-register-app-v2.md) して、[サービス](auth-v2-service.md) または [ユーザーの認証トークンを取得する](auth-v2-user.md) と、Microsoft Graph API に対して要求を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="09e3d-p102">Microsoft Graph is a RESTful web API that enables you to access Microsoft Cloud service resources. After you [register your app](auth-register-app-v2.md) and [get authentication tokens for a user](auth-v2-user.md) or [service](auth-v2-service.md), you can make requests to the Microsoft Graph API.</span></span>

> <span data-ttu-id="09e3d-107">**重要:** 条件付きアクセス ポリシーの Microsoft Graph への適用方法は変更されています。</span><span class="sxs-lookup"><span data-stu-id="09e3d-107">**Important:**  How conditional access policies apply to Microsoft Graph is changing.</span></span> <span data-ttu-id="09e3d-108">条件付きアクセス ポリシーが構成されるシナリオを処理するよう、アプリケーションを更新する必要があります。</span><span class="sxs-lookup"><span data-stu-id="09e3d-108">Applications need to be updated to handle scenarios where conditional access policies are configured.</span></span> <span data-ttu-id="09e3d-109">詳細およびガイダンスについては、「[Azure Active Directory の条件付きアクセスについての開発者ガイド](https://docs.microsoft.com/azure/active-directory/develop/active-directory-conditional-access-developer)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="09e3d-109">For more information and guidance, see [Developer Guidance for Azure Active Directory Conditional Access](https://docs.microsoft.com/azure/active-directory/develop/active-directory-conditional-access-developer).</span></span>

<span data-ttu-id="09e3d-110">ユーザーや電子メール メッセージなど、リソースの読み取りや書き込みを行うには、次のような要求を構築します。</span><span class="sxs-lookup"><span data-stu-id="09e3d-110">To read from or write to a resource such as a user or an email message, you construct a request that looks like the following.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
{HTTP method} https://graph.microsoft.com/{version}/{resource}?{query-parameters}
```

<span data-ttu-id="09e3d-111">要求のコンポーネントには以下が含まれます。</span><span class="sxs-lookup"><span data-stu-id="09e3d-111">The components of a request include:</span></span>

* <span data-ttu-id="09e3d-112">[{HTTP メソッド}](#http-methods) - Microsoft Graph への要求で使用する HTTP メソッド。</span><span class="sxs-lookup"><span data-stu-id="09e3d-112">[HTTP method](#http-methods) - The HTTP method used on the request to Microsoft Graph.</span></span>
* <span data-ttu-id="09e3d-113">[{バージョン}](#version) - アプリケーションが使用している Microsoft Graph API のバージョン。</span><span class="sxs-lookup"><span data-stu-id="09e3d-113">   - The version of the Microsoft Graph API your application is using.</span></span>
* <span data-ttu-id="09e3d-114">[{リソース}](#resource) - ユーザーが参照している Microsoft Graph のリソース。</span><span class="sxs-lookup"><span data-stu-id="09e3d-114">   - The resource in Microsoft Graph that you're referencing.</span></span> 
* <span data-ttu-id="09e3d-115">[{クエリ パラメーター}](#query-parameters-optional) - 応答をカスタマイズするために使用する省略可能な OData クエリ オプションまたは REST メソッド パラメーター。</span><span class="sxs-lookup"><span data-stu-id="09e3d-115">[{query-parameters}](#query-parameters-optional) - Optional OData query options or REST method parameters that customize the response.</span></span>

<span data-ttu-id="09e3d-116">要求を行うと、次を含む応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="09e3d-116">After you make a request, a response is returned that includes:</span></span> 

* <span data-ttu-id="09e3d-p104">状態コード - 成功または失敗を示す HTTP 状態コード。HTTP エラー コードの詳細については、「[エラー](errors.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="09e3d-p104">Status code - An HTTP status code that indicates success or failure. For details about HTTP error codes, see [Errors](errors.md).</span></span>
* <span data-ttu-id="09e3d-p105">応答メッセージ - 要求したデータ、または操作の結果。応答メッセージは、いくつかの操作で空になる場合があります。</span><span class="sxs-lookup"><span data-stu-id="09e3d-p105">Response message - The data that you requested or the result of the operation. The response message can be empty for some operations.</span></span>
* <span data-ttu-id="09e3d-p106">`nextLink` - 要求が大量のデータを返す場合は、`@odata.nextLink` で返される URL を使用して応答をページングする必要があります。詳細については、「[ページング](paging.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="09e3d-p106">`nextLink` link - If your request returns a lot of data, you need to page through it by choosing `@odata.nextLink`. For details, see [Paging](paging.md).</span></span>

## <a name="http-methods"></a><span data-ttu-id="09e3d-123">HTTP メソッド</span><span class="sxs-lookup"><span data-stu-id="09e3d-123">HTTP methods</span></span>

<span data-ttu-id="09e3d-p107">Microsoft Graph は、要求で HTTP メソッドを使用し、要求が何を行っているかを特定します。API は次のメソッドをサポートしています。</span><span class="sxs-lookup"><span data-stu-id="09e3d-p107">Microsoft Graph uses the HTTP method on your request to determine what your request is doing. The API supports the following methods.</span></span>


|<span data-ttu-id="09e3d-126">**メソッド**</span><span class="sxs-lookup"><span data-stu-id="09e3d-126">**Method**</span></span> |<span data-ttu-id="09e3d-127">**説明**</span><span class="sxs-lookup"><span data-stu-id="09e3d-127">**Description**</span></span>                             |
| :----- | :------------------------------------------- |
| <span data-ttu-id="09e3d-128">GET</span><span class="sxs-lookup"><span data-stu-id="09e3d-128">GET</span></span>    | <span data-ttu-id="09e3d-129">リソースからデータを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="09e3d-129">Read data from a resource.</span></span>                   |
| <span data-ttu-id="09e3d-130">POST</span><span class="sxs-lookup"><span data-stu-id="09e3d-130">POST</span></span>   | <span data-ttu-id="09e3d-131">新しいリソースを作成、または処理を実行します。</span><span class="sxs-lookup"><span data-stu-id="09e3d-131">Create a new resource, or perform an action.</span></span> |
| <span data-ttu-id="09e3d-132">PATCH</span><span class="sxs-lookup"><span data-stu-id="09e3d-132">PATCH</span></span>  | <span data-ttu-id="09e3d-133">リソースを新しい値で更新します。</span><span class="sxs-lookup"><span data-stu-id="09e3d-133">Update a resource with new values.</span></span>           |
| <span data-ttu-id="09e3d-134">PUT</span><span class="sxs-lookup"><span data-stu-id="09e3d-134">PUT</span></span>    | <span data-ttu-id="09e3d-135">リソースを新しいものと置換します。</span><span class="sxs-lookup"><span data-stu-id="09e3d-135">Replace a resource with a new one.</span></span>           |
| <span data-ttu-id="09e3d-136">DELETE</span><span class="sxs-lookup"><span data-stu-id="09e3d-136">DELETE</span></span> | <span data-ttu-id="09e3d-137">リソースを削除します。</span><span class="sxs-lookup"><span data-stu-id="09e3d-137">Remove a resource.</span></span>                           |

* <span data-ttu-id="09e3d-138">CRUD メソッドの `GET` と `DELETE` では、要求本文は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="09e3d-138">For the methods `GET` and `DELETE`, no request body is required.</span></span>
* <span data-ttu-id="09e3d-139">`POST`、`PATCH`、および `PUT` メソッドは、通常 JSON 形式で指定されている要求本文を必要とし、それには、リソースのプロパティの値などの追加の情報が含まれます。</span><span class="sxs-lookup"><span data-stu-id="09e3d-139">The `POST`, `PATCH`, and `PUT` methods require a request body, usually specified in JSON format, that contains additional information, such as the values for properties of the resource.</span></span>

## <a name="version"></a><span data-ttu-id="09e3d-140">バージョン</span><span class="sxs-lookup"><span data-stu-id="09e3d-140">Version</span></span>

<span data-ttu-id="09e3d-141">Microsoft Graph は、現在 `v1.0` と `beta` の 2 つのバージョンをサポートしています。</span><span class="sxs-lookup"><span data-stu-id="09e3d-141">Microsoft Graph currently supports two versions: `v1.0` and `beta`.</span></span>

* <span data-ttu-id="09e3d-p108">`v1.0` には、一般公開されている API が含まれます。すべての運用アプリで、v1.0 バージョンを使用します。</span><span class="sxs-lookup"><span data-stu-id="09e3d-p108">`v1.0` includes generally available APIs. Use the v1.0 version for all production apps.</span></span>
* <span data-ttu-id="09e3d-p109">`beta` には、現在プレビュー段階の API が含まれます。ベータ版 API に重大な変更を導入する可能性があるため、開発中のアプリのテストにのみ、ベータ版を使用することをお勧めします。運用アプリでは、ベータ版 API を使用しないでください。</span><span class="sxs-lookup"><span data-stu-id="09e3d-p109">`beta` includes APIs that are currently in preview. Because we might introduce breaking changes to our beta APIs, we recommend that you use the beta version only to test apps that are in development; do not use beta APIs in your production apps.</span></span>

<span data-ttu-id="09e3d-p110">ベータ版 API のフィードバックを常に募集しています。フィードバックの提供または機能のご要望は、「[UserVoice](https://officespdev.uservoice.com/)」ページを参照してください。</span><span class="sxs-lookup"><span data-stu-id="09e3d-p110">We are always looking for feedback on our beta APIs. To provide feedback or request features, see our [UserVoice](https://officespdev.uservoice.com/) page.</span></span>

<span data-ttu-id="09e3d-148">API のバージョンに関する詳細については、「[バージョン管理とサポート](versioning-and-support.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="09e3d-148">For more information about API versions, see [Versioning and support](versioning-and-support.md).</span></span>

## <a name="resource"></a><span data-ttu-id="09e3d-149">リソース</span><span class="sxs-lookup"><span data-stu-id="09e3d-149">Resource</span></span>

<span data-ttu-id="09e3d-150">リソースには、エンティティまたは複合型が使用でき、一般的にプロパティを使用して定義されます。</span><span class="sxs-lookup"><span data-stu-id="09e3d-150">A resource can be an entity or complex type, commonly defined with properties.</span></span> <span data-ttu-id="09e3d-151">エンティティは、常に "**id**" プロパティが含まれる点において、複合型とは異なります。</span><span class="sxs-lookup"><span data-stu-id="09e3d-151">Entities differ from complex types by always including an **id** property.</span></span>

<span data-ttu-id="09e3d-152">ユーザーの URL には、要求で操作するリソースが含まれます。たとえば、`me`、**user**、**group**、**drive**、**site** などです。</span><span class="sxs-lookup"><span data-stu-id="09e3d-152">Your URL will include the resource or resources you are interacting with in the request, such as `me`, \*\*\*\*, \*\*\*\*, \*\*\*\*, and \*\*\*\*.</span></span> <span data-ttu-id="09e3d-153">多くの場合、最上位のリソースには _リレーションシップ_も含まれます。`me/messages` または `me/drive` のように、追加のリソースにアクセスするのに使用できます。</span><span class="sxs-lookup"><span data-stu-id="09e3d-153">Each of the top-level resources also include _relationships_, which you can use to access additional resources, like `me/messages` or `me/drive`.</span></span> <span data-ttu-id="09e3d-154">_メソッド_を使用して、リソースを操作することもできます。たとえば、電子メールを送信するには `me/sendMail` を使用します。</span><span class="sxs-lookup"><span data-stu-id="09e3d-154">You can also interact with resources using _methods_; for example, to send an email, use `me/sendMail`.</span></span> <span data-ttu-id="09e3d-155">詳細については、「[Microsoft Graph 内を移動してデータとメソッドにアクセスする](traverse-the-graph.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="09e3d-155">For more information, see [Access data and methods by navigating Microsoft Graph](traverse-the-graph.md).</span></span>

<span data-ttu-id="09e3d-p113">各リソースにアクセスするために異なるアクセス許可が必要になる可能性があります。リソースの作成または更新には、リソースの読み取りよりも高いレベルのアクセス許可が必要になります。必要なアクセス許可に関する詳細については、メソッドの参照トピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="09e3d-p113">Each resource might require different permissions to access it. You will often need a higher level of permissions to create or update a resource than to read it. For details about required permissions, see the method reference topic.</span></span> 

<span data-ttu-id="09e3d-159">アクセス許可に関する詳細については、「[アクセス許可の参照](permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="09e3d-159">For details about permissions, see [Permissions reference](permissions-reference.md).</span></span>

## <a name="query-parameters"></a><span data-ttu-id="09e3d-160">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="09e3d-160">Query parameters</span></span>

<span data-ttu-id="09e3d-161">クエリ パラメーターには、OData のシステム クエリ オプション、または応答をカスタマイズするためにメソッドが受け入れる文字列を使用できます。</span><span class="sxs-lookup"><span data-stu-id="09e3d-161">Query parameters can be OData system query options, or other strings that a method accepts to customize its response.</span></span>

<span data-ttu-id="09e3d-162">省略可能の OData のシステム クエリ オプションを使用すると、既定の応答よりも多い、または少ないプロパティを含めたり、カスタム クエリに一致するアイテムについて応答をフィルター処理したり、メソッドの追加のパラメーターを提供したりできます。</span><span class="sxs-lookup"><span data-stu-id="09e3d-162">You can use optional query parameters to customize the response in your Microsoft Graph app. Use query parameters to include more or fewer properties than the default response, filter the response for items that match a custom query, or provide additional parameters for a method.</span></span>

<span data-ttu-id="09e3d-163">たとえば、次の `filter` パラメーターを追加すると、`jon@contoso.com` の `emailAddress` プロパティを持つメッセージのみが返されるように制限できます。</span><span class="sxs-lookup"><span data-stu-id="09e3d-163">For example, adding the following filter parameter restricts the messages returned to only those with the  property of .</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages?filter=emailAddress eq 'jon@contoso.com'
```

<span data-ttu-id="09e3d-164">OData クエリ オプションの詳細については、「[Use query parameters to customize responses (クエリパラメーターを使用して応答をカスタマイズする)](query-parameters.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="09e3d-164">For more information about OData query options, see [Use query parameters to customize responses](query-parameters.md).</span></span>

<span data-ttu-id="09e3d-165">OData クエリ オプション以外に、一部のメソッドでは、クエリ URL の一部としてパラメーター値を指定することが要求されます。</span><span class="sxs-lookup"><span data-stu-id="09e3d-165">Aside from OData query options, some methods require parameter values specified as part of the query URL.</span></span> <span data-ttu-id="09e3d-166">たとえば、ある一定期間内にユーザーの予定表で発生したイベントのコレクションを取得するには、クエリ パラメーターとして `startDateTime` と `endDateTime` の値を使用して期間を指定し、**user** の **calendarView** リレーションシップに対してクエリを実行します。</span><span class="sxs-lookup"><span data-stu-id="09e3d-166">For example, you can get a collection of events that occurred during a time period in a user's calendar, by querying the **calendarView** relationship of a **user**, and specifying the period `startDateTime` and `endDateTime` values as query parameters:</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/me/calendarView?startDateTime=2019-09-01T09:00:00.0000000&endDateTime=2019-09-01T17:00:00.0000000
```

## <a name="next-steps"></a><span data-ttu-id="09e3d-167">次のステップ</span><span class="sxs-lookup"><span data-stu-id="09e3d-167">Next steps</span></span>

<span data-ttu-id="09e3d-p115">Microsoft Graph を使用して、起動および実行する準備ができました。詳細について知るには、[Graph エクスプローラー](https://developer.microsoft.com/graph/graph-explorer)に移動して、いくつかの要求や[クイック スタート](https://developer.microsoft.com/graph/quick-start)を試したり、「[SDK とコード サンプル](https://developer.microsoft.com/graph/code-samples-and-sdks)」のいずれかを使用して開始したりします。</span><span class="sxs-lookup"><span data-stu-id="09e3d-p115">You're ready to get up and running with Microsoft Graph. To learn more, go to the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer) to try out some requests, try the [Quick Start](https://developer.microsoft.com/graph/quick-start), or get started using one of our [SDKs and code samples](https://developer.microsoft.com/graph/code-samples-and-sdks).</span></span>
