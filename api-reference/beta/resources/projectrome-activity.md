---
title: アクティビティのリソースの種類
description: -テレビ番組、ドキュメント、ビデオ ゲームの現在のキャンペーンなど、アプリケーション内で 1 つのアクティビティを表します。 ユーザーは、その活動と連携して、ときに、そのアクティビティの開始と終了時刻を示す履歴項目として契約がキャプチャされます。 ようにユーザーには、再、時間の経過と共にその活動と連携して、1 人のユーザーの活動の複数の項目の履歴が記録されます。
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 3d05c684d9498378a07a944f7aebd5e8a6b97f53
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573838"
---
# <a name="activity-resource-type"></a><span data-ttu-id="d44f8-105">アクティビティのリソースの種類</span><span class="sxs-lookup"><span data-stu-id="d44f8-105">activity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d44f8-106">-テレビ番組、ドキュメント、ビデオ ゲームの現在のキャンペーンなど、アプリケーション内で 1 つのアクティビティを表します。</span><span class="sxs-lookup"><span data-stu-id="d44f8-106">Represents a single activity within an app - for example, a TV show, a document, or a current campaign in a video game.</span></span> <span data-ttu-id="d44f8-107">ユーザーは、その活動と連携して、ときに、そのアクティビティの開始と終了時刻を示します、[履歴項目](projectrome-historyitem.md)として契約がキャプチャされます。</span><span class="sxs-lookup"><span data-stu-id="d44f8-107">When a user engages with that activity, the engagement is captured as a [history item](projectrome-historyitem.md) that indicates the start and end time for that activity.</span></span> <span data-ttu-id="d44f8-108">ようにユーザーには、再、時間の経過と共にその活動と連携して、1 人のユーザーの活動の複数の項目の履歴が記録されます。</span><span class="sxs-lookup"><span data-stu-id="d44f8-108">As the user re-engages with that activity over time, multiple history items are recorded for a single user activity.</span></span>

<span data-ttu-id="d44f8-109">何のアプリケーションでは、複数のデバイスを取得するのにユーザーを有効にするのに Microsoft Graph でのアクティビティを使用できます。</span><span class="sxs-lookup"><span data-stu-id="d44f8-109">You can use activities in Microsoft Graph to enable users to get back to what they were doing in their app, across multiple devices.</span></span> <span data-ttu-id="d44f8-110">アプリを作成する活動は、すべてのユーザーのデバイスに表示され、アプリ内で特定のコンテンツへの高度なリンクとしてユーザーに公開されます。</span><span class="sxs-lookup"><span data-stu-id="d44f8-110">Activities that your app creates appear on all users' devices, and are exposed to users as deep links to specific content within your app.</span></span> <span data-ttu-id="d44f8-111">Cortana の通知によってあっにアクセスし、Windows では、紹介先として、アプリケーション内で特定のコンテンツを表現できます。</span><span class="sxs-lookup"><span data-stu-id="d44f8-111">You can express specific content within your app as a destination that is showcased in Windows, and accessible on iOS and Android devices through Cortana notifications.</span></span>

<span data-ttu-id="d44f8-112">すべてのアプリケーションが異なるためにです Cortana およびタイムラインに表示されるユーザー ・ アクティビティをアプリケーション内で操作をマップする最善の方法を理解します。</span><span class="sxs-lookup"><span data-stu-id="d44f8-112">Because every app is different, it's up to you to understand the best way to map actions within your application to user activities that will appear in Cortana and Timeline.</span></span> <span data-ttu-id="d44f8-113">などのゲームは、各キャンペーンの活動を作成可能性があります、文書作成アプリケーションはそれぞれ固有のドキュメントのアクティビティを作成可能性があり、基幹業務アプリケーションは、各ワークフローのアクティビティを作成可能性があります。</span><span class="sxs-lookup"><span data-stu-id="d44f8-113">For example, games might create an activity for each campaign, document authoring apps might create an activity for each unique document, and line-of-business apps might create an activity for each workflow.</span></span>

<span data-ttu-id="d44f8-114">Cortana およびタイムラインの Windows ユーザー エクスペリエンスは、ユーザーの生産性と効率性を増やすことにより、過去に働いているコンテンツに戻ることに重点を置くに、ユーザーの作業中です。</span><span class="sxs-lookup"><span data-stu-id="d44f8-114">Your user activities will be showcased in Cortana and Windows Timeline user experiences, which are focused on increasing users' productivity and efficiency by helping them get back to content they worked on in the past.</span></span>

