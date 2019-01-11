---
title: アクティビティのリソースの種類
description: -テレビ番組、ドキュメント、ビデオ ゲームの現在のキャンペーンなど、アプリケーション内で 1 つのアクティビティを表します。 ユーザーは、その活動と連携して、ときに、そのアクティビティの開始と終了時刻を示す履歴項目として契約がキャプチャされます。 ようにユーザーには、再、時間の経過と共にその活動と連携して、1 人のユーザーの活動の複数の項目の履歴が記録されます。
localization_priority: Normal
ms.openlocfilehash: 79ed44ef0f6a38fbef8ead233debce3fc9e66b42
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27877071"
---
# <a name="activity-resource-type"></a><span data-ttu-id="43874-105">アクティビティのリソースの種類</span><span class="sxs-lookup"><span data-stu-id="43874-105">activity resource type</span></span>

<span data-ttu-id="43874-106">-テレビ番組、ドキュメント、ビデオ ゲームの現在のキャンペーンなど、アプリケーション内で 1 つのアクティビティを表します。</span><span class="sxs-lookup"><span data-stu-id="43874-106">Represents a single activity within an app - for example, a TV show, a document, or a current campaign in a video game.</span></span> <span data-ttu-id="43874-107">ユーザーは、その活動と連携して、ときに、そのアクティビティの開始と終了時刻を示します、[履歴項目](projectrome-historyitem.md)として契約がキャプチャされます。</span><span class="sxs-lookup"><span data-stu-id="43874-107">When a user engages with that activity, the engagement is captured as a [history item](projectrome-historyitem.md) that indicates the start and end time for that activity.</span></span> <span data-ttu-id="43874-108">ようにユーザーには、再、時間の経過と共にその活動と連携して、1 人のユーザーの活動の複数の項目の履歴が記録されます。</span><span class="sxs-lookup"><span data-stu-id="43874-108">As the user re-engages with that activity over time, multiple history items are recorded for a single user activity.</span></span>

<span data-ttu-id="43874-109">何のアプリケーションでは、複数のデバイスを取得するのにユーザーを有効にするのに Microsoft Graph でのアクティビティを使用できます。</span><span class="sxs-lookup"><span data-stu-id="43874-109">You can use activities in Microsoft Graph to enable users to get back to what they were doing in their app, across multiple devices.</span></span> <span data-ttu-id="43874-110">アプリを作成する活動は、すべてのユーザーのデバイスに表示され、アプリ内で特定のコンテンツへの高度なリンクとしてユーザーに公開されます。</span><span class="sxs-lookup"><span data-stu-id="43874-110">Activities that your app creates appear on all users' devices, and are exposed to users as deep links to specific content within your app.</span></span> <span data-ttu-id="43874-111">Cortana の通知によってあっにアクセスし、Windows では、紹介先として、アプリケーション内で特定のコンテンツを表現できます。</span><span class="sxs-lookup"><span data-stu-id="43874-111">You can express specific content within your app as a destination that is showcased in Windows, and accessible on iOS and Android devices through Cortana notifications.</span></span>

<span data-ttu-id="43874-112">すべてのアプリケーションが異なるためにです Cortana およびタイムラインに表示されるユーザー ・ アクティビティをアプリケーション内で操作をマップする最善の方法を理解します。</span><span class="sxs-lookup"><span data-stu-id="43874-112">Because every app is different, it's up to you to understand the best way to map actions within your application to user activities that will appear in Cortana and Timeline.</span></span> <span data-ttu-id="43874-113">などのゲームは、各キャンペーンの活動を作成可能性があります、文書作成アプリケーションはそれぞれ固有のドキュメントのアクティビティを作成可能性があり、基幹業務アプリケーションは、各ワークフローのアクティビティを作成可能性があります。</span><span class="sxs-lookup"><span data-stu-id="43874-113">For example, games might create an activity for each campaign, document authoring apps might create an activity for each unique document, and line-of-business apps might create an activity for each workflow.</span></span>

<span data-ttu-id="43874-114">Cortana およびタイムラインの Windows ユーザー エクスペリエンスは、ユーザーの生産性と効率性を増やすことにより、過去に働いているコンテンツに戻ることに重点を置くに、ユーザーの作業中です。</span><span class="sxs-lookup"><span data-stu-id="43874-114">Your user activities will be showcased in Cortana and Windows Timeline user experiences, which are focused on increasing users' productivity and efficiency by helping them get back to content they worked on in the past.</span></span>

## <a name="methods"></a><span data-ttu-id="43874-115">メソッド</span><span class="sxs-lookup"><span data-stu-id="43874-115">Methods</span></span>

