---
title: Microsoft Graph API を使用する
description: Microsoft Graph は、Microsoft Cloud サービス リソースへのアクセスを可能にする RESTful Web API です。アプリを登録 して、サービス または ユーザーの認証トークンを取得する と、Microsoft Graph API に対して要求を行うことができます。
ms.openlocfilehash: 1a9d9bcefdfb302a9de602aa15aa642a0c57a793
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092498"
---
# <a name="use-the-microsoft-graph-api"></a><span data-ttu-id="6d927-104">Microsoft Graph API を使用する</span><span class="sxs-lookup"><span data-stu-id="6d927-104">Use the Microsoft Graph API</span></span>

<span data-ttu-id="6d927-p102">Microsoft Graph は、Microsoft Cloud サービス リソースへのアクセスを可能にする RESTful Web API です。[アプリを登録](auth-register-app-v2.md) して、[サービス](auth-v2-service.md) または [ユーザーの認証トークンを取得する](auth-v2-user.md) と、Microsoft Graph API に対して要求を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="6d927-p102">Microsoft Graph is a RESTful web API that enables you to access Microsoft Cloud service resources. After you [register your app](auth-register-app-v2.md) and [get authentication tokens for a user](auth-v2-user.md) or [service](auth-v2-service.md), you can make requests to the Microsoft Graph API.</span></span>

