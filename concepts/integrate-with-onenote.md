---
title: OneNote API の概要
description: OneNote は、顧客が Web、電話、タブレット、またはデスクトップ上で文字、スケッチ、音声を入力することで、家庭、学校、または職場用のアイデアやメモを追跡できるデジタル ノートブックです。 自由にメモを整理し、デバイスを切り替えて作業の中断箇所から再開し、他のユーザーとリアルタイムでメモの共同作業を行えます。
author: Jewan-microsoft
localization_priority: Priority
ms.openlocfilehash: 7431bab05f0a749e20dd032f0b8472a1a822623d
ms.sourcegitcommit: 7c03131291113c343a98bb0234d31bd4535a4050
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/22/2019
ms.locfileid: "35133832"
---
# <a name="onenote-api-overview"></a><span data-ttu-id="e977e-104">OneNote API の概要</span><span class="sxs-lookup"><span data-stu-id="e977e-104">OneNote API overview</span></span>

<span data-ttu-id="e977e-105">OneNote は、顧客が Web、電話、タブレット、またはデスクトップ上で文字、スケッチ、音声を入力することで、家庭、学校、または職場用のアイデアやメモを追跡できるデジタル ノートブックです。</span><span class="sxs-lookup"><span data-stu-id="e977e-105">OneNote is a digital notebook that lets customers track ideas and notes for home, school, or work, by typing, sketching, or voice, on the web, phone, tablet, or desktop.</span></span> <span data-ttu-id="e977e-106">自由にメモを整理し、デバイスを切り替えて作業の中断箇所から再開し、他のユーザーとリアルタイムでメモの共同作業を行えます。</span><span class="sxs-lookup"><span data-stu-id="e977e-106">They can freely organize notes, switch devices and pick up where they left off, and collaborate on notes with others in real time.</span></span>

