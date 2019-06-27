---
title: tiIndicator を更新する
description: TiIndicator オブジェクトのプロパティを更新します。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 7948197515c5749f0e0691f81b8336699e32ae75
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35270659"
---
# <a name="update-tiindicator"></a><span data-ttu-id="9ec35-103">tiIndicator を更新する</span><span class="sxs-lookup"><span data-stu-id="9ec35-103">Update tiIndicator</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ec35-104">[Tiindicator](../resources/tiindicator.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="9ec35-104">Update the properties of a [tiIndicator](../resources/tiindicator.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9ec35-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9ec35-105">Permissions</span></span>

<span data-ttu-id="9ec35-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9ec35-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9ec35-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9ec35-108">Permission type</span></span>                        | <span data-ttu-id="9ec35-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9ec35-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9ec35-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9ec35-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="9ec35-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="9ec35-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="9ec35-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9ec35-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ec35-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9ec35-113">Not supported.</span></span> |
| <span data-ttu-id="9ec35-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9ec35-114">Application</span></span>                            | <span data-ttu-id="9ec35-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="9ec35-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="9ec35-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9ec35-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/tiIndicators/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9ec35-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9ec35-117">Request headers</span></span>

| <span data-ttu-id="9ec35-118">名前</span><span class="sxs-lookup"><span data-stu-id="9ec35-118">Name</span></span>       | <span data-ttu-id="9ec35-119">説明</span><span class="sxs-lookup"><span data-stu-id="9ec35-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="9ec35-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ec35-120">Authorization</span></span> | <span data-ttu-id="9ec35-121">ベアラー {コード} が**必要です**</span><span class="sxs-lookup"><span data-stu-id="9ec35-121">Bearer {code} **Required**</span></span> |
|<span data-ttu-id="9ec35-122">Prefer</span><span class="sxs-lookup"><span data-stu-id="9ec35-122">Prefer</span></span> | <span data-ttu-id="9ec35-123">戻り値 = 表現</span><span class="sxs-lookup"><span data-stu-id="9ec35-123">return=representation</span></span> |

## <a name="request-body"></a><span data-ttu-id="9ec35-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="9ec35-124">Request body</span></span>