> <span data-ttu-id="6d927-107">**重要:** 条件付きアクセス ポリシーの Microsoft Graph への適用方法は変更されています。</span><span class="sxs-lookup"><span data-stu-id="6d927-107">**Important:**  How conditional access policies apply to Microsoft Graph is changing.</span></span> <span data-ttu-id="6d927-108">条件付きアクセス ポリシーが構成されるシナリオを処理するよう、アプリケーションを更新する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6d927-108">Applications need to be updated to handle scenarios where conditional access policies are configured.</span></span> <span data-ttu-id="6d927-109">詳細およびガイダンスについては、「[Azure Active Directory の条件付きアクセスについての開発者ガイド](https://docs.microsoft.com/azure/active-directory/develop/active-directory-conditional-access-developer)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6d927-109">For more information and guidance, see [Developer Guidance for Azure Active Directory Conditional Access](https://docs.microsoft.com/azure/active-directory/develop/active-directory-conditional-access-developer).</span></span>

<span data-ttu-id="6d927-110">ユーザーや電子メール メッセージなど、リソースの読み取りや書き込みを行うには、次のような要求を構築します。</span><span class="sxs-lookup"><span data-stu-id="6d927-110">To read from or write to a resource such as a user or an email message, you construct a request that looks like the following.</span></span>

```http
https://graph.microsoft.com/{version}/{resource}?query-parameters
```

<span data-ttu-id="6d927-111">要求のコンポーネントには以下が含まれます。</span><span class="sxs-lookup"><span data-stu-id="6d927-111">The components of a request include:</span></span>

* <span data-ttu-id="6d927-112">[HTTP メソッド](#http-methods) - Microsoft Graph への要求で使用する HTTP メソッド。</span><span class="sxs-lookup"><span data-stu-id="6d927-112">[HTTP method](#http-methods) - The HTTP method used on the request to Microsoft Graph.</span></span>
* <span data-ttu-id="6d927-113">[`{version}`](#version) - アプリケーションが使用している Microsoft Graph API のバージョン。</span><span class="sxs-lookup"><span data-stu-id="6d927-113">[`{version}`](#version) - The version of the Microsoft Graph API your application is using.</span></span>
* <span data-ttu-id="6d927-114">[`{resource}`](#resource) - ユーザーが参照している Microsoft Graph のリソース。</span><span class="sxs-lookup"><span data-stu-id="6d927-114">[`{resource}`](#resource) - The resource in Microsoft Graph that you're referencing.</span></span>
* <span data-ttu-id="6d927-115">[クエリ パラメーター](#query-parameters-optional) - 要求または応答を変更するパラメーターのオプションのセット。</span><span class="sxs-lookup"><span data-stu-id="6d927-115">[query-parameters](#query-parameters-optional) - An optional set of parameters to modify the request or response.</span></span>

<span data-ttu-id="6d927-116">要求を行うと、次を含む応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="6d927-116">After you make a request, a response is returned that includes:</span></span> 

* <span data-ttu-id="6d927-p104">状態コード - 成功または失敗を示す HTTP 状態コード。HTTP エラー コードの詳細については、「[エラー](errors.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6d927-p104">Status code - An HTTP status code that indicates success or failure. For details about HTTP error codes, see [Errors](errors.md).</span></span>
* <span data-ttu-id="6d927-p105">応答メッセージ - 要求したデータ、または操作の結果。応答メッセージは、いくつかの操作で空になる場合があります。</span><span class="sxs-lookup"><span data-stu-id="6d927-p105">Response message - The data that you requested or the result of the operation. The response message can be empty for some operations.</span></span>
* <span data-ttu-id="6d927-p106">**[次へ]** リンク - 要求が大量のデータを返す場合は、[**次ヘ**] を選択して、ページを進める必要があります。詳細については、「[ページング](paging.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6d927-p106">**Next** link - If your request returns a lot of data, you need to page through it by choosing **Next**. For details, see [Paging](paging.md).</span></span>

## <a name="http-methods"></a><span data-ttu-id="6d927-123">HTTP メソッド</span><span class="sxs-lookup"><span data-stu-id="6d927-123">HTTP methods</span></span>

<span data-ttu-id="6d927-p107">Microsoft Graph は、要求で HTTP メソッドを使用し、要求が何を行っているかを特定します。API は次のメソッドをサポートしています。</span><span class="sxs-lookup"><span data-stu-id="6d927-p107">Microsoft Graph uses the HTTP method on your request to determine what your request is doing. The API supports the following methods.</span></span>


|<span data-ttu-id="6d927-126">**メソッド**</span><span class="sxs-lookup"><span data-stu-id="6d927-126">**Method**</span></span> |<span data-ttu-id="6d927-127">**説明**</span><span class="sxs-lookup"><span data-stu-id="6d927-127">**Description**</span></span>                             |
| :----- | :------------------------------------------- |
| <span data-ttu-id="6d927-128">GET</span><span class="sxs-lookup"><span data-stu-id="6d927-128">GET</span></span>    | <span data-ttu-id="6d927-129">リソースからデータを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="6d927-129">Read data from a resource.</span></span>                   |
| <span data-ttu-id="6d927-130">POST</span><span class="sxs-lookup"><span data-stu-id="6d927-130">POST</span></span>   | <span data-ttu-id="6d927-131">新しいリソースを作成、または処理を実行します。</span><span class="sxs-lookup"><span data-stu-id="6d927-131">Create a new resource, or perform an action.</span></span> |
| <span data-ttu-id="6d927-132">PATCH</span><span class="sxs-lookup"><span data-stu-id="6d927-132">PATCH</span></span>  | <span data-ttu-id="6d927-133">リソースを新しい値で更新します。</span><span class="sxs-lookup"><span data-stu-id="6d927-133">Update a resource with new values.</span></span>           |
| <span data-ttu-id="6d927-134">PUT</span><span class="sxs-lookup"><span data-stu-id="6d927-134">PUT</span></span>    | <span data-ttu-id="6d927-135">リソースを新しいものと置換します。</span><span class="sxs-lookup"><span data-stu-id="6d927-135">Replace a resource with a new one.</span></span>           |
| <span data-ttu-id="6d927-136">DELETE</span><span class="sxs-lookup"><span data-stu-id="6d927-136">DELETE</span></span> | <span data-ttu-id="6d927-137">リソースを削除します。</span><span class="sxs-lookup"><span data-stu-id="6d927-137">Remove a resource.</span></span>                           |

* <span data-ttu-id="6d927-138">メソッド **GET** と **DELETE** では、要求本文は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="6d927-138">For the methods **GET** and **DELETE**, no request body is required.</span></span>
* <span data-ttu-id="6d927-139">**POST**、**PATCH**、および **PUT** メソッドは、通常 JSON 形式で指定されている要求本文を必要とし、それには、リソースのプロパティの値などの追加の情報が含まれます。</span><span class="sxs-lookup"><span data-stu-id="6d927-139">The **POST**, **PATCH**, and **PUT** methods require a request body, usually specified in JSON format, that contains additional information, such as the values for properties of the resource.</span></span>

## <a name="version"></a><span data-ttu-id="6d927-140">バージョン</span><span class="sxs-lookup"><span data-stu-id="6d927-140">Version</span></span>

<span data-ttu-id="6d927-141">Microsoft Graph は、現在 `v1.0` と `beta` の 2 つのバージョンをサポートしています。</span><span class="sxs-lookup"><span data-stu-id="6d927-141">Microsoft Graph currently supports two versions: `v1.0` and `beta`.</span></span>

* <span data-ttu-id="6d927-p108">`v1.0` には、一般公開されている API が含まれます。すべての運用アプリで、v1.0 バージョンを使用します。</span><span class="sxs-lookup"><span data-stu-id="6d927-p108">`v1.0` includes generally available APIs. Use the v1.0 version for all production apps.</span></span>
* <span data-ttu-id="6d927-p109">`beta` には、現在プレビュー段階の API が含まれます。ベータ版 API に重大な変更を導入する可能性があるため、開発中のアプリのテストにのみ、ベータ版を使用することをお勧めします。運用アプリでは、ベータ版 API を使用しないでください。</span><span class="sxs-lookup"><span data-stu-id="6d927-p109">`beta` includes APIs that are currently in preview. Because we might introduce breaking changes to our beta APIs, we recommend that you use the beta version only to test apps that are in development; do not use beta APIs in your production apps.</span></span>

<span data-ttu-id="6d927-p110">ベータ版 API のフィードバックを常に募集しています。フィードバックの提供または機能のご要望は、「[UserVoice](https://officespdev.uservoice.com/)」ページを参照してください。</span><span class="sxs-lookup"><span data-stu-id="6d927-p110">We are always looking for feedback on our beta APIs. To provide feedback or request features, see our [UserVoice](https://officespdev.uservoice.com/) page.</span></span>

<span data-ttu-id="6d927-148">API のバージョンに関する詳細については、「[バージョン管理とサポート](versioning-and-support.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6d927-148">For more information about API versions, see [Versioning and support](versioning-and-support.md).</span></span>

## <a name="resource"></a><span data-ttu-id="6d927-149">リソース</span><span class="sxs-lookup"><span data-stu-id="6d927-149">Resource</span></span>

<span data-ttu-id="6d927-p111">ユーザーの URL には、要求で操作するリソースが含まれます。たとえば、`me`、`users`、`groups`、`drives`、`sites` などです。最上位のリソースそれぞれにも、**リレーションシップ**が含まれます。`me/messages` または `me/drive` のように、追加のリソースにアクセスするのに使用できます。**メソッド** を使用して、リソースを操作することもできます。たとえば、電子メールを送信するには `me/sendMail` を使用します。</span><span class="sxs-lookup"><span data-stu-id="6d927-p111">Your URL will include the resource or resources you are interacting with in the request, such as `me`, `users`, `groups`, `drives`, and `sites`. Each of the top-level resources also include **relationships**, which you can use to access additional resources, like `me/messages` or `me/drive`. You can also interact with resources using **methods**; for example, to send an email, use `me/sendMail`.</span></span>

<span data-ttu-id="6d927-153">リソースのリレーションシップおよびメソッドを移動する方法の詳細については、「[グラフをスキャンする](traverse-the-graph.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6d927-153">For more information about how to navigate resource relationships and methods, see [Traverse the graph](traverse-the-graph.md).</span></span> 

<span data-ttu-id="6d927-p112">各リソースにアクセスするために異なるアクセス許可が必要になる可能性があります。リソースの作成または更新には、リソースの読み取りよりも高いレベルのアクセス許可が必要になります。必要なアクセス許可に関する詳細については、メソッドの参照トピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="6d927-p112">Each resource might require different permissions to access it. You will often need a higher level of permissions to create or update a resource than to read it. For details about required permissions, see the method reference topic.</span></span> 

<span data-ttu-id="6d927-157">アクセス許可に関する詳細については、「[アクセス許可の参照](permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6d927-157">For details about permissions, see [Permissions reference](permissions-reference.md).</span></span>

## <a name="query-parameters-optional"></a><span data-ttu-id="6d927-158">クエリ パラメーター (オプション)</span><span class="sxs-lookup"><span data-stu-id="6d927-158">Query parameters (optional)</span></span>

<span data-ttu-id="6d927-p113">Microsoft Graph アプリで応答をカスタマイズするには、オプションのクエリ パラメーターを使用できます。クエリ パラメーターを使用して、既定の応答よりも多い、または少ないプロパティを含めたり、カスタム クエリに一致するアイテムの応答をフィルター処理したり、メソッドの追加のパラメーターを提供したりします。</span><span class="sxs-lookup"><span data-stu-id="6d927-p113">You can use optional query parameters to customize the response in your Microsoft Graph app. Use query parameters to include more or fewer properties than the default response, filter the response for items that match a custom query, or provide additional parameters for a method.</span></span>

<span data-ttu-id="6d927-161">たとえば、次のフィルター パラメーターを追加すると、メッセージが `jon@contoso.com` の `emailAddress` プロパティを持つものだけに返されるよう制限されます。</span><span class="sxs-lookup"><span data-stu-id="6d927-161">For example, adding the following filter parameter restricts the messages returned to only those with the `emailAddress` property of `jon@contoso.com`.</span></span>

```http
https://graph.microsoft.com/v1.0/me/messages?filter=emailAddress eq 'jon@contoso.com'
```

<span data-ttu-id="6d927-162">クエリ パラメーターに関する詳細については、「[応答をカスタマイズする](query-parameters.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6d927-162">For more information about query parameters, see [Customize responses](query-parameters.md).</span></span>

## <a name="next-steps"></a><span data-ttu-id="6d927-163">次のステップ</span><span class="sxs-lookup"><span data-stu-id="6d927-163">Next steps</span></span>

<span data-ttu-id="6d927-p114">Microsoft Graph を使用して、起動および実行する準備ができました。詳細について知るには、[Graph エクスプローラー](https://developer.microsoft.com/graph/graph-explorer)に移動して、いくつかの要求や[クイック スタート](https://developer.microsoft.com/graph/quick-start)を試したり、「[SDK とコード サンプル](https://developer.microsoft.com/graph/code-samples-and-sdks)」のいずれかを使用して開始したりします。</span><span class="sxs-lookup"><span data-stu-id="6d927-p114">You're ready to get up and running with Microsoft Graph. To learn more, go to the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer) to try out some requests, try the [Quick Start](https://developer.microsoft.com/graph/quick-start), or get started using one of our [SDKs and code samples](https://developer.microsoft.com/graph/code-samples-and-sdks).</span></span>