## <a name="methods"></a><span data-ttu-id="d44f8-115">メソッド</span><span class="sxs-lookup"><span data-stu-id="d44f8-115">Methods</span></span>

|<span data-ttu-id="d44f8-116">メソッド</span><span class="sxs-lookup"><span data-stu-id="d44f8-116">Method</span></span> | <span data-ttu-id="d44f8-117">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d44f8-117">Return Type</span></span> | <span data-ttu-id="d44f8-118">説明</span><span class="sxs-lookup"><span data-stu-id="d44f8-118">Description</span></span>|
|:------|:------------|:-----------|
|[<span data-ttu-id="d44f8-119">活動の作成または</span><span class="sxs-lookup"><span data-stu-id="d44f8-119">Create or replace activity</span></span>](../api/projectrome-put-activity.md) | [<span data-ttu-id="d44f8-120">アクティビティ</span><span class="sxs-lookup"><span data-stu-id="d44f8-120">activity</span></span>](projectrome-activity.md) |<span data-ttu-id="d44f8-121">作成または既存の活動 (アップサート) が置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="d44f8-121">Creates or replaces an existing activity (upsert).</span></span> <span data-ttu-id="d44f8-122">AppActivityId は URL セーフ (RFC 2396 の予約文字は、16 進表現に変換する必要がありますを除くすべての文字) である必要がありますが、元の appActivityId は、URL セーフである必要はありません。</span><span class="sxs-lookup"><span data-stu-id="d44f8-122">The appActivityId needs to be URL-safe (all characters except for RFC 2396 unreserved characters must be converted to their hexadecimal representation), but the original appActivityId does not have to be URL-safe.</span></span> |
|[<span data-ttu-id="d44f8-123">アクティビティを削除する</span><span class="sxs-lookup"><span data-stu-id="d44f8-123">Delete an activity</span></span>](../api/projectrome-delete-activity.md) | <span data-ttu-id="d44f8-124">内容なし</span><span class="sxs-lookup"><span data-stu-id="d44f8-124">No Content</span></span> | <span data-ttu-id="d44f8-125">アプリからそのユーザーの指定したアクティビティを削除します。</span><span class="sxs-lookup"><span data-stu-id="d44f8-125">Deletes the specified activity for that user from your app.</span></span>|
|[<span data-ttu-id="d44f8-126">アクティビティを取得します。</span><span class="sxs-lookup"><span data-stu-id="d44f8-126">Get activities</span></span>](../api/projectrome-get-activities.md) | <span data-ttu-id="d44f8-127">[活動](projectrome-activity.md)のコレクション</span><span class="sxs-lookup"><span data-stu-id="d44f8-127">Collection of [activities](projectrome-activity.md)</span></span> | <span data-ttu-id="d44f8-128">アプリが特定のユーザーのアクティビティを取得します。</span><span class="sxs-lookup"><span data-stu-id="d44f8-128">Gets the activities for your app for a given user.</span></span>|
|[<span data-ttu-id="d44f8-129">最近のアクティビティを取得する</span><span class="sxs-lookup"><span data-stu-id="d44f8-129">Get recent activities</span></span>](../api/projectrome-get-recent-activities.md) | <span data-ttu-id="d44f8-130">[活動](projectrome-activity.md)のコレクション</span><span class="sxs-lookup"><span data-stu-id="d44f8-130">Collection of [activities](projectrome-activity.md)</span></span> | <span data-ttu-id="d44f8-131">アプリが並べ替えられ、最も最近作成または更新された[historyItems](projectrome-historyitem.md)に基づいて、特定のユーザーの最新のアクティビティを取得します。</span><span class="sxs-lookup"><span data-stu-id="d44f8-131">Gets the most recent activities for your app for a given user, sorted and based on the most recently created or updated [historyItems](projectrome-historyitem.md).</span></span>|

## <a name="properties"></a><span data-ttu-id="d44f8-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d44f8-132">Properties</span></span>

