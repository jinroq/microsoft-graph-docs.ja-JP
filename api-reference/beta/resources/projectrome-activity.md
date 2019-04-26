---
title: アクティビティリソースの種類
description: アプリ内の1つのアクティビティを表します。たとえば、テレビ番組、ドキュメント、ビデオゲームの現在のキャンペーンなどがあります。 ユーザーがそのアクティビティを使用すると、そのアクティビティの開始時刻と終了時刻を示す履歴項目として契約が取得されます。 ユーザーが時間をかけてそのアクティビティを再実行すると、1つのユーザーアクティビティに対して複数の履歴項目が記録されます。
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 5deaab5d7ea071bfda686380d49fb41214a7b29e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563391"
---
# <a name="activity-resource-type"></a><span data-ttu-id="7062b-105">アクティビティリソースの種類</span><span class="sxs-lookup"><span data-stu-id="7062b-105">activity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7062b-106">アプリ内の1つのアクティビティを表します。たとえば、テレビ番組、ドキュメント、ビデオゲームの現在のキャンペーンなどがあります。</span><span class="sxs-lookup"><span data-stu-id="7062b-106">Represents a single activity within an app - for example, a TV show, a document, or a current campaign in a video game.</span></span> <span data-ttu-id="7062b-107">ユーザーがそのアクティビティを使用すると、そのアクティビティの開始時刻と終了時刻を示す[履歴項目](projectrome-historyitem.md)として契約が取得されます。</span><span class="sxs-lookup"><span data-stu-id="7062b-107">When a user engages with that activity, the engagement is captured as a [history item](projectrome-historyitem.md) that indicates the start and end time for that activity.</span></span> <span data-ttu-id="7062b-108">ユーザーが時間をかけてそのアクティビティを再実行すると、1つのユーザーアクティビティに対して複数の履歴項目が記録されます。</span><span class="sxs-lookup"><span data-stu-id="7062b-108">As the user re-engages with that activity over time, multiple history items are recorded for a single user activity.</span></span>

<span data-ttu-id="7062b-109">Microsoft Graph のアクティビティを使用すると、ユーザーが複数のデバイスでアプリで実行していた操作に戻れるようにすることができます。</span><span class="sxs-lookup"><span data-stu-id="7062b-109">You can use activities in Microsoft Graph to enable users to get back to what they were doing in their app, across multiple devices.</span></span> <span data-ttu-id="7062b-110">アプリによって作成されるアクティビティは、すべてのユーザーのデバイスに表示され、アプリ内の特定のコンテンツへの詳細なリンクとしてユーザーに公開されます。</span><span class="sxs-lookup"><span data-stu-id="7062b-110">Activities that your app creates appear on all users' devices, and are exposed to users as deep links to specific content within your app.</span></span> <span data-ttu-id="7062b-111">アプリ内の特定のコンテンツを、Windows で紹介されている送信先として表現し、Cortana 通知を介して iOS および Android デバイスでアクセスすることができます。</span><span class="sxs-lookup"><span data-stu-id="7062b-111">You can express specific content within your app as a destination that is showcased in Windows, and accessible on iOS and Android devices through Cortana notifications.</span></span>

<span data-ttu-id="7062b-112">すべてのアプリは異なるため、アプリケーション内のアクションを Cortana とタイムラインで表示されるユーザーアクティビティにマップするための最善の方法を理解しておく必要があります。</span><span class="sxs-lookup"><span data-stu-id="7062b-112">Because every app is different, it's up to you to understand the best way to map actions within your application to user activities that will appear in Cortana and Timeline.</span></span> <span data-ttu-id="7062b-113">たとえば、ゲームは各キャンペーンに対してアクティビティを作成し、ドキュメント作成アプリは固有のドキュメントごとにアクティビティを作成し、基幹業務アプリは各ワークフローのアクティビティを作成する場合があります。</span><span class="sxs-lookup"><span data-stu-id="7062b-113">For example, games might create an activity for each campaign, document authoring apps might create an activity for each unique document, and line-of-business apps might create an activity for each workflow.</span></span>

<span data-ttu-id="7062b-114">ユーザーのアクティビティは、Cortana および Windows タイムラインのユーザーエクスペリエンスで紹介されています。これは、ユーザーが過去に作業したコンテンツに戻れるようにすることによって、ユーザーの生産性と効率を向上させることに重点を置いています。</span><span class="sxs-lookup"><span data-stu-id="7062b-114">Your user activities will be showcased in Cortana and Windows Timeline user experiences, which are focused on increasing users' productivity and efficiency by helping them get back to content they worked on in the past.</span></span>