<span data-ttu-id="9ec35-125">要求本文で、更新する関連フィールドの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="9ec35-125">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="9ec35-126">要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。</span><span class="sxs-lookup"><span data-stu-id="9ec35-126">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="9ec35-127">最適なパフォーマンスを得るために、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="9ec35-127">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9ec35-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9ec35-128">Property</span></span>     | <span data-ttu-id="9ec35-129">型</span><span class="sxs-lookup"><span data-stu-id="9ec35-129">Type</span></span>        | <span data-ttu-id="9ec35-130">説明</span><span class="sxs-lookup"><span data-stu-id="9ec35-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9ec35-131">action</span><span class="sxs-lookup"><span data-stu-id="9ec35-131">action</span></span>|<span data-ttu-id="9ec35-132">string</span><span class="sxs-lookup"><span data-stu-id="9ec35-132">string</span></span>| <span data-ttu-id="9ec35-133">インジケーターが targetProduct セキュリティツール内から一致した場合に適用するアクション。</span><span class="sxs-lookup"><span data-stu-id="9ec35-133">The action to apply if the indicator is matched from within the targetProduct security tool.</span></span> <span data-ttu-id="9ec35-134">使用可能な値は、`unknown`、`allow`、`block`、`alert` です。</span><span class="sxs-lookup"><span data-stu-id="9ec35-134">Possible values are: `unknown`, `allow`, `block`, `alert`.</span></span>|
|<span data-ttu-id="9ec35-135">activityGroupNames</span><span class="sxs-lookup"><span data-stu-id="9ec35-135">activityGroupNames</span></span>|<span data-ttu-id="9ec35-136">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="9ec35-136">String collection</span></span>|<span data-ttu-id="9ec35-137">脅威指標でカバーされる悪意のあるアクティビティを担当する、その当事者のためのサイバー脅威インテリジェンス名。</span><span class="sxs-lookup"><span data-stu-id="9ec35-137">The cyber threat intelligence name(s) for the parties responsible for the malicious activity covered by the threat indicator.</span></span>|
|<span data-ttu-id="9ec35-138">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="9ec35-138">additionalInformation</span></span>|<span data-ttu-id="9ec35-139">String</span><span class="sxs-lookup"><span data-stu-id="9ec35-139">String</span></span>|<span data-ttu-id="9ec35-140">他の tiIndicator プロパティでカバーされていない特別なデータが配置される可能性がある catchall 領域。</span><span class="sxs-lookup"><span data-stu-id="9ec35-140">A catchall area into which extra data from the indicator not covered by the other tiIndicator properties may be placed.</span></span> <span data-ttu-id="9ec35-141">通常、additionalInformation に配置されるデータは、targetProduct セキュリティツールでは使用されません。</span><span class="sxs-lookup"><span data-stu-id="9ec35-141">Data placed into additionalInformation will typically not be utilized by the targetProduct security tool.</span></span>|
|<span data-ttu-id="9ec35-142">confidence</span><span class="sxs-lookup"><span data-stu-id="9ec35-142">confidence</span></span>|<span data-ttu-id="9ec35-143">Int32</span><span class="sxs-lookup"><span data-stu-id="9ec35-143">Int32</span></span>|<span data-ttu-id="9ec35-144">インジケーター内のデータが悪意のある動作を正確に特定していることを表す整数。</span><span class="sxs-lookup"><span data-stu-id="9ec35-144">An integer representing the confidence the data within the indicator accurately identifies malicious behavior.</span></span> <span data-ttu-id="9ec35-145">指定できる値は 0 ~ 100 で、100は最高です。</span><span class="sxs-lookup"><span data-stu-id="9ec35-145">Acceptable values are 0 – 100 with 100 being the highest.</span></span>|
|<span data-ttu-id="9ec35-146">description</span><span class="sxs-lookup"><span data-stu-id="9ec35-146">description</span></span>|<span data-ttu-id="9ec35-147">String</span><span class="sxs-lookup"><span data-stu-id="9ec35-147">String</span></span>|<span data-ttu-id="9ec35-148">インジケーターで表される脅威の簡単な説明 (100 文字以内)。</span><span class="sxs-lookup"><span data-stu-id="9ec35-148">Brief description (100 characters or less) of the threat represented by the indicator.</span></span>|
|<span data-ttu-id="9ec35-149">diamondModel</span><span class="sxs-lookup"><span data-stu-id="9ec35-149">diamondModel</span></span>|[<span data-ttu-id="9ec35-150">diamondModel</span><span class="sxs-lookup"><span data-stu-id="9ec35-150">diamondModel</span></span>](#diamondmodel-values)|<span data-ttu-id="9ec35-151">このインジケーターが存在する菱形モデルの領域。</span><span class="sxs-lookup"><span data-stu-id="9ec35-151">The area of the Diamond Model in which this indicator exists.</span></span> <span data-ttu-id="9ec35-152">可能な値は、`unknown`、`adversary`、`capability`、`infrastructure`、`victim` です。</span><span class="sxs-lookup"><span data-stu-id="9ec35-152">Possible values are: `unknown`, `adversary`, `capability`, `infrastructure`, `victim`.</span></span>|
|<span data-ttu-id="9ec35-153">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="9ec35-153">expirationDateTime</span></span>|<span data-ttu-id="9ec35-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ec35-154">DateTimeOffset</span></span>| <span data-ttu-id="9ec35-155">インジケーターがいつ期限切れになるかを示す DateTime 文字列。</span><span class="sxs-lookup"><span data-stu-id="9ec35-155">DateTime string indicating when the Indicator expires.</span></span> <span data-ttu-id="9ec35-156">システム内の古いインジケーターが保持されないようにするには、すべてのインジケーターに有効期限が設定されている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9ec35-156">All indicators must have an expiration date to avoid stale indicators persisting in the system.</span></span> <span data-ttu-id="9ec35-157">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="9ec35-157">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9ec35-158">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="9ec35-158">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="9ec35-159">externalId</span><span class="sxs-lookup"><span data-stu-id="9ec35-159">externalId</span></span>|<span data-ttu-id="9ec35-160">String</span><span class="sxs-lookup"><span data-stu-id="9ec35-160">String</span></span>|<span data-ttu-id="9ec35-161">インジケーターをインジケータープロバイダーのシステム (例: 外部キー) に結びつける識別番号。</span><span class="sxs-lookup"><span data-stu-id="9ec35-161">An identification number that ties the indicator back to the indicator provider’s system (e.g. a foreign key).</span></span>|
|<span data-ttu-id="9ec35-162">isActive</span><span class="sxs-lookup"><span data-stu-id="9ec35-162">isActive</span></span>|<span data-ttu-id="9ec35-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ec35-163">Boolean</span></span>|<span data-ttu-id="9ec35-164">システム内のインジケーターを非アクティブ化するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="9ec35-164">Used to deactivate indicators within system.</span></span> <span data-ttu-id="9ec35-165">既定では、送信されたインジケーターはすべてアクティブとして設定されます。</span><span class="sxs-lookup"><span data-stu-id="9ec35-165">By default, any indicator submitted is set as active.</span></span> <span data-ttu-id="9ec35-166">ただし、プロバイダーは、この設定を使用した既存のインジケーターを ' False ' に送信して、システム内のインジケーターを非アクティブ化することができます。</span><span class="sxs-lookup"><span data-stu-id="9ec35-166">However, providers may submit existing indicators with this set to ‘False’ to deactivate indicators in the system.</span></span>|
|<span data-ttu-id="9ec35-167">"出てきたチェイン"</span><span class="sxs-lookup"><span data-stu-id="9ec35-167">killChain</span></span>|<span data-ttu-id="9ec35-168">[](#killchain-values)指定したコレクション</span><span class="sxs-lookup"><span data-stu-id="9ec35-168">[killChain](#killchain-values) collection</span></span>|<span data-ttu-id="9ec35-169">このインジケーターが対象とする、キルチェーン上の点または点を表す文字列の JSON 配列。</span><span class="sxs-lookup"><span data-stu-id="9ec35-169">A JSON array of strings that describes which point or points on the Kill Chain this indicator targets.</span></span> <span data-ttu-id="9ec35-170">正確な値については、以下の「"" を参照」の値」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9ec35-170">See "killChain values" below for exact values.</span></span>|
|<span data-ttu-id="9ec35-171">Knownfalse 陽性</span><span class="sxs-lookup"><span data-stu-id="9ec35-171">knownFalsePositives</span></span>|<span data-ttu-id="9ec35-172">String</span><span class="sxs-lookup"><span data-stu-id="9ec35-172">String</span></span>|<span data-ttu-id="9ec35-173">インジケーターが誤検知を引き起こす可能性があるシナリオ。</span><span class="sxs-lookup"><span data-stu-id="9ec35-173">Scenarios in which the indicator may cause false positives.</span></span> <span data-ttu-id="9ec35-174">これは、人間が判読できるテキストである必要があります。</span><span class="sxs-lookup"><span data-stu-id="9ec35-174">This should be human-readable text.</span></span>|
|<span data-ttu-id="9ec35-175">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="9ec35-175">lastReportedDateTime</span></span>|<span data-ttu-id="9ec35-176">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ec35-176">DateTimeOffset</span></span>|<span data-ttu-id="9ec35-177">最後にインジケーターが表示された時刻。</span><span class="sxs-lookup"><span data-stu-id="9ec35-177">The last time the indicator was seen.</span></span> <span data-ttu-id="9ec35-178">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="9ec35-178">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9ec35-179">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="9ec35-179">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="9ec35-180">悪意のある Refrefamilynames</span><span class="sxs-lookup"><span data-stu-id="9ec35-180">malwareFamilyNames</span></span>|<span data-ttu-id="9ec35-181">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="9ec35-181">String collection</span></span>|<span data-ttu-id="9ec35-182">インジケーターに関連付けられたマルウェアファミリ名 (存在する場合)。</span><span class="sxs-lookup"><span data-stu-id="9ec35-182">The malware family name associated with an indicator if it exists.</span></span> <span data-ttu-id="9ec35-183">Microsoft では、Windows Defender セキュリティインテリジェンスの[脅威の百科事典](https://www.microsoft.com/wdsi/threats)を使用して検出できる場合は、microsoft マルウェアファミリ名を推奨しています。</span><span class="sxs-lookup"><span data-stu-id="9ec35-183">Microsoft prefers the Microsoft malware family name if at all possible which can be found via the Windows Defender Security Intelligence [threat encyclopedia](https://www.microsoft.com/wdsi/threats).</span></span>|
|<span data-ttu-id="9ec35-184">「いいえ Veonly」</span><span class="sxs-lookup"><span data-stu-id="9ec35-184">passiveOnly</span></span>|<span data-ttu-id="9ec35-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ec35-185">Boolean</span></span>|<span data-ttu-id="9ec35-186">エンドユーザーに表示されるイベントをインジケーターがトリガーするかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="9ec35-186">Determines if the indicator should trigger an event that is visible to an end-user.</span></span> <span data-ttu-id="9ec35-187">[True] に設定されている場合、セキュリティツールは、' hit ' が発生したことをエンドユーザーに通知しません。</span><span class="sxs-lookup"><span data-stu-id="9ec35-187">When set to ‘true,’ security tools will not notify the end user that a ‘hit’ has occurred.</span></span> <span data-ttu-id="9ec35-188">これは、通常、一致が発生したが、その操作は実行されないことをログに記録するセキュリティ製品によって、監査またはサイレントモードとして扱われます。</span><span class="sxs-lookup"><span data-stu-id="9ec35-188">This is most often treated as audit or silent mode by security products where they will simply log that a match occurred but will not perform the action.</span></span> <span data-ttu-id="9ec35-189">既定値は False です。</span><span class="sxs-lookup"><span data-stu-id="9ec35-189">Default value is false.</span></span>|
|<span data-ttu-id="9ec35-190">severity</span><span class="sxs-lookup"><span data-stu-id="9ec35-190">severity</span></span>|<span data-ttu-id="9ec35-191">Int32</span><span class="sxs-lookup"><span data-stu-id="9ec35-191">Int32</span></span>|<span data-ttu-id="9ec35-192">インジケーター内のデータによって識別される、悪意のある動作の重要度を表す整数。</span><span class="sxs-lookup"><span data-stu-id="9ec35-192">An integer representing the severity of the malicious behavior identified by the data within the indicator.</span></span> <span data-ttu-id="9ec35-193">指定可能な値は0–5で、5は最も深刻であり、0はまったく重要ではありません。</span><span class="sxs-lookup"><span data-stu-id="9ec35-193">Acceptable values are 0 – 5 where 5 is the most severe and zero is not severe at all.</span></span> <span data-ttu-id="9ec35-194">既定値は3です。</span><span class="sxs-lookup"><span data-stu-id="9ec35-194">Default value is 3.</span></span>|
|<span data-ttu-id="9ec35-195">タグ</span><span class="sxs-lookup"><span data-stu-id="9ec35-195">tags</span></span>|<span data-ttu-id="9ec35-196">String collection</span><span class="sxs-lookup"><span data-stu-id="9ec35-196">String collection</span></span>|<span data-ttu-id="9ec35-197">任意のタグ/キーワードを格納する文字列の JSON 配列。</span><span class="sxs-lookup"><span data-stu-id="9ec35-197">A JSON array of strings that stores arbitrary tags/keywords.</span></span>|
|<span data-ttu-id="9ec35-198">tlpLevel</span><span class="sxs-lookup"><span data-stu-id="9ec35-198">tlpLevel</span></span>|[<span data-ttu-id="9ec35-199">tlpLevel</span><span class="sxs-lookup"><span data-stu-id="9ec35-199">tlpLevel</span></span>](#tlplevel-values)| <span data-ttu-id="9ec35-200">インジケーターのトラフィックライトプロトコルの値。</span><span class="sxs-lookup"><span data-stu-id="9ec35-200">Traffic Light Protocol value for the indicator.</span></span> <span data-ttu-id="9ec35-201">可能な値は、`unknown`、`white`、`green`、`amber`、`red` です。</span><span class="sxs-lookup"><span data-stu-id="9ec35-201">Possible values are: `unknown`, `white`, `green`, `amber`, `red`.</span></span>|

### <a name="diamondmodel-values"></a><span data-ttu-id="9ec35-202">diamondModel の値</span><span class="sxs-lookup"><span data-stu-id="9ec35-202">diamondModel values</span></span>

<span data-ttu-id="9ec35-203">このモデルの詳細については、[ダイヤモンドモデル](http://diamondmodel.org)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9ec35-203">For information about this model, see [The diamond model](http://diamondmodel.org).</span></span>

| <span data-ttu-id="9ec35-204">値</span><span class="sxs-lookup"><span data-stu-id="9ec35-204">Values</span></span> | <span data-ttu-id="9ec35-205">説明</span><span class="sxs-lookup"><span data-stu-id="9ec35-205">Description</span></span> |
|:-------|:------------|
|<span data-ttu-id="9ec35-206">攻撃</span><span class="sxs-lookup"><span data-stu-id="9ec35-206">adversary</span></span>|<span data-ttu-id="9ec35-207">このマークは、敵対について説明します。</span><span class="sxs-lookup"><span data-stu-id="9ec35-207">The indicator describes the adversary.</span></span>|
|<span data-ttu-id="9ec35-208">capability</span><span class="sxs-lookup"><span data-stu-id="9ec35-208">capability</span></span>|<span data-ttu-id="9ec35-209">マークは敵対機の機能です。</span><span class="sxs-lookup"><span data-stu-id="9ec35-209">The indicator is a capability of the adversary.</span></span>|
|<span data-ttu-id="9ec35-210">構築</span><span class="sxs-lookup"><span data-stu-id="9ec35-210">infrastructure</span></span>|<span data-ttu-id="9ec35-211">このインジケーターは、敵対のインフラストラクチャを示しています。</span><span class="sxs-lookup"><span data-stu-id="9ec35-211">The indicator describes infrastructure of the adversary.</span></span>|
|<span data-ttu-id="9ec35-212">犠牲</span><span class="sxs-lookup"><span data-stu-id="9ec35-212">victim</span></span>|<span data-ttu-id="9ec35-213">インジケーターは、敵対者の被害者を示します。</span><span class="sxs-lookup"><span data-stu-id="9ec35-213">The indicator describes the victim of the adversary.</span></span>|

### <a name="killchain-values"></a><span data-ttu-id="9ec35-214">指定した値の継承</span><span class="sxs-lookup"><span data-stu-id="9ec35-214">killChain values</span></span>

| <span data-ttu-id="9ec35-215">値</span><span class="sxs-lookup"><span data-stu-id="9ec35-215">Values</span></span> | <span data-ttu-id="9ec35-216">説明</span><span class="sxs-lookup"><span data-stu-id="9ec35-216">Description</span></span> |
|:-------|:------------|
|<span data-ttu-id="9ec35-217">アクション</span><span class="sxs-lookup"><span data-stu-id="9ec35-217">Actions</span></span>|<span data-ttu-id="9ec35-218">"目的に対するアクション" を表します。</span><span class="sxs-lookup"><span data-stu-id="9ec35-218">Represents “Actions on Objectives”.</span></span> <span data-ttu-id="9ec35-219">攻撃者が侵害されたシステムを活用して、分散型サービス拒否攻撃などの処理を実行している。</span><span class="sxs-lookup"><span data-stu-id="9ec35-219">The attacker is leveraging the compromised system to take actions such as a distributed denial of service attack.</span></span>|
|<span data-ttu-id="9ec35-220">基準</span><span class="sxs-lookup"><span data-stu-id="9ec35-220">C2</span></span>|<span data-ttu-id="9ec35-221">侵害されたシステムの操作によって制御されるチャネルを表します。</span><span class="sxs-lookup"><span data-stu-id="9ec35-221">Represents the control channel by which a compromised system is manipulated.</span></span>|
|<span data-ttu-id="9ec35-222">Delivery</span><span class="sxs-lookup"><span data-stu-id="9ec35-222">Delivery</span></span>|<span data-ttu-id="9ec35-223">悪用コードを (例: USB、電子メール、web サイトなどの) 被害に分配するプロセス。</span><span class="sxs-lookup"><span data-stu-id="9ec35-223">The process of distributing the exploit code to victims (for example USB, email, websites).</span></span>|
|<span data-ttu-id="9ec35-224">活用</span><span class="sxs-lookup"><span data-stu-id="9ec35-224">Exploitation</span></span>|<span data-ttu-id="9ec35-225">脆弱性を利用するエクスプロイトコード (例: コードの実行)。</span><span class="sxs-lookup"><span data-stu-id="9ec35-225">The exploit code taking advantage of vulnerabilities (for example, code execution).</span></span>|
|<span data-ttu-id="9ec35-226">インストール</span><span class="sxs-lookup"><span data-stu-id="9ec35-226">Installation</span></span>|<span data-ttu-id="9ec35-227">脆弱性が悪用された後にマルウェアをインストールする。</span><span class="sxs-lookup"><span data-stu-id="9ec35-227">Installing malware after a vulnerability has been exploited.</span></span>|
|<span data-ttu-id="9ec35-228">予備</span><span class="sxs-lookup"><span data-stu-id="9ec35-228">Reconnaissance</span></span>|<span data-ttu-id="9ec35-229">マークは、今後の攻撃で使用されるアクティビティグループの情報の証拠です。</span><span class="sxs-lookup"><span data-stu-id="9ec35-229">Indicator is evidence of an activity group harvesting information to be used in a future attack.</span></span>|
|<span data-ttu-id="9ec35-230">Weaponization</span><span class="sxs-lookup"><span data-stu-id="9ec35-230">Weaponization</span></span>|<span data-ttu-id="9ec35-231">脆弱性を悪用コードに変える (たとえば、マルウェア)。</span><span class="sxs-lookup"><span data-stu-id="9ec35-231">Turning a vulnerability into exploit code (for example, malware).</span></span>|

### <a name="tlplevel-values"></a><span data-ttu-id="9ec35-232">tlpLevel の値</span><span class="sxs-lookup"><span data-stu-id="9ec35-232">tlpLevel values</span></span>

<span data-ttu-id="9ec35-233">各インジケーターには、送信時にトラフィックライトプロトコル (tlp) 値が必要です。</span><span class="sxs-lookup"><span data-stu-id="9ec35-233">Every indicator must have a Traffic Light Protocol (tlp) value when it is submitted.</span></span> <span data-ttu-id="9ec35-234">この値は、特定のインジケーターの感度と共有の範囲を表します。</span><span class="sxs-lookup"><span data-stu-id="9ec35-234">This value represents the sensitivity and sharing scope of a given indicator.</span></span>

| <span data-ttu-id="9ec35-235">値</span><span class="sxs-lookup"><span data-stu-id="9ec35-235">Values</span></span> | <span data-ttu-id="9ec35-236">説明</span><span class="sxs-lookup"><span data-stu-id="9ec35-236">Description</span></span> |
|:-------|:------------|
|<span data-ttu-id="9ec35-237">ホワイト</span><span class="sxs-lookup"><span data-stu-id="9ec35-237">White</span></span>| <span data-ttu-id="9ec35-238">共有スコープ: 無制限。</span><span class="sxs-lookup"><span data-stu-id="9ec35-238">Sharing scope: Unlimited.</span></span> <span data-ttu-id="9ec35-239">インジケーターは無制限に共有できます。制限はありません。</span><span class="sxs-lookup"><span data-stu-id="9ec35-239">Indicators can be shared freely, without restriction.</span></span>|
|<span data-ttu-id="9ec35-240">緑</span><span class="sxs-lookup"><span data-stu-id="9ec35-240">Green</span></span>| <span data-ttu-id="9ec35-241">共有スコープ: コミュニティ。</span><span class="sxs-lookup"><span data-stu-id="9ec35-241">Sharing scope: Community.</span></span> <span data-ttu-id="9ec35-242">インジケーターはセキュリティコミュニティと共有できます。</span><span class="sxs-lookup"><span data-stu-id="9ec35-242">Indicators can be shared with the security community.</span></span>|
|<span data-ttu-id="9ec35-243">黄色い</span><span class="sxs-lookup"><span data-stu-id="9ec35-243">Amber</span></span>| <span data-ttu-id="9ec35-244">共有スコープ: 制限されています。</span><span class="sxs-lookup"><span data-stu-id="9ec35-244">Sharing scope: Limited.</span></span> <span data-ttu-id="9ec35-245">これは、インジケーターの既定の設定であり、共有を脅威インテリジェンスを実装するサービスとサービスオペレーターだけに限定し、共有を制限します。2) システムの動作がインジケーターと同じであるお客様。</span><span class="sxs-lookup"><span data-stu-id="9ec35-245">This is the default setting for indicators and restricts sharing to only those with a need-to-know: 1) Services and service operators that implement threat intelligence; 2) Customers whose system(s) exhibit behavior consistent with the indicator.</span></span>|
|<span data-ttu-id="9ec35-246">赤</span><span class="sxs-lookup"><span data-stu-id="9ec35-246">Red</span></span>| <span data-ttu-id="9ec35-247">共有スコープ: Personal。</span><span class="sxs-lookup"><span data-stu-id="9ec35-247">Sharing scope: Personal.</span></span> <span data-ttu-id="9ec35-248">これらのインジケーターは、本人でのみ直接共有されるようになっています。</span><span class="sxs-lookup"><span data-stu-id="9ec35-248">These indicators are to only be shared directly and, preferably, in person.</span></span> <span data-ttu-id="9ec35-249">通常は、指定された制限によって TLP 赤のインジケーターは取り込まれたされません。</span><span class="sxs-lookup"><span data-stu-id="9ec35-249">Typically, TLP Red indicators are not ingested due to their pre-defined restrictions.</span></span> <span data-ttu-id="9ec35-250">TLP 赤のインジケーターが送信され\*\*\*\* た場合は、"いいえ" の`True`プロパティをに設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="9ec35-250">If TLP Red indicators are submitted, the **passiveOnly** property should be set to `True` as well.</span></span> |

## <a name="response"></a><span data-ttu-id="9ec35-251">応答</span><span class="sxs-lookup"><span data-stu-id="9ec35-251">Response</span></span>

<span data-ttu-id="9ec35-252">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="9ec35-252">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="9ec35-253">省略可能な`200 OK`要求ヘッダーが使用されている場合、メソッドは応答コードと、応答本文で更新された[tiindicator](../resources/tiindicator.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9ec35-253">If the optional request header is used, the method returns a `200 OK` response code and the updated [tiIndicator](../resources/tiindicator.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9ec35-254">例</span><span class="sxs-lookup"><span data-stu-id="9ec35-254">Examples</span></span>

### <a name="example-1-request-without-prefer-header"></a><span data-ttu-id="9ec35-255">例 1: 希望するヘッダーのない要求</span><span class="sxs-lookup"><span data-stu-id="9ec35-255">Example 1: Request without Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="9ec35-256">要求</span><span class="sxs-lookup"><span data-stu-id="9ec35-256">Request</span></span>

<span data-ttu-id="9ec35-257">ヘッダーの`Prefer`ない要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9ec35-257">The following is an example of the request without the `Prefer` header.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_tiIndicator"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/tiIndicators/{id}
Content-type: application/json

{
  "description": "description-updated",
}
```

#### <a name="response"></a><span data-ttu-id="9ec35-258">応答</span><span class="sxs-lookup"><span data-stu-id="9ec35-258">Response</span></span>

<span data-ttu-id="9ec35-259">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9ec35-259">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tiIndicator"
} -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="9ec35-260">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="9ec35-260">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="9ec35-261">C#</span><span class="sxs-lookup"><span data-stu-id="9ec35-261">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_tiIndicator-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9ec35-262">Javascript</span><span class="sxs-lookup"><span data-stu-id="9ec35-262">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_tiIndicator-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="9ec35-263">目的-C</span><span class="sxs-lookup"><span data-stu-id="9ec35-263">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_tiIndicator-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="example-2-request-with-prefer-header"></a><span data-ttu-id="9ec35-264">例 2: 要求ヘッダーを使用した要求</span><span class="sxs-lookup"><span data-stu-id="9ec35-264">Example 2: Request with Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="9ec35-265">要求</span><span class="sxs-lookup"><span data-stu-id="9ec35-265">Request</span></span>

<span data-ttu-id="9ec35-266">`Prefer`ヘッダーを含む要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9ec35-266">The following is an example of the request that includes the `Prefer` header.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_tiIndicator"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/tiIndicators/{id}
Content-type: application/json
Prefer: return=representation

{
  "additionalInformation": "additionalInformation-after-update",
  "confidence": 42,
  "description": "description-after-update",
}
```

#### <a name="response"></a><span data-ttu-id="9ec35-267">応答</span><span class="sxs-lookup"><span data-stu-id="9ec35-267">Response</span></span>

<span data-ttu-id="9ec35-268">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9ec35-268">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="9ec35-269">ここに示す response オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="9ec35-269">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9ec35-270">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="9ec35-270">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tiIndicator"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Security/tiIndicators/$entity",
    "id": "e58c072b-c9bb-a5c4-34ce-eb69af44fb1e",
    "azureTenantId": "XXXXXXXXXXXXXXXXXXXXXXXXX",
    "action": null,
    "additionalInformation": "additionalInformation-after-update",
    "activityGroupNames": [],
    "confidence": 42,
    "description": "description-after-update",
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update tiIndicator",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/tiindicator-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/tiindicator-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/tiindicator-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/tiindicator-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/tiindicator-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
