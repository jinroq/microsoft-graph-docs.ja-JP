---
title: Microsoft Graph 調整ガイド
description: 調整とは、リソースの使いすぎを防ぐために、サービスの同時呼び出し数を制限することをいいます。Microsoft Graph は、大量の要求を処理できるよう設計されています。過剰な数の要求が発生した場合、調整を行うことは Microsoft Graph サービスの最適なパフォーマンスと信頼性の維持に役立ちます。
ms.openlocfilehash: dfe7fed3efc01932137df00d6d62ad069faf64cd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092416"
---
# <a name="microsoft-graph-throttling-guidance"></a><span data-ttu-id="bef87-105">Microsoft Graph 調整ガイド</span><span class="sxs-lookup"><span data-stu-id="bef87-105">Microsoft Graph throttling guidance</span></span>


<span data-ttu-id="bef87-p102">調整とは、リソースの使いすぎを防ぐために、サービスの同時呼び出し数を制限することをいいます。Microsoft Graph は、大量の要求を処理できるよう設計されています。過剰な数の要求が発生した場合、調整を行うことは Microsoft Graph サービスの最適なパフォーマンスと信頼性の維持に役立ちます。</span><span class="sxs-lookup"><span data-stu-id="bef87-p102">Throttling limits the number of concurrent calls to a service to prevent overuse of resources. Microsoft Graph is designed to handle a high volume of requests. If an overwhelming number of requests occurs, throttling helps maintain optimal performance and reliability of the Microsoft Graph service.</span></span>

<span data-ttu-id="bef87-p103">制限の調整はシナリオによって異なります。たとえば、大量の書き込みを行う際には、読み込みのみを行う場合に比べて調整が起こる可能性は高くなります。</span><span class="sxs-lookup"><span data-stu-id="bef87-p103">Throttling limits vary based on the scenario. For example, if you are performing a large volume of writes, the possibility for throttling is higher than if you are only performing reads.</span></span>

## <a name="what-happens-when-throttling-occurs"></a><span data-ttu-id="bef87-111">調整が発生すると、何が起こるのでしょうか</span><span class="sxs-lookup"><span data-stu-id="bef87-111">What happens when throttling occurs?</span></span>

<span data-ttu-id="bef87-p104">調整のしきい値を超えた場合、Microsoft Graph はそのクライアントの以降の要求を一定時間制限します。調整が発生した場合、Microsoft Graph は HTTP ステータス コード 429 (Too Many Requests) を返し、要求は失敗します。失敗した要求の応答ヘッダーで、推奨される待機時間を返します。調整の動作は要求の種類と数によります。たとえば、大量の要求があれば、すべての種類の要求が調整されます。しきい値は要求の種類によって異なります。そのため、書き込みは調整を受けるが、読み込みはそのままで許容されるシナリオが起こりえます。</span><span class="sxs-lookup"><span data-stu-id="bef87-p104">When a throttling threshold is exceeded, Microsoft Graph limits any further requests from that client for a period of time. When throttling occurs, Microsoft Graph returns HTTP status code 429 (Too many requests), and the requests fail. A suggested wait time is returned in the response header of the failed request. Throttling behavior can depend on the type and number of requests. For example, if you have a high volume of requests, all requests types are throttled. Threshold limits vary based on the request type. Therefore, you could encounter a scenario where writes are throttled but reads are still permitted.</span></span> 

## <a name="common-throttling-scenarios"></a><span data-ttu-id="bef87-119">一般的な調整のシナリオ</span><span class="sxs-lookup"><span data-stu-id="bef87-119">Common throttling scenarios</span></span>

<span data-ttu-id="bef87-120">クライアントに対して調整が発生する最も一般的な原因は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="bef87-120">The most common causes of throttling of clients include:</span></span>

* <span data-ttu-id="bef87-121">あるテナントのすべてのアプリケーションから大量の要求がある。</span><span class="sxs-lookup"><span data-stu-id="bef87-121">A large number of requests across all applications in a tenant.</span></span>
* <span data-ttu-id="bef87-122">すべてのテナントで、特定のアプリケーションから大量の要求がある。</span><span class="sxs-lookup"><span data-stu-id="bef87-122">A large number of requests from a particular application across all tenants.</span></span>

## <a name="best-practices-to-handle-throttling"></a><span data-ttu-id="bef87-123">調整に対応するためのベスト プラクティス</span><span class="sxs-lookup"><span data-stu-id="bef87-123">Best practices to handle throttling</span></span>

<span data-ttu-id="bef87-124">調整に対応するためのベスト プラクティスには、次のようなものがあります。</span><span class="sxs-lookup"><span data-stu-id="bef87-124">The following are best practices for handling throttling:</span></span>