|<span data-ttu-id="43874-116">メソッド</span><span class="sxs-lookup"><span data-stu-id="43874-116">Method</span></span> | <span data-ttu-id="43874-117">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="43874-117">Return Type</span></span> | <span data-ttu-id="43874-118">説明</span><span class="sxs-lookup"><span data-stu-id="43874-118">Description</span></span>|
|:------|:------------|:-----------|
|[<span data-ttu-id="43874-119">活動の作成または</span><span class="sxs-lookup"><span data-stu-id="43874-119">Create or replace activity</span></span>](../api/projectrome-put-activity.md) | [<span data-ttu-id="43874-120">アクティビティ</span><span class="sxs-lookup"><span data-stu-id="43874-120">activity</span></span>](projectrome-activity.md) |<span data-ttu-id="43874-121">作成または既存の活動 (アップサート) が置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="43874-121">Creates or replaces an existing activity (upsert).</span></span> <span data-ttu-id="43874-122">AppActivityId は URL セーフ (RFC 2396 の予約文字は、16 進表現に変換する必要がありますを除くすべての文字) である必要がありますが、元の appActivityId は、URL セーフである必要はありません。</span><span class="sxs-lookup"><span data-stu-id="43874-122">The appActivityId needs to be URL-safe (all characters except for RFC 2396 unreserved characters must be converted to their hexadecimal representation), but the original appActivityId does not have to be URL-safe.</span></span> |
|[<span data-ttu-id="43874-123">アクティビティを削除する</span><span class="sxs-lookup"><span data-stu-id="43874-123">Delete an activity</span></span>](../api/projectrome-delete-activity.md) | <span data-ttu-id="43874-124">内容なし</span><span class="sxs-lookup"><span data-stu-id="43874-124">No Content</span></span> | <span data-ttu-id="43874-125">アプリからそのユーザーの指定したアクティビティを削除します。</span><span class="sxs-lookup"><span data-stu-id="43874-125">Deletes the specified activity for that user from your app.</span></span>|
|[<span data-ttu-id="43874-126">アクティビティを取得します。</span><span class="sxs-lookup"><span data-stu-id="43874-126">Get activities</span></span>](../api/projectrome-get-activities.md) | <span data-ttu-id="43874-127">[活動](projectrome-activity.md)のコレクション</span><span class="sxs-lookup"><span data-stu-id="43874-127">Collection of [activities](projectrome-activity.md)</span></span> | <span data-ttu-id="43874-128">アプリが特定のユーザーのアクティビティを取得します。</span><span class="sxs-lookup"><span data-stu-id="43874-128">Gets the activities for your app for a given user.</span></span>|
|[<span data-ttu-id="43874-129">最近のアクティビティを取得する</span><span class="sxs-lookup"><span data-stu-id="43874-129">Get recent activities</span></span>](../api/projectrome-get-recent-activities.md) | <span data-ttu-id="43874-130">[活動](projectrome-activity.md)のコレクション</span><span class="sxs-lookup"><span data-stu-id="43874-130">Collection of [activities](projectrome-activity.md)</span></span> | <span data-ttu-id="43874-131">アプリが並べ替えられ、最も最近作成または更新された[historyItems](projectrome-historyitem.md)に基づいて、特定のユーザーの最新のアクティビティを取得します。</span><span class="sxs-lookup"><span data-stu-id="43874-131">Gets the most recent activities for your app for a given user, sorted and based on the most recently created or updated [historyItems](projectrome-historyitem.md).</span></span>|

## <a name="properties"></a><span data-ttu-id="43874-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="43874-132">Properties</span></span>

