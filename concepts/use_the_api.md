# <a name="use-the-microsoft-graph-api"></a><span data-ttu-id="e4c0d-101">Microsoft Graph API を使用する</span><span class="sxs-lookup"><span data-stu-id="e4c0d-101">Use the Microsoft Graph API</span></span>

<span data-ttu-id="e4c0d-102">Microsoft Graph は、Microsoft Cloud サービス リソースへのアクセスを可能にする RESTful Web API です。</span><span class="sxs-lookup"><span data-stu-id="e4c0d-102">Microsoft Graph is a RESTful web API that enables you to access Microsoft Cloud service resources.</span></span> <span data-ttu-id="e4c0d-103">[アプリを登録](auth_register_app_v2.md) して、[サービス](auth_v2_service.md) または [ユーザーの認証トークンを取得する](auth_v2_user.md) と、Microsoft Graph API に対して要求を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="e4c0d-103">After you [register your app](auth_register_app_v2.md) and [get authentication tokens for a user](auth_v2_user.md) or [service](auth_v2_service.md), you can make requests to the Microsoft Graph API.</span></span>

> <span data-ttu-id="e4c0d-104">**重要:**条件付きアクセス ポリシーの Microsoft Graph への適用方法は変更されています。</span><span class="sxs-lookup"><span data-stu-id="e4c0d-104">**Important:**  How conditional access policies apply to Microsoft Graph is changing.</span></span> <span data-ttu-id="e4c0d-105">条件付きアクセス ポリシーが構成されるシナリオを処理するよう、アプリケーションを更新する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e4c0d-105">Applications need to be updated to handle scenarios where conditional access policies are configured.</span></span> <span data-ttu-id="e4c0d-106">詳細およびガイダンスについては、「[Azure Active Directory の条件付きアクセスについての開発者ガイド]((https://docs.microsoft.com/azure/active-directory/develop/active-directory-conditional-access-developer))」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e4c0d-106">For more information and guidance, see [Developer Guidance for Azure Active Directory Conditional Access]((https://docs.microsoft.com/azure/active-directory/develop/active-directory-conditional-access-developer)).</span></span>

<span data-ttu-id="e4c0d-107">ユーザーや電子メール メッセージなど、リソースの読み取りや書き込みを行うには、次のような要求を構築します。</span><span class="sxs-lookup"><span data-stu-id="e4c0d-107">To read from or write to a resource such as a user or an email message, you construct a request that looks like the following.</span></span>

```http
https://graph.microsoft.com/{version}/{resource}?query-parameters
```

<span data-ttu-id="e4c0d-108">要求のコンポーネントには以下が含まれます。</span><span class="sxs-lookup"><span data-stu-id="e4c0d-108">The components of a request include:</span></span>

* <span data-ttu-id="e4c0d-109">[HTTP メソッド](#http-methods) - Microsoft Graph への要求で使用する HTTP メソッド。</span><span class="sxs-lookup"><span data-stu-id="e4c0d-109">[HTTP method](#http-methods) - The HTTP method used on the request to Microsoft Graph.</span></span>
* <span data-ttu-id="e4c0d-110">[`{version}`](#version) - アプリケーションが使用している Microsoft Graph API のバージョン。</span><span class="sxs-lookup"><span data-stu-id="e4c0d-110">[`{version}`](#version) - The version of the Microsoft Graph API your application is using.</span></span>
* <span data-ttu-id="e4c0d-111">[`{resource}`](#resource) - ユーザーが参照している Microsoft Graph のリソース。</span><span class="sxs-lookup"><span data-stu-id="e4c0d-111">[`{resource}`](#resource) - The resource in Microsoft Graph that you're referencing.</span></span>
* <span data-ttu-id="e4c0d-112">[クエリ パラメーター](#query-parameters-optional) - 要求または応答を変更するパラメーターのオプションのセット。</span><span class="sxs-lookup"><span data-stu-id="e4c0d-112">[query-parameters](#query-parameters-optional) - An optional set of parameters to modify the request or response.</span></span>

<span data-ttu-id="e4c0d-113">要求を行うと、次を含む応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="e4c0d-113">After you make a request, a response is returned that includes:</span></span> 

* <span data-ttu-id="e4c0d-114">状態コード - 成功または失敗を示す HTTP 状態コード。</span><span class="sxs-lookup"><span data-stu-id="e4c0d-114">Status code - An HTTP status code that indicates success or failure.</span></span> <span data-ttu-id="e4c0d-115">HTTP エラー コードの詳細については、「[エラー](errors.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e4c0d-115">For details about HTTP error codes, see [Errors](errors.md).</span></span>
* <span data-ttu-id="e4c0d-p104">応答メッセージ - 要求したデータ、または操作の結果。応答メッセージは、いくつかの操作で空になる場合があります。</span><span class="sxs-lookup"><span data-stu-id="e4c0d-p104">Response message - The data that you requested or the result of the operation. The response message can be empty for some operations.</span></span>
* <span data-ttu-id="e4c0d-118">**[次へ]** リンク - 要求が大量のデータを返す場合は、**[次ヘ]** を選択して、ページを進める必要があります。</span><span class="sxs-lookup"><span data-stu-id="e4c0d-118">**Next** link - If your request returns a lot of data, you need to page through it by choosing **Next**.</span></span> <span data-ttu-id="e4c0d-119">詳細については、「[ページング](paging.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e4c0d-119">For details, see [Paging](paging.md).</span></span>

## <a name="http-methods"></a><span data-ttu-id="e4c0d-120">HTTP メソッド</span><span class="sxs-lookup"><span data-stu-id="e4c0d-120">HTTP methods</span></span>

<span data-ttu-id="e4c0d-p106">Microsoft Graph は、要求で HTTP メソッドを使用し、要求が何を行っているかを特定します。API は次のメソッドをサポートしています。</span><span class="sxs-lookup"><span data-stu-id="e4c0d-p106">Microsoft Graph uses the HTTP method on your request to determine what your request is doing. The API supports the following methods.</span></span>


|<span data-ttu-id="e4c0d-123">**メソッド**</span><span class="sxs-lookup"><span data-stu-id="e4c0d-123">**Method**</span></span> |<span data-ttu-id="e4c0d-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="e4c0d-124">**Description**</span></span>                             |
| :----- | :------------------------------------------- |
| <span data-ttu-id="e4c0d-125">GET</span><span class="sxs-lookup"><span data-stu-id="e4c0d-125">GET</span></span>    | <span data-ttu-id="e4c0d-126">リソースからデータを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e4c0d-126">Read data from a resource.</span></span>                   |
| <span data-ttu-id="e4c0d-127">POST</span><span class="sxs-lookup"><span data-stu-id="e4c0d-127">POST</span></span>   | <span data-ttu-id="e4c0d-128">新しいリソースを作成、または処理を実行します。</span><span class="sxs-lookup"><span data-stu-id="e4c0d-128">Create a new resource, or perform an action.</span></span> |
| <span data-ttu-id="e4c0d-129">PATCH</span><span class="sxs-lookup"><span data-stu-id="e4c0d-129">PATCH</span></span>  | <span data-ttu-id="e4c0d-130">リソースを新しい値で更新します。</span><span class="sxs-lookup"><span data-stu-id="e4c0d-130">Update a resource with new values.</span></span>           |
| <span data-ttu-id="e4c0d-131">PUT</span><span class="sxs-lookup"><span data-stu-id="e4c0d-131">PUT</span></span>    | <span data-ttu-id="e4c0d-132">リソースを新しいものと置換します。</span><span class="sxs-lookup"><span data-stu-id="e4c0d-132">Replace a resource with a new one.</span></span>           |
| <span data-ttu-id="e4c0d-133">DELETE</span><span class="sxs-lookup"><span data-stu-id="e4c0d-133">DELETE</span></span> | <span data-ttu-id="e4c0d-134">リソースを削除します。</span><span class="sxs-lookup"><span data-stu-id="e4c0d-134">Remove a resource.</span></span>                           |

* <span data-ttu-id="e4c0d-135">メソッド **GET** と **DELETE** では、要求本文は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="e4c0d-135">For the methods **GET** and **DELETE**, no request body is required.</span></span>
* <span data-ttu-id="e4c0d-136">**POST**、**PATCH**、および **PUT** メソッドは、通常 JSON 形式で指定されている要求本文を必要とし、それには、リソースのプロパティの値などの追加の情報が含まれます。</span><span class="sxs-lookup"><span data-stu-id="e4c0d-136">The **POST**, **PATCH**, and **PUT** methods require a request body, usually specified in JSON format, that contains additional information, such as the values for properties of the resource.</span></span>

## <a name="version"></a><span data-ttu-id="e4c0d-137">バージョン</span><span class="sxs-lookup"><span data-stu-id="e4c0d-137">Version</span></span>

<span data-ttu-id="e4c0d-138">Microsoft Graph は、現在 `v1.0` と `beta` の 2 つのバージョンをサポートしています。</span><span class="sxs-lookup"><span data-stu-id="e4c0d-138">Microsoft Graph currently supports two versions: `v1.0` and `beta`.</span></span>

* <span data-ttu-id="e4c0d-139">`v1.0` には、一般公開されている API が含まれます。</span><span class="sxs-lookup"><span data-stu-id="e4c0d-139">`v1.0` includes generally available APIs.</span></span> <span data-ttu-id="e4c0d-140">すべての運用アプリで、v1.0 バージョンを使用します。</span><span class="sxs-lookup"><span data-stu-id="e4c0d-140">Use the v1.0 version for all production apps.</span></span>
* <span data-ttu-id="e4c0d-141">`beta` には、現在プレビュー段階の API が含まれます。</span><span class="sxs-lookup"><span data-stu-id="e4c0d-141">`beta` includes APIs that are currently in preview.</span></span> <span data-ttu-id="e4c0d-142">ベータ版 API に重大な変更を導入する可能性があるため、開発中のアプリのテストにのみ、ベータ版を使用することをお勧めします。運用アプリでは、ベータ版 API を使用しないでください。</span><span class="sxs-lookup"><span data-stu-id="e4c0d-142">Because we might introduce breaking changes to our beta APIs, we recommend that you use the beta version only to test apps that are in development; do not use beta APIs in your production apps.</span></span>

<span data-ttu-id="e4c0d-143">ベータ版 API のフィードバックを常に募集しています。</span><span class="sxs-lookup"><span data-stu-id="e4c0d-143">We are always looking for feedback on our beta APIs.</span></span> <span data-ttu-id="e4c0d-144">フィードバックの提供または機能のご要望は、「[UserVoice]((https://officespdev.uservoice.com/))」ページを参照してください。</span><span class="sxs-lookup"><span data-stu-id="e4c0d-144">To provide feedback or request features, see our [UserVoice]((https://officespdev.uservoice.com/)) page.</span></span>

<span data-ttu-id="e4c0d-145">API のバージョンに関する詳細については、「[バージョン管理とサポート](versioning_and_support.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e4c0d-145">For more information about API versions, see [Versioning and support](versioning_and_support.md).</span></span>

## <a name="resource"></a><span data-ttu-id="e4c0d-146">リソース</span><span class="sxs-lookup"><span data-stu-id="e4c0d-146">Resource</span></span>

<span data-ttu-id="e4c0d-147">ユーザーの URL には、要求で操作するリソースが含まれます。たとえば、`me`、`users`、`groups`、`drives`、`sites` などです。</span><span class="sxs-lookup"><span data-stu-id="e4c0d-147">Your URL will include the resource or resources you are interacting with in the request, such as `me`, `users`, `groups`, `drives`, and `sites`.</span></span> <span data-ttu-id="e4c0d-148">最上位のリソースそれぞれにも、**リレーションシップ**が含まれます。`me/messages` または `me/drive` のように、追加のリソースにアクセスするのに使用できます。</span><span class="sxs-lookup"><span data-stu-id="e4c0d-148">Each of the top-level resources also include **relationships**, which you can use to access additional resources, like `me/messages` or `me/drive`.</span></span> <span data-ttu-id="e4c0d-149">**メソッド**を使用して、リソースを操作することもできます。たとえば、電子メールを送信するには `me/sendMail` を使用します。</span><span class="sxs-lookup"><span data-stu-id="e4c0d-149">You can also interact with resources using **methods**; for example, to send an email, use `me/sendMail`.</span></span>

<span data-ttu-id="e4c0d-150">リソースのリレーションシップおよびメソッドを移動する方法に関する詳細については、「[グラフをスキャンする](traverse_the_graph.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e4c0d-150">For more information about how to navigate resource relationships and methods, see Traverse the graph.</span></span> 

<span data-ttu-id="e4c0d-p111">各リソースにアクセスするために異なるアクセス許可が必要になる可能性があります。リソースの作成または更新には、リソースの読み取りよりも高いレベルのアクセス許可が必要になります。必要なアクセス許可に関する詳細については、メソッドの参照トピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="e4c0d-p111">Each resource might require different permissions to access it. You will often need a higher level of permissions to create or update a resource than to read it. For details about required permissions, see the method reference topic.</span></span> 

<span data-ttu-id="e4c0d-154">アクセス許可に関する詳細については、「[アクセス許可の参照](permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e4c0d-154">For details about permissions, see [Permissions reference](permissions_reference.md).</span></span>

## <a name="query-parameters-optional"></a><span data-ttu-id="e4c0d-155">クエリ パラメーター (オプション)</span><span class="sxs-lookup"><span data-stu-id="e4c0d-155">Query parameters (optional)</span></span>

<span data-ttu-id="e4c0d-p112">Microsoft Graph アプリで応答をカスタマイズするには、オプションのクエリ パラメーターを使用できます。クエリ パラメーターを使用して、既定の応答よりも多い、または少ないプロパティを含めたり、カスタム クエリに一致するアイテムの応答をフィルター処理したり、メソッドの追加のパラメーターを提供したりします。</span><span class="sxs-lookup"><span data-stu-id="e4c0d-p112">You can use optional query parameters to customize the response in your Microsoft Graph app. Use query parameters to include more or fewer properties than the default response, filter the response for items that match a custom query, or provide additional parameters for a method.</span></span>

<span data-ttu-id="e4c0d-158">たとえば、次のフィルター パラメーターを追加すると、メッセージが `jon@contoso.com` の `emailAddress` プロパティを持つものだけに返されるよう制限されます。</span><span class="sxs-lookup"><span data-stu-id="e4c0d-158">For example, adding the following filter parameter restricts the messages returned to only those with the `emailAddress` property of `jon@contoso.com`.</span></span>

```http
https://graph.microsoft.com/v1.0/me/messages?filter=emailAddress eq 'jon@contoso.com'
```

<span data-ttu-id="e4c0d-159">クエリ パラメーターに関する詳細については、「[応答をカスタマイズする](query_parameters.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e4c0d-159">For more information about query parameters, see [Customize responses](query_parameters.md).</span></span>

## <a name="next-steps"></a><span data-ttu-id="e4c0d-160">次の手順</span><span class="sxs-lookup"><span data-stu-id="e4c0d-160">Next steps</span></span>

<span data-ttu-id="e4c0d-161">Microsoft Graph を使用して、起動および実行する準備ができました。</span><span class="sxs-lookup"><span data-stu-id="e4c0d-161">You're ready to get up and running with Microsoft Graph.</span></span> <span data-ttu-id="e4c0d-162">詳細について知るには、[Graph エクスプローラー]((https://developer.microsoft.com/ja-JP/graph/graph-explorer))に移動して、いくつかの要求や[クイック スタート]((https://developer.microsoft.com/ja-JP/graph/quick-start))を試したり、「[SDK とコード サンプル]((https://developer.microsoft.com/ja-JP/graph/code-samples-and-sdks))」のいずれかを使用して開始したりします。</span><span class="sxs-lookup"><span data-stu-id="e4c0d-162">To learn more, go to the [Graph Explorer]((https://developer.microsoft.com/ja-JP/graph/graph-explorer)) to try out some requests, try the [Quick Start]((https://developer.microsoft.com/ja-JP/graph/quick-start)), or get started using one of our [SDKs and code samples]((https://developer.microsoft.com/ja-JP/graph/code-samples-and-sdks)).</span></span>