## <a name="methods"></a><span data-ttu-id="7062b-115">メソッド</span><span class="sxs-lookup"><span data-stu-id="7062b-115">Methods</span></span>

|<span data-ttu-id="7062b-116">メソッド</span><span class="sxs-lookup"><span data-stu-id="7062b-116">Method</span></span> | <span data-ttu-id="7062b-117">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="7062b-117">Return Type</span></span> | <span data-ttu-id="7062b-118">説明</span><span class="sxs-lookup"><span data-stu-id="7062b-118">Description</span></span>|
|:------|:------------|:-----------|
|[<span data-ttu-id="7062b-119">アクティビティを作成または置換する</span><span class="sxs-lookup"><span data-stu-id="7062b-119">Create or replace activity</span></span>](../api/projectrome-put-activity.md) | [<span data-ttu-id="7062b-120">アクティビティ</span><span class="sxs-lookup"><span data-stu-id="7062b-120">activity</span></span>](projectrome-activity.md) |<span data-ttu-id="7062b-121">既存のアクティビティ (upsert) を作成または置換します。</span><span class="sxs-lookup"><span data-stu-id="7062b-121">Creates or replaces an existing activity (upsert).</span></span> <span data-ttu-id="7062b-122">appactivityid は url セーフである必要があります (RFC 2396 の予約されていない文字を除くすべての文字を16進表記に変換する必要があります) が、元の appactivityid を url セーフにする必要はありません。</span><span class="sxs-lookup"><span data-stu-id="7062b-122">The appActivityId needs to be URL-safe (all characters except for RFC 2396 unreserved characters must be converted to their hexadecimal representation), but the original appActivityId does not have to be URL-safe.</span></span> |
|[<span data-ttu-id="7062b-123">アクティビティを削除する</span><span class="sxs-lookup"><span data-stu-id="7062b-123">Delete an activity</span></span>](../api/projectrome-delete-activity.md) | <span data-ttu-id="7062b-124">No Content</span><span class="sxs-lookup"><span data-stu-id="7062b-124">No Content</span></span> | <span data-ttu-id="7062b-125">そのユーザーの指定したアクティビティをアプリから削除します。</span><span class="sxs-lookup"><span data-stu-id="7062b-125">Deletes the specified activity for that user from your app.</span></span>|
|[<span data-ttu-id="7062b-126">アクティビティを取得する</span><span class="sxs-lookup"><span data-stu-id="7062b-126">Get activities</span></span>](../api/projectrome-get-activities.md) | <span data-ttu-id="7062b-127">[アクティビティ](projectrome-activity.md)のコレクション</span><span class="sxs-lookup"><span data-stu-id="7062b-127">Collection of [activities](projectrome-activity.md)</span></span> | <span data-ttu-id="7062b-128">特定のユーザーのアプリのアクティビティを取得します。</span><span class="sxs-lookup"><span data-stu-id="7062b-128">Gets the activities for your app for a given user.</span></span>|
|[<span data-ttu-id="7062b-129">最近のアクティビティを取得する</span><span class="sxs-lookup"><span data-stu-id="7062b-129">Get recent activities</span></span>](../api/projectrome-get-recent-activities.md) | <span data-ttu-id="7062b-130">[アクティビティ](projectrome-activity.md)のコレクション</span><span class="sxs-lookup"><span data-stu-id="7062b-130">Collection of [activities](projectrome-activity.md)</span></span> | <span data-ttu-id="7062b-131">指定されたユーザーのアプリの最新のアクティビティを取得し、最後に作成または更新された[履歴アイテム](projectrome-historyitem.md)に基づいて並べ替えます。</span><span class="sxs-lookup"><span data-stu-id="7062b-131">Gets the most recent activities for your app for a given user, sorted and based on the most recently created or updated [historyItems](projectrome-historyitem.md).</span></span>|

## <a name="properties"></a><span data-ttu-id="7062b-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7062b-132">Properties</span></span>