|<span data-ttu-id="43874-133">名前</span><span class="sxs-lookup"><span data-stu-id="43874-133">Name</span></span> | <span data-ttu-id="43874-134">種類</span><span class="sxs-lookup"><span data-stu-id="43874-134">Type</span></span> | <span data-ttu-id="43874-135">説明</span><span class="sxs-lookup"><span data-stu-id="43874-135">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="43874-136">userTimezone</span><span class="sxs-lookup"><span data-stu-id="43874-136">userTimezone</span></span> | <span data-ttu-id="43874-137">String</span><span class="sxs-lookup"><span data-stu-id="43874-137">String</span></span> | <span data-ttu-id="43874-138">省略可能。</span><span class="sxs-lookup"><span data-stu-id="43874-138">Optional.</span></span> <span data-ttu-id="43874-139">活動の作成時に配置されましたユーザーのデバイスのアクティビティを生成するために使用するタイム ゾーンクロスプラット フォーム形式をサポートするために、Olson の Id として指定された値です。</span><span class="sxs-lookup"><span data-stu-id="43874-139">The timezone in which the user's device used to generate the activity was located at activity creation time; values supplied as Olson IDs in order to support cross-platform representation.</span></span>|
|<span data-ttu-id="43874-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="43874-140">createdDateTime</span></span> | <span data-ttu-id="43874-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43874-141">DateTimeOffset</span></span> | <span data-ttu-id="43874-142">サーバーで設定します。</span><span class="sxs-lookup"><span data-stu-id="43874-142">Set by the server.</span></span> <span data-ttu-id="43874-143">サーバー上にオブジェクトが作成されたときの utc 日時。</span><span class="sxs-lookup"><span data-stu-id="43874-143">DateTime in UTC when the object was created on the server.</span></span> |
|<span data-ttu-id="43874-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="43874-144">lastModifiedDateTime</span></span> | <span data-ttu-id="43874-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43874-145">DateTimeOffset</span></span> | <span data-ttu-id="43874-146">サーバーで設定します。</span><span class="sxs-lookup"><span data-stu-id="43874-146">Set by the server.</span></span> <span data-ttu-id="43874-147">サーバー上にオブジェクトが変更されたときの utc 日時。</span><span class="sxs-lookup"><span data-stu-id="43874-147">DateTime in UTC when the object was modified on the server.</span></span> |
|<span data-ttu-id="43874-148">id</span><span class="sxs-lookup"><span data-stu-id="43874-148">id</span></span> | <span data-ttu-id="43874-149">String</span><span class="sxs-lookup"><span data-stu-id="43874-149">String</span></span> | <span data-ttu-id="43874-150">サーバーによって生成される ID が URL に対応するために使用します。</span><span class="sxs-lookup"><span data-stu-id="43874-150">Server-generated ID used for URL addressing.</span></span>|
|<span data-ttu-id="43874-151">appActivityId</span><span class="sxs-lookup"><span data-stu-id="43874-151">appActivityId</span></span> | <span data-ttu-id="43874-152">String</span><span class="sxs-lookup"><span data-stu-id="43874-152">String</span></span> | <span data-ttu-id="43874-153">必須。</span><span class="sxs-lookup"><span data-stu-id="43874-153">Required.</span></span> <span data-ttu-id="43874-154">呼び出し元によって、不変をその後提供された - アプリケーションのコンテキストで一意のアクティビティ ID です。</span><span class="sxs-lookup"><span data-stu-id="43874-154">The unique activity ID in the context of the app - supplied by caller and immutable thereafter.</span></span>|
|<span data-ttu-id="43874-155">activitySourceHost</span><span class="sxs-lookup"><span data-stu-id="43874-155">activitySourceHost</span></span> | <span data-ttu-id="43874-156">String</span><span class="sxs-lookup"><span data-stu-id="43874-156">String</span></span> | <span data-ttu-id="43874-157">必須。</span><span class="sxs-lookup"><span data-stu-id="43874-157">Required.</span></span> <span data-ttu-id="43874-158">アプリケーションのクロスプラット フォームの id のマッピングを表すドメインの URL です。</span><span class="sxs-lookup"><span data-stu-id="43874-158">URL for the domain representing the cross-platform identity mapping for the app.</span></span> <span data-ttu-id="43874-159">マッピングは、ドメインでホストされている JSON ファイルとして、ストアドや Windows デベロッパー センターを使用して構成できます。</span><span class="sxs-lookup"><span data-stu-id="43874-159">Mapping is stored either as a JSON file hosted on the domain or configurable via Windows Dev Center.</span></span> <span data-ttu-id="43874-160">JSON ファイルは、クロス プラットフォーム アプリケーション識別子の名前はまたはトップ レベルのドメイン レベルのいずれか、"HTTPS"ドメインのルートでホストされていますとサブのドメインが含まれます。</span><span class="sxs-lookup"><span data-stu-id="43874-160">The JSON file is named cross-platform-app-identifiers and is hosted at root of your HTTPS domain, either at the top level domain or include a sub domain.</span></span> <span data-ttu-id="43874-161">例: https://contoso.com または https://myapp.contoso.com。しかし、https://myapp.contoso.com/somepath は無効です。</span><span class="sxs-lookup"><span data-stu-id="43874-161">For example: https://contoso.com or https://myapp.contoso.com but NOT https://myapp.contoso.com/somepath.</span></span> <span data-ttu-id="43874-162">クロスプラット フォームのアプリケーション id ごと、一意のファイルおよびドメイン (またはサブドメイン) をすることが必要です。</span><span class="sxs-lookup"><span data-stu-id="43874-162">You must have a unique file and domain (or sub domain) per cross-platform app identity.</span></span> <span data-ttu-id="43874-163">たとえば、PowerPoint と Word の別のファイルとドメインが必要です。</span><span class="sxs-lookup"><span data-stu-id="43874-163">For example, a separate file and domain is needed for Word vs. PowerPoint.</span></span>|
|<span data-ttu-id="43874-164">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="43874-164">appDisplayName</span></span> | <span data-ttu-id="43874-165">String</span><span class="sxs-lookup"><span data-stu-id="43874-165">String</span></span> | <span data-ttu-id="43874-166">省略可能。</span><span class="sxs-lookup"><span data-stu-id="43874-166">Optional.</span></span> <span data-ttu-id="43874-167">アプリケーションがユーザーのローカル デバイスにインストールされていない場合の場合に使用するための活動を生成するために使用するアプリケーションの短い説明です。</span><span class="sxs-lookup"><span data-stu-id="43874-167">Short text description of the app used to generate the activity for use in cases when the app is not installed on the user’s local device.</span></span>|
|<span data-ttu-id="43874-168">activationUrl</span><span class="sxs-lookup"><span data-stu-id="43874-168">activationUrl</span></span> | <span data-ttu-id="43874-169">String</span><span class="sxs-lookup"><span data-stu-id="43874-169">String</span></span> | <span data-ttu-id="43874-170">必須。</span><span class="sxs-lookup"><span data-stu-id="43874-170">Required.</span></span> <span data-ttu-id="43874-171">AppId によって表される最適なネイティブの経験ではアクティビティを起動するために使用する URL です。</span><span class="sxs-lookup"><span data-stu-id="43874-171">URL used to launch the activity in the best native experience represented by the appId.</span></span> <span data-ttu-id="43874-172">ネイティブ アプリケーションが存在しない場合は、web ベースのアプリケーションを起動する場合があります。</span><span class="sxs-lookup"><span data-stu-id="43874-172">Might launch a web-based app if no native app exists.</span></span>|
|<span data-ttu-id="43874-173">fallbackUrl</span><span class="sxs-lookup"><span data-stu-id="43874-173">fallbackUrl</span></span> | <span data-ttu-id="43874-174">String</span><span class="sxs-lookup"><span data-stu-id="43874-174">String</span></span> | <span data-ttu-id="43874-175">省略可能。</span><span class="sxs-lookup"><span data-stu-id="43874-175">Optional.</span></span> <span data-ttu-id="43874-176">URL が利用可能な場合は、web ベースのアプリケーションでは、アクティビティの起動に使用します。</span><span class="sxs-lookup"><span data-stu-id="43874-176">URL used to launch the activity in a web-based app, if available.</span></span>|
|<span data-ttu-id="43874-177">contentUrl</span><span class="sxs-lookup"><span data-stu-id="43874-177">contentUrl</span></span> | <span data-ttu-id="43874-178">String</span><span class="sxs-lookup"><span data-stu-id="43874-178">String</span></span> | <span data-ttu-id="43874-179">省略可能。</span><span class="sxs-lookup"><span data-stu-id="43874-179">Optional.</span></span> <span data-ttu-id="43874-180">ネイティブまたは web ベースのアプリケーションの操作 (たとえば、RSS フィード内のアイテムへのポインター) の外部コンテンツを表示できる場合に使用されます。</span><span class="sxs-lookup"><span data-stu-id="43874-180">Used in the event the content can be rendered outside of a native or web-based app experience (for example, a pointer to an item in an RSS feed).</span></span>|
|<span data-ttu-id="43874-181">visualElements</span><span class="sxs-lookup"><span data-stu-id="43874-181">visualElements</span></span>| [<span data-ttu-id="43874-182">visualInfo</span><span class="sxs-lookup"><span data-stu-id="43874-182">visualInfo</span></span>](../resources/projectrome-visualinfo.md) | <span data-ttu-id="43874-183">必須。</span><span class="sxs-lookup"><span data-stu-id="43874-183">Required.</span></span> <span data-ttu-id="43874-184">エクスペリエンスの利用状況を表示する情報を格納しているオブジェクト</span><span class="sxs-lookup"><span data-stu-id="43874-184">The object containing information to render the activity in the UX.</span></span>|
|<span data-ttu-id="43874-185">contentInfo</span><span class="sxs-lookup"><span data-stu-id="43874-185">contentInfo</span></span> | <span data-ttu-id="43874-186">JSON オブジェクトの型指定されていません。</span><span class="sxs-lookup"><span data-stu-id="43874-186">Untyped JSON object</span></span> | <span data-ttu-id="43874-187">省略可能。</span><span class="sxs-lookup"><span data-stu-id="43874-187">Optional.</span></span> <span data-ttu-id="43874-188">[Schema.org](https://schema.org)の構文に従ってコンテンツの拡張の説明を %ld 個の JSON データのカスタムの一部。</span><span class="sxs-lookup"><span data-stu-id="43874-188">A custom piece of data - JSON-LD extensible description of content according to [schema.org](https://schema.org) syntax.</span></span>|
|<span data-ttu-id="43874-189">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="43874-189">expirationDateTime</span></span> | <span data-ttu-id="43874-190">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43874-190">DateTimeOffset</span></span> | <span data-ttu-id="43874-191">サーバーで設定します。</span><span class="sxs-lookup"><span data-stu-id="43874-191">Set by the server.</span></span> <span data-ttu-id="43874-192">オブジェクトは、サーバー上で有効期限が切れたときの utc 日時。</span><span class="sxs-lookup"><span data-stu-id="43874-192">DateTime in UTC when the object expired on the server.</span></span>|
|<span data-ttu-id="43874-193">status</span><span class="sxs-lookup"><span data-stu-id="43874-193">status</span></span> | <span data-ttu-id="43874-194">status</span><span class="sxs-lookup"><span data-stu-id="43874-194">status</span></span> | <span data-ttu-id="43874-195">サーバーで設定します。</span><span class="sxs-lookup"><span data-stu-id="43874-195">Set by the server.</span></span> <span data-ttu-id="43874-196">有効なオブジェクトを識別するために使用する状態コードです。</span><span class="sxs-lookup"><span data-stu-id="43874-196">A status code used to identify valid objects.</span></span> <span data-ttu-id="43874-197">値: アクティブな場合、更新、削除、無視されます。</span><span class="sxs-lookup"><span data-stu-id="43874-197">Values: active, updated, deleted, ignored.</span></span>|

## <a name="relationships"></a><span data-ttu-id="43874-198">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="43874-198">Relationships</span></span>

|<span data-ttu-id="43874-199">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="43874-199">Relationship</span></span> | <span data-ttu-id="43874-200">型</span><span class="sxs-lookup"><span data-stu-id="43874-200">Type</span></span> | <span data-ttu-id="43874-201">説明</span><span class="sxs-lookup"><span data-stu-id="43874-201">Description</span></span>|
|:------------|:-----|:-----------|
|<span data-ttu-id="43874-202">historyItems</span><span class="sxs-lookup"><span data-stu-id="43874-202">historyItems</span></span>| <span data-ttu-id="43874-203">[activityHistoryItem](../resources/projectrome-historyitem.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="43874-203">[activityHistoryItem](../resources/projectrome-historyitem.md) collection</span></span> | <span data-ttu-id="43874-204">省略可能。</span><span class="sxs-lookup"><span data-stu-id="43874-204">Optional.</span></span> <span data-ttu-id="43874-205">受け取りますおよび抑制ソリューションです。アクティビティの historyItems にナビゲーション プロパティです。</span><span class="sxs-lookup"><span data-stu-id="43874-205">NavigationProperty/Containment; navigation property to the activity's historyItems.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="43874-206">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="43874-206">JSON representation</span></span>

<span data-ttu-id="43874-207">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="43874-207">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "userTimezone",
    "appDisplayName",
    "fallbackUrl",
    "contentUrl",
    "contentInfo",
    "visualElements",
    "historyItems"
  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.userActivity",
  "@odata.annotations": [
    {
      "capabilities": {
        "countable": false,
        "selectable": false,
        "skippable": false
      }
    }
  ]
}-->

```json
{
    "appActivityId": "String",
    "activitySourceHost": "String (host name/domain/URL)",
    "userTimezone": "String",
    "appDisplayName": "String",
    "activationUrl": "String (URL)",
    "contentUrl": "String (URL)",
    "fallbackUrl": "String (URL)",
    "createdDateTime": "DateTimeOffset",
    "lastModifiedDateTime": "DateTimeOffset",
    "expirationDateTime": "DateTimeOffset",
    "id": "String",
    "status": "active | updated | deleted | ignored",
    "contentInfo": { "@odata.type": "microsoft.graph.Json" },
    "visualElements": { "@odata.type": "microsoft.graph.visualInfo" },
    "historyItems": [{ "@odata.type": "microsoft.graph.activityHistoryItem" }]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "activity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