* <span data-ttu-id="bef87-125">要求あたりの操作の数を減らす。</span><span class="sxs-lookup"><span data-stu-id="bef87-125">Reduce the number of operations per request.</span></span>
* <span data-ttu-id="bef87-126">呼び出しの頻度を減らす。</span><span class="sxs-lookup"><span data-stu-id="bef87-126">Reduce the frequency of calls.</span></span>
* <span data-ttu-id="bef87-127">すべての要求が使用量の制限に計上されるため、即時の再試行を避ける。</span><span class="sxs-lookup"><span data-stu-id="bef87-127">Avoid immediate retries, because all requests accrue against your usage limits.</span></span>

<span data-ttu-id="bef87-p105">エラー処理を実装する場合は、HTTP エラー コード 429 を使用して調整の発生を検出します。失敗した要求への応答ヘッダーには、*Retry-After* フィールドが含まれています。Microsoft Graph はクライアントが調整による制限を受けている間でもリソースの使用量を記録しています。そのため、*Retry-After* の指示に従って要求を遅延させることが最も迅速に調整を解消できる方法です。</span><span class="sxs-lookup"><span data-stu-id="bef87-p105">When you implement error handling, use the HTTP error code 429 to detect throttling. The failed response includes the *Retry-After* field in the response header. Backing off requests using the *Retry-After* delay is the fastest way to recover from throttling because Microsoft Graph continues to log resource usage while a client is being throttled.</span></span>

1. <span data-ttu-id="bef87-131">*Retry-After* フィールドに指定された秒数だけ待機してください。</span><span class="sxs-lookup"><span data-stu-id="bef87-131">Wait the number of seconds specified in the *Retry-After* field.</span></span>
2. <span data-ttu-id="bef87-132">要求を再試行してください。</span><span class="sxs-lookup"><span data-stu-id="bef87-132">Retry the request.</span></span>
3. <span data-ttu-id="bef87-p106">要求が再度エラーコード 429 で失敗した場合は、依然として調整を受けています。Retry-After で推奨された遅延に引き続き従い、成功するまで再試行してください。</span><span class="sxs-lookup"><span data-stu-id="bef87-p106">If the request fails again with a 429 error code, you are still being throttled. Continue to use the recommended Retry-After delay and retry the request until it succeeds.</span></span>

<span data-ttu-id="bef87-135">現在、次のリソースで Retry-After ヘッダーが提供されています。</span><span class="sxs-lookup"><span data-stu-id="bef87-135">The following resources currently provide a retry-after header:</span></span>
- [<span data-ttu-id="bef87-136">ユーザー</span><span class="sxs-lookup"><span data-stu-id="bef87-136">User</span></span>](/graph/api/resources/user?view=graph-rest-1.0)
- [<span data-ttu-id="bef87-137">写真</span><span class="sxs-lookup"><span data-stu-id="bef87-137">Photo</span></span>](/graph/api/resources/profilephoto?view=graph-rest-1.0)
- [<span data-ttu-id="bef87-138">メール</span><span class="sxs-lookup"><span data-stu-id="bef87-138">Mail</span></span>](/graph/api/resources/message?view=graph-rest-1.0)
- [<span data-ttu-id="bef87-139">カレンダー (ユーザーおよびグループ)</span><span class="sxs-lookup"><span data-stu-id="bef87-139">Calendar (users and groups)</span></span>](/graph/api/resources/event?view=graph-rest-1.0)
- [<span data-ttu-id="bef87-140">連絡先</span><span class="sxs-lookup"><span data-stu-id="bef87-140">Contact</span></span>](/graph/api/resources/contact?view=graph-rest-1.0)
- [<span data-ttu-id="bef87-141">添付ファイル</span><span class="sxs-lookup"><span data-stu-id="bef87-141">Attachment</span></span>](/graph/api/resources/attachment?view=graph-rest-1.0)
- [<span data-ttu-id="bef87-142">グループ会話</span><span class="sxs-lookup"><span data-stu-id="bef87-142">Group conversations</span></span>](/graph/api/resources/conversation?view=graph-rest-1.0)
- [<span data-ttu-id="bef87-143">ユーザーとソーシャル</span><span class="sxs-lookup"><span data-stu-id="bef87-143">People and social</span></span>](/graph/api/resources/social-overview?view=graph-rest-beta)
- [<span data-ttu-id="bef87-144">ドライブ (OneDrive)</span><span class="sxs-lookup"><span data-stu-id="bef87-144">Drive (OneDrive)</span></span>](/graph/api/resources/drive?view=graph-rest-1.0)

<span data-ttu-id="bef87-145">Microsoft Cloud における調整についてのより幅広い議論については「[調整パターン](https://msdn.microsoft.com/library/office/dn589798.aspx)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bef87-145">For a broader discussion of throttling on the Microsoft Cloud, see [Throttling Pattern](https://msdn.microsoft.com/library/office/dn589798.aspx).</span></span>
