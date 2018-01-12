# <a name="microsoft-graph-throttling-guidance"></a><span data-ttu-id="46a05-101">Microsoft Graph 調整ガイド</span><span class="sxs-lookup"><span data-stu-id="46a05-101">Microsoft Graph throttling guidance</span></span>


<span data-ttu-id="46a05-p101">調整とは、リソースの使いすぎを防ぐために、サービスの同時呼び出し数を制限することをいいます。Microsoft Graph は、大量の要求を処理できるよう設計されています。過剰な数の要求が発生した場合、調整を行うことは Microsoft Graph サービスの最適なパフォーマンスと信頼性の維持に役立ちます。</span><span class="sxs-lookup"><span data-stu-id="46a05-p101">Throttling limits the number of concurrent calls to a service to prevent overuse of resources. Microsoft Graph is designed to handle a high volume of requests. If an overwhelming number of requests occurs, throttling helps maintain optimal performance and reliability of the Microsoft Graph service.</span></span>

<span data-ttu-id="46a05-p102">制限の調整はシナリオによって異なります。たとえば、大量の書き込みを行う際には、読み込みのみを行う場合に比べて調整が起こる可能性は高くなります。</span><span class="sxs-lookup"><span data-stu-id="46a05-p102">Throttling limits vary based on the scenario. For example, if you are performing a large volume of writes, the possibility for throttling is higher than if you are only performing reads.</span></span>

## <a name="what-happens-when-throttling-occurs"></a><span data-ttu-id="46a05-107">調整が発生すると、何が起こるのでしょうか</span><span class="sxs-lookup"><span data-stu-id="46a05-107">What happens when throttling occurs?</span></span>

<span data-ttu-id="46a05-p103">調整のしきい値を超えた場合、Microsoft Graph はそのクライアントの以降の要求を一定時間制限します。調整が発生した場合、Microsoft Graph は HTTP ステータス コード 429 (Too Many Requests) を返し、要求は失敗します。失敗した要求の応答ヘッダーで、推奨される待機時間を返します。調整の動作は要求の種類と数によります。たとえば、大量の要求があれば、すべての種類の要求が調整されます。しきい値は要求の種類によって異なります。そのため、書き込みは調整を受けるが、読み込みはそのままで許容されるシナリオが起こりえます。</span><span class="sxs-lookup"><span data-stu-id="46a05-p103">When a throttling threshold is exceeded, Microsoft Graph limits any further requests from that client for a period of time. When throttling occurs, Microsoft Graph returns HTTP status code 429 (Too many requests), and the requests fail. A suggested wait time is returned in the response header of the failed request. Throttling behavior can depend on the type and number of requests. For example, if you have a high volume of requests, all requests types are throttled. Threshold limits vary based on the request type. Therefore, you could encounter a scenario where writes are throttled but reads are still permitted.</span></span> 

## <a name="common-throttling-scenarios"></a><span data-ttu-id="46a05-115">一般的な調整のシナリオ</span><span class="sxs-lookup"><span data-stu-id="46a05-115">Common throttling scenarios</span></span>

<span data-ttu-id="46a05-116">クライアントに対して調整が発生する最も一般的な原因は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="46a05-116">The most common causes of throttling of clients include:</span></span>

* <span data-ttu-id="46a05-117">あるテナントのすべてのアプリケーションから大量の要求がある。</span><span class="sxs-lookup"><span data-stu-id="46a05-117">A large number of requests across all applications in a tenant.</span></span>
* <span data-ttu-id="46a05-118">すべてのテナントで、特定のアプリケーションから大量の要求がある。</span><span class="sxs-lookup"><span data-stu-id="46a05-118">A large number of requests from a particular application across all tenants.</span></span>

## <a name="best-practices-to-handle-throttling"></a><span data-ttu-id="46a05-119">調整に対応するためのベスト プラクティス</span><span class="sxs-lookup"><span data-stu-id="46a05-119">Best practices to handle throttling</span></span>

<span data-ttu-id="46a05-120">調整に対応するためのベスト プラクティスには、次のようなものがあります。</span><span class="sxs-lookup"><span data-stu-id="46a05-120">The following are best practices for handling throttling:</span></span>

* <span data-ttu-id="46a05-121">要求あたりの操作の数を減らす。</span><span class="sxs-lookup"><span data-stu-id="46a05-121">Reduce the number of operations per request.</span></span>
* <span data-ttu-id="46a05-122">呼び出しの頻度を減らす。</span><span class="sxs-lookup"><span data-stu-id="46a05-122">Reduce the frequency of calls.</span></span>
* <span data-ttu-id="46a05-123">すべての要求が使用量の制限に計上されるため、即時の再試行を避ける。</span><span class="sxs-lookup"><span data-stu-id="46a05-123">Avoid immediate retries, because all requests accrue against your usage limits.</span></span>