|<span data-ttu-id="d44f8-133">名前</span><span class="sxs-lookup"><span data-stu-id="d44f8-133">Name</span></span> | <span data-ttu-id="d44f8-134">型</span><span class="sxs-lookup"><span data-stu-id="d44f8-134">Type</span></span> | <span data-ttu-id="d44f8-135">説明</span><span class="sxs-lookup"><span data-stu-id="d44f8-135">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="d44f8-136">userTimezone</span><span class="sxs-lookup"><span data-stu-id="d44f8-136">userTimezone</span></span> | <span data-ttu-id="d44f8-137">String</span><span class="sxs-lookup"><span data-stu-id="d44f8-137">String</span></span> | <span data-ttu-id="d44f8-138">省略可能。</span><span class="sxs-lookup"><span data-stu-id="d44f8-138">Optional.</span></span> <span data-ttu-id="d44f8-139">活動の作成時に配置されましたユーザーのデバイスのアクティビティを生成するために使用するタイム ゾーンクロスプラット フォーム形式をサポートするために、Olson の Id として指定された値です。</span><span class="sxs-lookup"><span data-stu-id="d44f8-139">The timezone in which the user's device used to generate the activity was located at activity creation time; values supplied as Olson IDs in order to support cross-platform representation.</span></span>|
|<span data-ttu-id="d44f8-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d44f8-140">createdDateTime</span></span> | <span data-ttu-id="d44f8-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d44f8-141">DateTimeOffset</span></span> | <span data-ttu-id="d44f8-142">サーバーで設定します。</span><span class="sxs-lookup"><span data-stu-id="d44f8-142">Set by the server.</span></span> <span data-ttu-id="d44f8-143">サーバー上にオブジェクトが作成されたときの utc 日時。</span><span class="sxs-lookup"><span data-stu-id="d44f8-143">DateTime in UTC when the object was created on the server.</span></span> |
|<span data-ttu-id="d44f8-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d44f8-144">lastModifiedDateTime</span></span> | <span data-ttu-id="d44f8-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d44f8-145">DateTimeOffset</span></span> | <span data-ttu-id="d44f8-146">サーバーで設定します。</span><span class="sxs-lookup"><span data-stu-id="d44f8-146">Set by the server.</span></span> <span data-ttu-id="d44f8-147">サーバー上にオブジェクトが変更されたときの utc 日時。</span><span class="sxs-lookup"><span data-stu-id="d44f8-147">DateTime in UTC when the object was modified on the server.</span></span> |
|<span data-ttu-id="d44f8-148">id</span><span class="sxs-lookup"><span data-stu-id="d44f8-148">id</span></span> | <span data-ttu-id="d44f8-149">String</span><span class="sxs-lookup"><span data-stu-id="d44f8-149">String</span></span> | <span data-ttu-id="d44f8-150">サーバーによって生成される ID が URL に対応するために使用します。</span><span class="sxs-lookup"><span data-stu-id="d44f8-150">Server-generated ID used for URL addressing.</span></span>|
|<span data-ttu-id="d44f8-151">appActivityId</span><span class="sxs-lookup"><span data-stu-id="d44f8-151">appActivityId</span></span> | <span data-ttu-id="d44f8-152">String</span><span class="sxs-lookup"><span data-stu-id="d44f8-152">String</span></span> | <span data-ttu-id="d44f8-153">必須。</span><span class="sxs-lookup"><span data-stu-id="d44f8-153">Required.</span></span> <span data-ttu-id="d44f8-154">呼び出し元によって、不変をその後提供された - アプリケーションのコンテキストで一意のアクティビティ ID です。</span><span class="sxs-lookup"><span data-stu-id="d44f8-154">The unique activity ID in the context of the app - supplied by caller and immutable thereafter.</span></span>|
|<span data-ttu-id="d44f8-155">activitySourceHost</span><span class="sxs-lookup"><span data-stu-id="d44f8-155">activitySourceHost</span></span> | <span data-ttu-id="d44f8-156">String</span><span class="sxs-lookup"><span data-stu-id="d44f8-156">String</span></span> | <span data-ttu-id="d44f8-157">必須。</span><span class="sxs-lookup"><span data-stu-id="d44f8-157">Required.</span></span> <span data-ttu-id="d44f8-158">アプリケーションのクロスプラット フォームの id のマッピングを表すドメインの URL です。</span><span class="sxs-lookup"><span data-stu-id="d44f8-158">URL for the domain representing the cross-platform identity mapping for the app.</span></span> <span data-ttu-id="d44f8-159">マッピングは、ドメインでホストされている JSON ファイルとして、ストアドや Windows デベロッパー センターを使用して構成できます。</span><span class="sxs-lookup"><span data-stu-id="d44f8-159">Mapping is stored either as a JSON file hosted on the domain or configurable via Windows Dev Center.</span></span> <span data-ttu-id="d44f8-160">JSON ファイルは、クロス プラットフォーム アプリケーション識別子の名前はまたはトップ レベルのドメイン レベルのいずれか、"HTTPS"ドメインのルートでホストされていますとサブのドメインが含まれます。</span><span class="sxs-lookup"><span data-stu-id="d44f8-160">The JSON file is named cross-platform-app-identifiers and is hosted at root of your HTTPS domain, either at the top level domain or include a sub domain.</span></span> <span data-ttu-id="d44f8-161">例: https://contoso.com または https://myapp.contoso.com。しかし、https://myapp.contoso.com/somepath は無効です。</span><span class="sxs-lookup"><span data-stu-id="d44f8-161">For example: https://contoso.com or https://myapp.contoso.com but NOT https://myapp.contoso.com/somepath.</span></span> <span data-ttu-id="d44f8-162">クロスプラット フォームのアプリケーション id ごと、一意のファイルおよびドメイン (またはサブドメイン) をすることが必要です。</span><span class="sxs-lookup"><span data-stu-id="d44f8-162">You must have a unique file and domain (or sub domain) per cross-platform app identity.</span></span> <span data-ttu-id="d44f8-163">たとえば、PowerPoint と Word の別のファイルとドメインが必要です。</span><span class="sxs-lookup"><span data-stu-id="d44f8-163">For example, a separate file and domain is needed for Word vs. PowerPoint.</span></span>|
|<span data-ttu-id="d44f8-164">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="d44f8-164">appDisplayName</span></span> | <span data-ttu-id="d44f8-165">String</span><span class="sxs-lookup"><span data-stu-id="d44f8-165">String</span></span> | <span data-ttu-id="d44f8-166">省略可能。</span><span class="sxs-lookup"><span data-stu-id="d44f8-166">Optional.</span></span> <span data-ttu-id="d44f8-167">アプリケーションがユーザーのローカル デバイスにインストールされていない場合の場合に使用するための活動を生成するために使用するアプリケーションの短い説明です。</span><span class="sxs-lookup"><span data-stu-id="d44f8-167">Short text description of the app used to generate the activity for use in cases when the app is not installed on the user’s local device.</span></span>|
|<span data-ttu-id="d44f8-168">activationUrl</span><span class="sxs-lookup"><span data-stu-id="d44f8-168">activationUrl</span></span> | <span data-ttu-id="d44f8-169">String</span><span class="sxs-lookup"><span data-stu-id="d44f8-169">String</span></span> | <span data-ttu-id="d44f8-170">必須。</span><span class="sxs-lookup"><span data-stu-id="d44f8-170">Required.</span></span> <span data-ttu-id="d44f8-171">AppId によって表される最適なネイティブの経験ではアクティビティを起動するために使用する URL です。</span><span class="sxs-lookup"><span data-stu-id="d44f8-171">URL used to launch the activity in the best native experience represented by the appId.</span></span> <span data-ttu-id="d44f8-172">ネイティブ アプリケーションが存在しない場合は、web ベースのアプリケーションを起動する場合があります。</span><span class="sxs-lookup"><span data-stu-id="d44f8-172">Might launch a web-based app if no native app exists.</span></span>|
|<span data-ttu-id="d44f8-173">fallbackUrl</span><span class="sxs-lookup"><span data-stu-id="d44f8-173">fallbackUrl</span></span> | <span data-ttu-id="d44f8-174">String</span><span class="sxs-lookup"><span data-stu-id="d44f8-174">String</span></span> | <span data-ttu-id="d44f8-175">省略可能。</span><span class="sxs-lookup"><span data-stu-id="d44f8-175">Optional.</span></span> <span data-ttu-id="d44f8-176">URL が利用可能な場合は、web ベースのアプリケーションでは、アクティビティの起動に使用します。</span><span class="sxs-lookup"><span data-stu-id="d44f8-176">URL used to launch the activity in a web-based app, if available.</span></span>|
|<span data-ttu-id="d44f8-177">contentUrl</span><span class="sxs-lookup"><span data-stu-id="d44f8-177">contentUrl</span></span> | <span data-ttu-id="d44f8-178">String</span><span class="sxs-lookup"><span data-stu-id="d44f8-178">String</span></span> | <span data-ttu-id="d44f8-179">省略可能。</span><span class="sxs-lookup"><span data-stu-id="d44f8-179">Optional.</span></span> <span data-ttu-id="d44f8-180">ネイティブまたは web ベースのアプリケーションの操作 (たとえば、RSS フィード内のアイテムへのポインター) の外部コンテンツを表示できる場合に使用されます。</span><span class="sxs-lookup"><span data-stu-id="d44f8-180">Used in the event the content can be rendered outside of a native or web-based app experience (for example, a pointer to an item in an RSS feed).</span></span>|
|<span data-ttu-id="d44f8-181">visualElements</span><span class="sxs-lookup"><span data-stu-id="d44f8-181">visualElements</span></span>| [<span data-ttu-id="d44f8-182">visualInfo</span><span class="sxs-lookup"><span data-stu-id="d44f8-182">visualInfo</span></span>](../resources/projectrome-visualinfo.md) | <span data-ttu-id="d44f8-183">必須です。</span><span class="sxs-lookup"><span data-stu-id="d44f8-183">Required.</span></span> <span data-ttu-id="d44f8-184">エクスペリエンスの利用状況を表示する情報を格納しているオブジェクト</span><span class="sxs-lookup"><span data-stu-id="d44f8-184">The object containing information to render the activity in the UX.</span></span>|
|<span data-ttu-id="d44f8-185">contentInfo</span><span class="sxs-lookup"><span data-stu-id="d44f8-185">contentInfo</span></span> | <span data-ttu-id="d44f8-186">JSON オブジェクトの型指定されていません。</span><span class="sxs-lookup"><span data-stu-id="d44f8-186">Untyped JSON object</span></span> | <span data-ttu-id="d44f8-187">省略可能。</span><span class="sxs-lookup"><span data-stu-id="d44f8-187">Optional.</span></span> <span data-ttu-id="d44f8-188">[Schema.org](https://schema.org)の構文に従ってコンテンツの拡張の説明を %ld 個の JSON データのカスタムの一部。</span><span class="sxs-lookup"><span data-stu-id="d44f8-188">A custom piece of data - JSON-LD extensible description of content according to [schema.org](https://schema.org) syntax.</span></span>|
|<span data-ttu-id="d44f8-189">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="d44f8-189">expirationDateTime</span></span> | <span data-ttu-id="d44f8-190">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d44f8-190">DateTimeOffset</span></span> | <span data-ttu-id="d44f8-191">サーバーで設定します。</span><span class="sxs-lookup"><span data-stu-id="d44f8-191">Set by the server.</span></span> <span data-ttu-id="d44f8-192">オブジェクトは、サーバー上で有効期限が切れたときの utc 日時。</span><span class="sxs-lookup"><span data-stu-id="d44f8-192">DateTime in UTC when the object expired on the server.</span></span>|
|<span data-ttu-id="d44f8-193">status</span><span class="sxs-lookup"><span data-stu-id="d44f8-193">status</span></span> | <span data-ttu-id="d44f8-194">列挙型文字列</span><span class="sxs-lookup"><span data-stu-id="d44f8-194">enum-string</span></span> | <span data-ttu-id="d44f8-195">サーバーで設定します。</span><span class="sxs-lookup"><span data-stu-id="d44f8-195">Set by the server.</span></span> <span data-ttu-id="d44f8-196">有効なオブジェクトを識別するために使用する状態コードです。</span><span class="sxs-lookup"><span data-stu-id="d44f8-196">A status code used to identify valid objects.</span></span> <span data-ttu-id="d44f8-197">値: アクティブな場合、更新、削除、無視されます。</span><span class="sxs-lookup"><span data-stu-id="d44f8-197">Values: active, updated, deleted, ignored.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d44f8-198">関係</span><span class="sxs-lookup"><span data-stu-id="d44f8-198">Relationships</span></span>

|<span data-ttu-id="d44f8-199">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d44f8-199">Relationship</span></span> | <span data-ttu-id="d44f8-200">型</span><span class="sxs-lookup"><span data-stu-id="d44f8-200">Type</span></span> | <span data-ttu-id="d44f8-201">説明</span><span class="sxs-lookup"><span data-stu-id="d44f8-201">Description</span></span>|
|:------------|:-----|:-----------|
|<span data-ttu-id="d44f8-202">historyItems</span><span class="sxs-lookup"><span data-stu-id="d44f8-202">historyItems</span></span>| <span data-ttu-id="d44f8-203">[historyItem](../resources/projectrome-historyitem.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="d44f8-203">[historyItem](../resources/projectrome-historyitem.md) collection</span></span> | <span data-ttu-id="d44f8-204">省略可能。</span><span class="sxs-lookup"><span data-stu-id="d44f8-204">Optional.</span></span> <span data-ttu-id="d44f8-205">受け取りますおよび抑制ソリューションです。アクティビティの historyItems にナビゲーション プロパティです。</span><span class="sxs-lookup"><span data-stu-id="d44f8-205">NavigationProperty/Containment; navigation property to the activity's historyItems.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d44f8-206">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d44f8-206">JSON representation</span></span>

<span data-ttu-id="d44f8-207">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d44f8-207">Here is a JSON representation of the resource.</span></span>

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
    "status": "active | updated | deleted | ignored",
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