|<span data-ttu-id="7062b-133">名前</span><span class="sxs-lookup"><span data-stu-id="7062b-133">Name</span></span> | <span data-ttu-id="7062b-134">型</span><span class="sxs-lookup"><span data-stu-id="7062b-134">Type</span></span> | <span data-ttu-id="7062b-135">説明</span><span class="sxs-lookup"><span data-stu-id="7062b-135">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="7062b-136">usertimezone</span><span class="sxs-lookup"><span data-stu-id="7062b-136">userTimezone</span></span> | <span data-ttu-id="7062b-137">String</span><span class="sxs-lookup"><span data-stu-id="7062b-137">String</span></span> | <span data-ttu-id="7062b-138">省略可能。</span><span class="sxs-lookup"><span data-stu-id="7062b-138">Optional.</span></span> <span data-ttu-id="7062b-139">アクティビティを生成するために使用されたユーザーのデバイスがアクティビティの作成時にあるタイムゾーン。クロスプラットフォーム表現をサポートするために olson id として提供される値。</span><span class="sxs-lookup"><span data-stu-id="7062b-139">The timezone in which the user's device used to generate the activity was located at activity creation time; values supplied as Olson IDs in order to support cross-platform representation.</span></span>|
|<span data-ttu-id="7062b-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7062b-140">createdDateTime</span></span> | <span data-ttu-id="7062b-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7062b-141">DateTimeOffset</span></span> | <span data-ttu-id="7062b-142">サーバーによって設定されます。</span><span class="sxs-lookup"><span data-stu-id="7062b-142">Set by the server.</span></span> <span data-ttu-id="7062b-143">サーバー上でオブジェクトが作成された日時 (UTC)。</span><span class="sxs-lookup"><span data-stu-id="7062b-143">DateTime in UTC when the object was created on the server.</span></span> |
|<span data-ttu-id="7062b-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7062b-144">lastModifiedDateTime</span></span> | <span data-ttu-id="7062b-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7062b-145">DateTimeOffset</span></span> | <span data-ttu-id="7062b-146">サーバーによって設定されます。</span><span class="sxs-lookup"><span data-stu-id="7062b-146">Set by the server.</span></span> <span data-ttu-id="7062b-147">サーバー上のオブジェクトが変更された日時 (UTC)。</span><span class="sxs-lookup"><span data-stu-id="7062b-147">DateTime in UTC when the object was modified on the server.</span></span> |
|<span data-ttu-id="7062b-148">id</span><span class="sxs-lookup"><span data-stu-id="7062b-148">id</span></span> | <span data-ttu-id="7062b-149">String</span><span class="sxs-lookup"><span data-stu-id="7062b-149">String</span></span> | <span data-ttu-id="7062b-150">サーバーによって生成された ID。 URL アドレス指定に使用されます。</span><span class="sxs-lookup"><span data-stu-id="7062b-150">Server-generated ID used for URL addressing.</span></span>|
|<span data-ttu-id="7062b-151">appactivityid</span><span class="sxs-lookup"><span data-stu-id="7062b-151">appActivityId</span></span> | <span data-ttu-id="7062b-152">String</span><span class="sxs-lookup"><span data-stu-id="7062b-152">String</span></span> | <span data-ttu-id="7062b-153">必須。</span><span class="sxs-lookup"><span data-stu-id="7062b-153">Required.</span></span> <span data-ttu-id="7062b-154">発信者によって提供される、またはその後に不変である、アプリのコンテキスト内の一意のアクティビティ ID。</span><span class="sxs-lookup"><span data-stu-id="7062b-154">The unique activity ID in the context of the app - supplied by caller and immutable thereafter.</span></span>|
|<span data-ttu-id="7062b-155">activitysourcehost</span><span class="sxs-lookup"><span data-stu-id="7062b-155">activitySourceHost</span></span> | <span data-ttu-id="7062b-156">String</span><span class="sxs-lookup"><span data-stu-id="7062b-156">String</span></span> | <span data-ttu-id="7062b-157">必須。</span><span class="sxs-lookup"><span data-stu-id="7062b-157">Required.</span></span> <span data-ttu-id="7062b-158">アプリのクロスプラットフォーム id マッピングを表すドメインの URL。</span><span class="sxs-lookup"><span data-stu-id="7062b-158">URL for the domain representing the cross-platform identity mapping for the app.</span></span> <span data-ttu-id="7062b-159">マッピングは、ドメインでホストされている JSON ファイルとして、または Windows デベロッパーセンターから構成可能な JSON ファイルのいずれかとして格納されます。</span><span class="sxs-lookup"><span data-stu-id="7062b-159">Mapping is stored either as a JSON file hosted on the domain or configurable via Windows Dev Center.</span></span> <span data-ttu-id="7062b-160">JSON ファイルは、クロスプラットフォームアプリ識別子と呼ばれ、トップレベルドメインまたはサブドメインを含む HTTPS ドメインのルートでホストされます。</span><span class="sxs-lookup"><span data-stu-id="7062b-160">The JSON file is named cross-platform-app-identifiers and is hosted at root of your HTTPS domain, either at the top level domain or include a sub domain.</span></span> <span data-ttu-id="7062b-161">例: https://contoso.com または https://myapp.contoso.com。しかし、https://myapp.contoso.com/somepath は無効です。</span><span class="sxs-lookup"><span data-stu-id="7062b-161">For example: https://contoso.com or https://myapp.contoso.com but NOT https://myapp.contoso.com/somepath.</span></span> <span data-ttu-id="7062b-162">クロスプラットフォームのアプリ id ごとに一意のファイルとドメイン (またはサブドメイン) が必要です。</span><span class="sxs-lookup"><span data-stu-id="7062b-162">You must have a unique file and domain (or sub domain) per cross-platform app identity.</span></span> <span data-ttu-id="7062b-163">たとえば、Word と PowerPoint では、別のファイルとドメインが必要になります。</span><span class="sxs-lookup"><span data-stu-id="7062b-163">For example, a separate file and domain is needed for Word vs. PowerPoint.</span></span>|
|<span data-ttu-id="7062b-164">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="7062b-164">appDisplayName</span></span> | <span data-ttu-id="7062b-165">String</span><span class="sxs-lookup"><span data-stu-id="7062b-165">String</span></span> | <span data-ttu-id="7062b-166">省略可能。</span><span class="sxs-lookup"><span data-stu-id="7062b-166">Optional.</span></span> <span data-ttu-id="7062b-167">アプリがユーザーのローカルデバイスにインストールされていない場合に使用するアクティビティの生成に使用するアプリの短いテキストの説明。</span><span class="sxs-lookup"><span data-stu-id="7062b-167">Short text description of the app used to generate the activity for use in cases when the app is not installed on the user’s local device.</span></span>|
|<span data-ttu-id="7062b-168">activationUrl</span><span class="sxs-lookup"><span data-stu-id="7062b-168">activationUrl</span></span> | <span data-ttu-id="7062b-169">String</span><span class="sxs-lookup"><span data-stu-id="7062b-169">String</span></span> | <span data-ttu-id="7062b-170">必須。</span><span class="sxs-lookup"><span data-stu-id="7062b-170">Required.</span></span> <span data-ttu-id="7062b-171">appId で表される最高のネイティブの操作でアクティビティを開始するために使用される URL。</span><span class="sxs-lookup"><span data-stu-id="7062b-171">URL used to launch the activity in the best native experience represented by the appId.</span></span> <span data-ttu-id="7062b-172">ネイティブアプリが存在しない場合は、web ベースのアプリを起動する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="7062b-172">Might launch a web-based app if no native app exists.</span></span>|
|<span data-ttu-id="7062b-173">fallbackurl</span><span class="sxs-lookup"><span data-stu-id="7062b-173">fallbackUrl</span></span> | <span data-ttu-id="7062b-174">String</span><span class="sxs-lookup"><span data-stu-id="7062b-174">String</span></span> | <span data-ttu-id="7062b-175">省略可能。</span><span class="sxs-lookup"><span data-stu-id="7062b-175">Optional.</span></span> <span data-ttu-id="7062b-176">web ベースのアプリでアクティビティを起動するために使用される URL (可能な場合)。</span><span class="sxs-lookup"><span data-stu-id="7062b-176">URL used to launch the activity in a web-based app, if available.</span></span>|
|<span data-ttu-id="7062b-177">contentUrl</span><span class="sxs-lookup"><span data-stu-id="7062b-177">contentUrl</span></span> | <span data-ttu-id="7062b-178">String</span><span class="sxs-lookup"><span data-stu-id="7062b-178">String</span></span> | <span data-ttu-id="7062b-179">省略可能。</span><span class="sxs-lookup"><span data-stu-id="7062b-179">Optional.</span></span> <span data-ttu-id="7062b-180">ネイティブまたは web ベースのアプリの使用状況 (RSS フィード内のアイテムへのポインターなど) の外部でコンテンツをレンダリングできる場合に使用します。</span><span class="sxs-lookup"><span data-stu-id="7062b-180">Used in the event the content can be rendered outside of a native or web-based app experience (for example, a pointer to an item in an RSS feed).</span></span>|
|<span data-ttu-id="7062b-181">visualelements</span><span class="sxs-lookup"><span data-stu-id="7062b-181">visualElements</span></span>| [<span data-ttu-id="7062b-182">visualinfo</span><span class="sxs-lookup"><span data-stu-id="7062b-182">visualInfo</span></span>](../resources/projectrome-visualinfo.md) | <span data-ttu-id="7062b-183">必須です。</span><span class="sxs-lookup"><span data-stu-id="7062b-183">Required.</span></span> <span data-ttu-id="7062b-184">UX でアクティビティをレンダリングするための情報を含むオブジェクト。</span><span class="sxs-lookup"><span data-stu-id="7062b-184">The object containing information to render the activity in the UX.</span></span>|
|<span data-ttu-id="7062b-185">contentinfo</span><span class="sxs-lookup"><span data-stu-id="7062b-185">contentInfo</span></span> | <span data-ttu-id="7062b-186">型指定のない JSON オブジェクト</span><span class="sxs-lookup"><span data-stu-id="7062b-186">Untyped JSON object</span></span> | <span data-ttu-id="7062b-187">省略可能。</span><span class="sxs-lookup"><span data-stu-id="7062b-187">Optional.</span></span> <span data-ttu-id="7062b-188">[schema.org](https://schema.org)構文に従ったコンテンツの、データのカスタム部分。</span><span class="sxs-lookup"><span data-stu-id="7062b-188">A custom piece of data - JSON-LD extensible description of content according to [schema.org](https://schema.org) syntax.</span></span>|
|<span data-ttu-id="7062b-189">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="7062b-189">expirationDateTime</span></span> | <span data-ttu-id="7062b-190">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7062b-190">DateTimeOffset</span></span> | <span data-ttu-id="7062b-191">サーバーによって設定されます。</span><span class="sxs-lookup"><span data-stu-id="7062b-191">Set by the server.</span></span> <span data-ttu-id="7062b-192">サーバー上のオブジェクトの有効期限が切れたときの日時。</span><span class="sxs-lookup"><span data-stu-id="7062b-192">DateTime in UTC when the object expired on the server.</span></span>|
|<span data-ttu-id="7062b-193">status</span><span class="sxs-lookup"><span data-stu-id="7062b-193">status</span></span> | <span data-ttu-id="7062b-194">EnumType</span><span class="sxs-lookup"><span data-stu-id="7062b-194">EnumType</span></span> | <span data-ttu-id="7062b-195">サーバーによって設定されます。</span><span class="sxs-lookup"><span data-stu-id="7062b-195">Set by the server.</span></span> <span data-ttu-id="7062b-196">有効なオブジェクトを識別するために使用される状態コード。</span><span class="sxs-lookup"><span data-stu-id="7062b-196">A status code used to identify valid objects.</span></span> <span data-ttu-id="7062b-197">値: アクティブ、更新済み、削除済み、無視。</span><span class="sxs-lookup"><span data-stu-id="7062b-197">Values: active, updated, deleted, ignored.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7062b-198">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7062b-198">Relationships</span></span>

|<span data-ttu-id="7062b-199">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7062b-199">Relationship</span></span> | <span data-ttu-id="7062b-200">型</span><span class="sxs-lookup"><span data-stu-id="7062b-200">Type</span></span> | <span data-ttu-id="7062b-201">説明</span><span class="sxs-lookup"><span data-stu-id="7062b-201">Description</span></span>|
|:------------|:-----|:-----------|
|<span data-ttu-id="7062b-202">historyItems</span><span class="sxs-lookup"><span data-stu-id="7062b-202">historyItems</span></span>| <span data-ttu-id="7062b-203">[履歴アイテム](../resources/projectrome-historyitem.md)のコレクション</span><span class="sxs-lookup"><span data-stu-id="7062b-203">[historyItem](../resources/projectrome-historyitem.md) collection</span></span> | <span data-ttu-id="7062b-204">省略可能。</span><span class="sxs-lookup"><span data-stu-id="7062b-204">Optional.</span></span> <span data-ttu-id="7062b-205">NavigationProperty/コンテインメント;アクティビティの履歴アイテムへのナビゲーションプロパティ。</span><span class="sxs-lookup"><span data-stu-id="7062b-205">NavigationProperty/Containment; navigation property to the activity's historyItems.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7062b-206">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7062b-206">JSON representation</span></span>

<span data-ttu-id="7062b-207">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7062b-207">Here is a JSON representation of the resource.</span></span>

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
  "@odata.type": "microsoft.graph.activity"
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
    "status": "EnumType",
    "contentInfo": { "@data.type": "microsoft.graph.Json" },
    "visualElements": { "@data.type": "microsoft.graph.visualInfo" },
    "historyItems": [{ "@odata.type": "microsoft.graph.historyItem" }]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "activity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/projectrome-activity.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