<span data-ttu-id="46a05-124">エラー処理を実装する場合は、HTTP エラー コード 429 を使用して調整の発生を検出します。</span><span class="sxs-lookup"><span data-stu-id="46a05-124">When you implement error handling, use the HTTP error code 429 to detect throttling.</span></span> <span data-ttu-id="46a05-125">失敗した応答の応答ヘッダーには、*Retry-After* フィールドが含まれています。</span><span class="sxs-lookup"><span data-stu-id="46a05-125">The failed response includes the *Retry-After* field in the response header.</span></span> <span data-ttu-id="46a05-126">Microsoft Graph はクライアントが調整による制限を受けている間でもリソースの使用量を記録しています。そのため、*Retry-After* の指示に従って要求を遅延させることが最も迅速に調整を解消できる方法です。</span><span class="sxs-lookup"><span data-stu-id="46a05-126">When you implement error handling, use the HTTP error code 429 to detect throttling. The failed response includes the Retry-After field in the response header. Backing off requests using the *Retry-After* delay is the fastest way to recover from throttling because Microsoft Graph continues to log resource usage while a client is being throttled.</span></span>

1. <span data-ttu-id="46a05-127">*Retry-After* フィールドに指定された秒数だけ待機してください。</span><span class="sxs-lookup"><span data-stu-id="46a05-127">Wait the number of seconds specified in the *Retry-After* field.</span></span>
2. <span data-ttu-id="46a05-128">要求を再試行してください。</span><span class="sxs-lookup"><span data-stu-id="46a05-128">Retry the request.</span></span>
3. <span data-ttu-id="46a05-p105">要求が再度エラーコード 429 で失敗した場合は、依然として調整を受けています。Retry-After で推奨された遅延に引き続き従い、成功するまで再試行してください。</span><span class="sxs-lookup"><span data-stu-id="46a05-p105">If the request fails again with a 429 error code, you are still being throttled. Continue to use the recommended Retry-After delay and retry the request until it succeeds.</span></span>

<span data-ttu-id="46a05-131">現在、次のリソースで Retry-After ヘッダーが提供されています。</span><span class="sxs-lookup"><span data-stu-id="46a05-131">The following resources currently provide a retry-after header:</span></span>
- [<span data-ttu-id="46a05-132">ユーザー</span><span class="sxs-lookup"><span data-stu-id="46a05-132">User</span></span>](../api-reference/v1.0/resources/user.md)
- [<span data-ttu-id="46a05-133">写真</span><span class="sxs-lookup"><span data-stu-id="46a05-133">Photo</span></span>](../api-reference/v1.0/resources/profilephoto.md)
- [<span data-ttu-id="46a05-134">メール</span><span class="sxs-lookup"><span data-stu-id="46a05-134">mail</span></span>](../api-reference/v1.0/resources/message.md)
- [<span data-ttu-id="46a05-135">カレンダー (ユーザーおよびグループ)</span><span class="sxs-lookup"><span data-stu-id="46a05-135">Calendar (users and groups)</span></span>](../api-reference/v1.0/resources/event.md)
- [<span data-ttu-id="46a05-136">連絡先</span><span class="sxs-lookup"><span data-stu-id="46a05-136">Contact</span></span>](../api-reference/v1.0/resources/contact.md)
- [<span data-ttu-id="46a05-137">添付ファイル</span><span class="sxs-lookup"><span data-stu-id="46a05-137">Attachment</span></span>](../api-reference/v1.0/resources/attachment.md)
- [<span data-ttu-id="46a05-138">グループ会話</span><span class="sxs-lookup"><span data-stu-id="46a05-138">Group conversations</span></span>](../api-reference/v1.0/resources/conversation.md)
- [<span data-ttu-id="46a05-139">ユーザーとソーシャル</span><span class="sxs-lookup"><span data-stu-id="46a05-139">People and social</span></span>](../api-reference/beta/resources/social_overview.md)
- [<span data-ttu-id="46a05-140">ドライブ (OneDrive)</span><span class="sxs-lookup"><span data-stu-id="46a05-140">Drive (OneDrive)</span></span>](../api-reference/v1.0/resources/drive.md)

<span data-ttu-id="46a05-141">Microsoft Cloud における調整についてのより幅広い議論については「[調整パターン]((https://msdn.microsoft.com/ja-JP/library/office/dn589798.aspx))」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="46a05-141">For a broader discussion of throttling on the Microsoft Cloud, see [Throttling Pattern]((https://msdn.microsoft.com/ja-JP/library/office/dn589798.aspx)).</span></span>