> [!VIDEO https://www.youtube-nocookie.com/embed/VXd4OeQU1ek]

## <a name="why-integrate-with-onenote"></a><span data-ttu-id="e977e-107">OneNote と統合する理由</span><span class="sxs-lookup"><span data-stu-id="e977e-107">Why integrate with OneNote?</span></span>

<span data-ttu-id="e977e-108">アプリを OneNote に統合すると、複数のプラットフォームで利用できる便利な機能を作成し、世界中の数百万人のユーザーに届けることができます。</span><span class="sxs-lookup"><span data-stu-id="e977e-108">By integrating your apps with OneNote, you can create empowering experiences across multiple platforms that reach millions of users worldwide.</span></span> <span data-ttu-id="e977e-109">Microsoft Graph を使用して OneNote のノートブック、セクション、ページにアクセスし、ユーザーによるアイデアや情報の計画や整理を支援するソリューションを作成することができます。</span><span class="sxs-lookup"><span data-stu-id="e977e-109">You can use Microsoft Graph to access notebooks, sections, and pages in OneNote to create solutions that help your users plan and organize ideas and information.</span></span>

### <a name="collect-and-organize-notes-and-ideas"></a><span data-ttu-id="e977e-110">メモやアイデアを収集して整理する</span><span class="sxs-lookup"><span data-stu-id="e977e-110">Collect and organize notes and ideas</span></span>  

<span data-ttu-id="e977e-111">コンテンツを追加したり、アレンジしたりできるキャンバスとして OneNote を使用します。</span><span class="sxs-lookup"><span data-stu-id="e977e-111">Use OneNote as a canvas where users can add and arrange their content.</span></span> <span data-ttu-id="e977e-112">Microsoft Graph を使用すると、学生がメモを取って調査すること、家族が計画とアイデアを共有すること、買い物客が画像を共有することを可能にするアプリを簡単に作成できます。</span><span class="sxs-lookup"><span data-stu-id="e977e-112">Microsoft Graph makes it easy to write apps that enable students to take notes and do research, families to share plans and ideas, or shoppers to share pictures.</span></span> <span data-ttu-id="e977e-113">アプリでは、みんなが必要とする情報を集め、OneNote に送り、それらを整理することができます。</span><span class="sxs-lookup"><span data-stu-id="e977e-113">Your app can grab the information people want, send it to OneNote, and then help them organize it.</span></span>

### <a name="capture-information-in-many-formats"></a><span data-ttu-id="e977e-114">さまざまな形式で情報をキャプチャする</span><span class="sxs-lookup"><span data-stu-id="e977e-114">Capture information in many formats</span></span>

<span data-ttu-id="e977e-115">HTML、埋め込み画像 (ローカルやパブリック URL にある)、ビデオ、オーディオ、メール メッセージ、その他の一般的なファイル タイプをキャプチャします。</span><span class="sxs-lookup"><span data-stu-id="e977e-115">Capture HTML, embed images (sourced locally or at a public URL), video, audio, email messages, and other common file types.</span></span> <span data-ttu-id="e977e-116">OneNote では、Web ページや PDF ファイルをスナップショットとして表示することもできます。</span><span class="sxs-lookup"><span data-stu-id="e977e-116">OneNote can even render webpages and PDF files as snapshots.</span></span> <span data-ttu-id="e977e-117">Microsoft Graph は、OneNote ページ レイアウト用に標準 HTML および CSS のセットをサポートします。そのため、表、インライン イメージ、基本書式を使用して思いどおりの外観を実現できます。</span><span class="sxs-lookup"><span data-stu-id="e977e-117">Microsoft Graph supports a set of standard HTML and CSS for OneNote page layout, so you can use tables, inline images, and basic formatting to get the look you want.</span></span> 

### <a name="use-the-onenote-ecosystem-to-enhance-your-core-scenarios"></a><span data-ttu-id="e977e-118">OneNote エコシステムを使用して、コア シナリオを強化する</span><span class="sxs-lookup"><span data-stu-id="e977e-118">Use the OneNote ecosystem to enhance your core scenarios</span></span>

<span data-ttu-id="e977e-119">その他の強力な OneNote の機能を利用できます。</span><span class="sxs-lookup"><span data-stu-id="e977e-119">Tap into other powerful OneNote features.</span></span> <span data-ttu-id="e977e-120">この Microsoft Graph の OneNote API では、イメージに対する OCR の実行、フルテキスト検索のサポート、クライアントの自動同期、イメージの処理、名刺キャプチャ、オンライン製品一覧やレシピ一覧の抽出などを実行できます。</span><span class="sxs-lookup"><span data-stu-id="e977e-120">The OneNote APIs in Microsoft Graph run OCR on images, support full-text search, auto-syncs clients, process images, and extract business card captures and online product and recipe listings.</span></span> <span data-ttu-id="e977e-121">メモや軽量メディアのクラウドでのデジタル メモリ ストアとして、またはドメイン固有データのデータ フィードとして OneNote を使用します。</span><span class="sxs-lookup"><span data-stu-id="e977e-121">Use OneNote as your digital memory store in the cloud for notes and lightweight media, or as a data feed for domain-specific data.</span></span> 

### <a name="reach-millions-of-onenote-users-on-all-major-platforms"></a><span data-ttu-id="e977e-122">すべての主要プラットフォームの数百万人に上る OneNote ユーザーが利用できる
</span><span class="sxs-lookup"><span data-stu-id="e977e-122">Reach millions of OneNote users on all major platforms</span></span>

<span data-ttu-id="e977e-123">OneNote を使用すると、アプリの使用量が増加します。</span><span class="sxs-lookup"><span data-stu-id="e977e-123">Use OneNote to increase your app usage.</span></span> <span data-ttu-id="e977e-124">OneNote は新しい Windows デバイスにプレインストールされており、ほとんどのプラットフォームでオンライン、および Office 365 の一部として利用可能です。</span><span class="sxs-lookup"><span data-stu-id="e977e-124">OneNote is preinstalled on new Windows devices, and is available for most platforms, online, and as part of Office 365.</span></span> <span data-ttu-id="e977e-125">機能の豊富な OneNote 環境を利用するアプリを公開すると、広範なクロスプラットフォーム市場の潜在的な可能性にアクセスできるようになります。</span><span class="sxs-lookup"><span data-stu-id="e977e-125">When you publish apps that use the feature-rich OneNote environment, you have access to broad cross-platform market potential.</span></span>

<!-- Might be good to show a few examples of Microsoft Graph API calls here, similar to what we have in the featured scenarios topic: featured_scenarios..md You could have an H2 section called "What can I do with OneNote APIs in Microsoft Graph?"-->

## <a name="what-can-i-do-with-onenote-apis-in-microsoft-graph"></a><span data-ttu-id="e977e-126">Microsoft Graph の OneNote API で実行できること</span><span class="sxs-lookup"><span data-stu-id="e977e-126">What can I do with OneNote APIs in Microsoft Graph?</span></span>

<span data-ttu-id="e977e-127">OneNote のリソースの操作で最もよく使用される要求の一部を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e977e-127">The following are some of the most popular requests for working with OneNote resources.</span></span>

|<span data-ttu-id="e977e-128">操作</span><span class="sxs-lookup"><span data-stu-id="e977e-128">Operation</span></span>|<span data-ttu-id="e977e-129">URL</span><span class="sxs-lookup"><span data-stu-id="e977e-129">URL</span></span>|
|:--------|:--|
|<span data-ttu-id="e977e-130">自分のノートブックを取得する</span><span class="sxs-lookup"><span data-stu-id="e977e-130">GET my notebooks</span></span>|[https://graph.microsoft.com/v1.0/me/onenote/notebooks](https://developer.microsoft.com/graph/graph-explorer?request=me/onenote/notebooks&version=1.0)|
|<span data-ttu-id="e977e-131">自分のセクションを取得する</span><span class="sxs-lookup"><span data-stu-id="e977e-131">GET my sections</span></span>|[https://graph.microsoft.com/v1.0/me/onenote/sections](https://developer.microsoft.com/graph/graph-explorer?request=me/onenote/sections&version=1.0)|
|<span data-ttu-id="e977e-132">自分のページを取得する</span><span class="sxs-lookup"><span data-stu-id="e977e-132">GET my pages</span></span>|[https://graph.microsoft.com/v1.0/me/onenote/pages](https://developer.microsoft.com/graph/graph-explorer?request=me/onenote/pages&version=1.0)|

## <a name="learn-more-about-onenote-apis"></a><span data-ttu-id="e977e-133">OneNote API に関する詳細情報</span><span class="sxs-lookup"><span data-stu-id="e977e-133">Learn more about OneNote APIs</span></span>

<span data-ttu-id="e977e-134">OneNote のコンテンツ更新機能については、Microsoft Graph API の詳細情報をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="e977e-134">Take an in-depth look at Microsoft Graph APIs to learn about the OneNote content updating capabilities.</span></span> <span data-ttu-id="e977e-135">次の一覧の各トピックは、新しい OneNote ページを作成し、既存のページを新しいコンテンツで更新する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="e977e-135">The topics in the following list show you how to create new OneNote pages and update existing pages with new content.</span></span> <span data-ttu-id="e977e-136">Microsoft Graph を使用した OneNote ノートブックの更新に関するベスト プラクティスも参照してください。</span><span class="sxs-lookup"><span data-stu-id="e977e-136">You'll also learn about best practices in using Microsoft Graph to update OneNote notebooks.</span></span> 


### <a name="work-with-onenote"></a><span data-ttu-id="e977e-137">OneNote での作業</span><span class="sxs-lookup"><span data-stu-id="e977e-137">Work with OneNote</span></span>

* [<span data-ttu-id="e977e-138">OneNote REST API を使用する</span><span class="sxs-lookup"><span data-stu-id="e977e-138">Use the OneNote REST API</span></span>](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0)
* [<span data-ttu-id="e977e-139">ベスト プラクティス</span><span class="sxs-lookup"><span data-stu-id="e977e-139">Best practices</span></span>](onenote-best-practices.md)
* [<span data-ttu-id="e977e-140">ブランドのガイドライン</span><span class="sxs-lookup"><span data-stu-id="e977e-140">Branding guidelines</span></span>](onenote-branding.md)
* [<span data-ttu-id="e977e-141">OneNote クライアントを開く</span><span class="sxs-lookup"><span data-stu-id="e977e-141">Open the OneNote client</span></span>](open-onenote-client.md)
* [<span data-ttu-id="e977e-142">OneNote ページでノート シールを使用する</span><span class="sxs-lookup"><span data-stu-id="e977e-142">Use note tags in OneNote pages</span></span>](onenote-note-tags.md)
* [<span data-ttu-id="e977e-143">Microsoft Graph の OneNote API のエラー コード</span><span class="sxs-lookup"><span data-stu-id="e977e-143">Error codes for OneNote APIs in Microsoft Graph</span></span>](onenote-error-codes.md)

### <a name="work-with-onenote-pages"></a><span data-ttu-id="e977e-144">OneNote ページでの作業</span><span class="sxs-lookup"><span data-stu-id="e977e-144">Work with OneNote pages</span></span>

* [<span data-ttu-id="e977e-145">OneNote ページの入出力 HTML</span><span class="sxs-lookup"><span data-stu-id="e977e-145">Input and output HTML in OneNote pages</span></span>](onenote-input-output-html.md)
* [<span data-ttu-id="e977e-146">Microsoft Graph によって OneNote コンテンツと構造を取得する</span><span class="sxs-lookup"><span data-stu-id="e977e-146">Get OneNote content and structure with Microsoft Graph</span></span>](onenote-get-content.md)
* [<span data-ttu-id="e977e-147">OneNote ページを作成する</span><span class="sxs-lookup"><span data-stu-id="e977e-147">Create OneNote pages</span></span>](onenote-create-page.md)
* [<span data-ttu-id="e977e-148">OneNote ページ コンテンツを更新する</span><span class="sxs-lookup"><span data-stu-id="e977e-148">Update OneNote page content</span></span>](onenote-update-page.md)

### <a name="work-with-onenote-page-content"></a><span data-ttu-id="e977e-149">OneNote ページ コンテンツを使用する</span><span class="sxs-lookup"><span data-stu-id="e977e-149">Work with OneNote page content</span></span>

* [<span data-ttu-id="e977e-150">OneNote ページで絶対配置要素を作成する</span><span class="sxs-lookup"><span data-stu-id="e977e-150">Create absolute positioned elements in OneNote pages</span></span>](onenote-abs-pos.md)
* [<span data-ttu-id="e977e-151">OneNote ページに画像、ビデオ、ファイルを追加する</span><span class="sxs-lookup"><span data-stu-id="e977e-151">Add images, videos, and files to OneNote pages</span></span>](onenote-images-files.md)
* [<span data-ttu-id="e977e-152">OneNote API div タグを使用してキャプチャからデータを抽出する</span><span class="sxs-lookup"><span data-stu-id="e977e-152">Use OneNote API div tags to extract data from captures</span></span>](onenote-extract-data.md)

## <a name="see-also"></a><span data-ttu-id="e977e-153">関連項目</span><span class="sxs-lookup"><span data-stu-id="e977e-153">See also</span></span>
<span data-ttu-id="e977e-154">OneNote サービス固有の REST エンドポイントにのみ公開されている、OneNote その他の機能の一部について説明します。</span><span class="sxs-lookup"><span data-stu-id="e977e-154">Find out about a few other OneNote features that are exposed only on the OneNote service-specific REST endpoint.</span></span>

- <span data-ttu-id="e977e-155">
  [OneNote の開発](https://docs.microsoft.com/ja-JP/previous-versions/office/office-365-api/how-to/onenote-landing)</span><span class="sxs-lookup"><span data-stu-id="e977e-155">[OneNote development](https://docs.microsoft.com/en-us/previous-versions/office/office-365-api/how-to/onenote-landing)</span></span>
- <span data-ttu-id="e977e-156">
  [クラス ノートブックの操作](https://docs.microsoft.com/ja-JP/previous-versions/office/office-365-api/how-to/onenote-classnotebook)</span><span class="sxs-lookup"><span data-stu-id="e977e-156">[Work with class notebooks](https://docs.microsoft.com/en-us/previous-versions/office/office-365-api/how-to/onenote-classnotebook)</span></span>
- <span data-ttu-id="e977e-157">
  [非同期クラス ノートブックの操作](https://docs.microsoft.com/ja-JP/previous-versions/office/office-365-api/how-to/onenote-classnotebook-asynchronous)</span><span class="sxs-lookup"><span data-stu-id="e977e-157">[Work with asynchronous class notebooks](https://docs.microsoft.com/en-us/previous-versions/office/office-365-api/how-to/onenote-classnotebook-asynchronous)</span></span>
- <span data-ttu-id="e977e-158">
  [スタッフ ノートブックの操作](https://docs.microsoft.com/ja-JP/previous-versions/office/office-365-api/how-to/onenote-staffnotebook)</span><span class="sxs-lookup"><span data-stu-id="e977e-158">[Work with staff notebooks](https://docs.microsoft.com/en-us/previous-versions/office/office-365-api/how-to/onenote-staffnotebook)</span></span>
- <span data-ttu-id="e977e-159">
  [ノートブック、セクション、ページのコピー](https://docs.microsoft.com/ja-JP/previous-versions/office/office-365-api/how-to/onenote-copy)</span><span class="sxs-lookup"><span data-stu-id="e977e-159">[Copy notebooks, sections, and pages](https://docs.microsoft.com/en-us/previous-versions/office/office-365-api/how-to/onenote-copy)</span></span>
- <span data-ttu-id="e977e-160">
  [OneNote エンティティのアクセス許可を管理する](https://docs.microsoft.com/ja-JP/previous-versions/office/office-365-api/how-to/onenote-manage-perms)</span><span class="sxs-lookup"><span data-stu-id="e977e-160">[Manage permissions on OneNote entities](https://docs.microsoft.com/en-us/previous-versions/office/office-365-api/how-to/onenote-manage-perms)</span></span>
- <span data-ttu-id="e977e-161">
  [Web ページで OneNote 保存ダイアログを使用する](https://docs.microsoft.com/ja-JP/previous-versions/office/office-365-api/how-to/onenote-save-dialog)</span><span class="sxs-lookup"><span data-stu-id="e977e-161">[Use the OneNote save dialog on your webpages](https://docs.microsoft.com/en-us/previous-versions/office/office-365-api/how-to/onenote-save-dialog)</span></span>
- <span data-ttu-id="e977e-162">
  [Webhooks の購読](https://docs.microsoft.com/ja-JP/previous-versions/office/office-365-api/how-to/onenote-sync)</span><span class="sxs-lookup"><span data-stu-id="e977e-162">[Subscribe to webhooks](https://docs.microsoft.com/en-us/previous-versions/office/office-365-api/how-to/onenote-sync)</span></span>

## <a name="api-reference"></a><span data-ttu-id="e977e-163">API リファレンス</span><span class="sxs-lookup"><span data-stu-id="e977e-163">API reference</span></span>
<span data-ttu-id="e977e-164">このサービスの API リファレンスをお探しですか?</span><span class="sxs-lookup"><span data-stu-id="e977e-164">Looking for the API reference for this service?</span></span>

- [<span data-ttu-id="e977e-165">Microsoft Graph v1.0 の OneNote API</span><span class="sxs-lookup"><span data-stu-id="e977e-165">OneNote API in Microsoft Graph v1.0</span></span>](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0)
- [<span data-ttu-id="e977e-166">Microsoft Graph ベータ版の OneNote API</span><span class="sxs-lookup"><span data-stu-id="e977e-166">OneNote API in Microsoft Graph beta</span></span>](/graph/api/resources/onenote-api-overview?view=graph-rest-beta)

## <a name="next-steps"></a><span data-ttu-id="e977e-167">次のステップ</span><span class="sxs-lookup"><span data-stu-id="e977e-167">Next steps</span></span>

<span data-ttu-id="e977e-168">[Microsoft Graph Explorer](https://developer.microsoft.com/graph/graph-explorer) を使用して、自分の OneNote ノートブックで OneNote API を試してみます。</span><span class="sxs-lookup"><span data-stu-id="e977e-168">Use the [Microsoft Graph Explorer](https://developer.microsoft.com/graph/graph-explorer) to try out the OneNote APIs with your own OneNote notebooks.</span></span>

<span data-ttu-id="e977e-169">Graph Explorer から OneNote API 呼び出しを行うには、左側の列にある **[その他のサンプルを表示]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="e977e-169">To make OneNote API calls from the Graph Explorer, choose **Show more samples** in the column on the left.</span></span> <span data-ttu-id="e977e-170">メニューを使用して、OneNote を **[オン]** に切り替えます。</span><span class="sxs-lookup"><span data-stu-id="e977e-170">Use the menu to toggle OneNote **On**.</span></span> <span data-ttu-id="e977e-171">また、適切なアクセス許可を有効にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="e977e-171">You will also need to enable the appropriate permissions.</span></span> <span data-ttu-id="e977e-172">左側のメニューのアカウント名の下で、**[アクセス許可の修正]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="e977e-172">Under your account name in the menu on the left, choose **modify permissions**.</span></span> <span data-ttu-id="e977e-173">OneNote のアクセス許可の詳細については、「[メモのアクセス許可](permissions-reference.md#notes-permissions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e977e-173">For more information about OneNote permissions, see [Notes permissions](permissions-reference.md#notes-permissions).</span></span>

<span data-ttu-id="e977e-174">Microsoft Graph の OneNote API を使い始めるには、[OneNote 参照コンテンツ](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0)に関する記事をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="e977e-174">To get started with OneNote APIs in Microsoft Graph, see the [OneNote reference content](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0).</span></span>

