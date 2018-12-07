---
title: OneNote API の概要
description: OneNote は、顧客が Web、電話、タブレット、またはデスクトップ上で文字、スケッチ、音声を入力することで、家庭、学校、または職場用のアイデアやメモを追跡できるデジタル ノートブックです。 自由にメモを整理し、デバイスを切り替えて作業の中断箇所から再開し、他のユーザーとリアルタイムでメモの共同作業を行えます。
ms.openlocfilehash: 9f0c82c8cdc4e336a1ee9d604b13e7e5b5bc0282
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092478"
---
# <a name="onenote-api-overview"></a><span data-ttu-id="fef49-104">OneNote API の概要</span><span class="sxs-lookup"><span data-stu-id="fef49-104">OneNote API overview</span></span>

<span data-ttu-id="fef49-105">OneNote は、顧客が Web、電話、タブレット、またはデスクトップ上で文字、スケッチ、音声を入力することで、家庭、学校、または職場用のアイデアやメモを追跡できるデジタル ノートブックです。</span><span class="sxs-lookup"><span data-stu-id="fef49-105">OneNote is a digital notebook that lets customers track ideas and notes for home, school, or work, by typing, sketching, or voice, on the web, phone, tablet, or desktop.</span></span> <span data-ttu-id="fef49-106">自由にメモを整理し、デバイスを切り替えて作業の中断箇所から再開し、他のユーザーとリアルタイムでメモの共同作業を行えます。</span><span class="sxs-lookup"><span data-stu-id="fef49-106">They can freely organize notes, switch devices and pick up where they left off, and collaborate on notes with others in real time.</span></span>

![OneNote ノートブックとセクションとページ](images/onenote-page.png)

## <a name="why-integrate-with-onenote"></a><span data-ttu-id="fef49-108">OneNote と統合する理由</span><span class="sxs-lookup"><span data-stu-id="fef49-108">Why integrate with OneNote?</span></span>

<span data-ttu-id="fef49-109">アプリを OneNote に統合すると、複数のプラットフォームで利用できる便利な機能を作成し、世界中の数百万人のユーザーに届けることができます。</span><span class="sxs-lookup"><span data-stu-id="fef49-109">By integrating your apps with OneNote, you can create empowering experiences across multiple platforms that reach millions of users worldwide.</span></span> <span data-ttu-id="fef49-110">Microsoft Graph を使用して OneNote のノートブック、セクション、ページにアクセスし、ユーザーによるアイデアや情報の計画や整理を支援するソリューションを作成することができます。</span><span class="sxs-lookup"><span data-stu-id="fef49-110">You can use Microsoft Graph to access notebooks, sections, and pages in OneNote to create solutions that help your users plan and organize ideas and information.</span></span>

### <a name="collect-and-organize-notes-and-ideas"></a><span data-ttu-id="fef49-111">メモやアイデアを収集して整理する</span><span class="sxs-lookup"><span data-stu-id="fef49-111">Collect and organize notes and ideas</span></span>  

<span data-ttu-id="fef49-112">コンテンツを追加したり、アレンジしたりできるキャンバスとして OneNote を使用します。</span><span class="sxs-lookup"><span data-stu-id="fef49-112">Use OneNote as a canvas where users can add and arrange their content.</span></span> <span data-ttu-id="fef49-113">Microsoft Graph を使用すると、学生がメモを取って調査すること、家族が計画とアイデアを共有すること、買い物客が画像を共有することを可能にするアプリを簡単に作成できます。</span><span class="sxs-lookup"><span data-stu-id="fef49-113">Microsoft Graph makes it easy to write apps that enable students to take notes and do research, families to share plans and ideas, or shoppers to share pictures.</span></span> <span data-ttu-id="fef49-114">アプリでは、みんなが必要とする情報を集め、OneNote に送り、それらを整理することができます。</span><span class="sxs-lookup"><span data-stu-id="fef49-114">Your app can grab the information people want, send it to OneNote, and then help them organize it.</span></span>

### <a name="capture-information-in-many-formats"></a><span data-ttu-id="fef49-115">さまざまな形式で情報をキャプチャする</span><span class="sxs-lookup"><span data-stu-id="fef49-115">Capture information in many formats</span></span>

<span data-ttu-id="fef49-116">HTML、埋め込み画像 (ローカルやパブリック URL にある)、ビデオ、オーディオ、メール メッセージ、その他の一般的なファイル タイプをキャプチャします。</span><span class="sxs-lookup"><span data-stu-id="fef49-116">Capture HTML, embed images (sourced locally or at a public URL), video, audio, email messages, and other common file types.</span></span> <span data-ttu-id="fef49-117">OneNote では、Web ページや PDF ファイルをスナップショットとして表示することもできます。</span><span class="sxs-lookup"><span data-stu-id="fef49-117">OneNote can even render webpages and PDF files as snapshots.</span></span> <span data-ttu-id="fef49-118">Microsoft Graph は、OneNote ページ レイアウト用に標準 HTML および CSS のセットをサポートします。そのため、表、インライン イメージ、基本書式を使用して思いどおりの外観を実現できます。</span><span class="sxs-lookup"><span data-stu-id="fef49-118">Microsoft Graph supports a set of standard HTML and CSS for OneNote page layout, so you can use tables, inline images, and basic formatting to get the look you want.</span></span> 

### <a name="use-the-onenote-ecosystem-to-enhance-your-core-scenarios"></a><span data-ttu-id="fef49-119">OneNote エコシステムを使用して、コア シナリオを強化する</span><span class="sxs-lookup"><span data-stu-id="fef49-119">Use the OneNote ecosystem to enhance your core scenarios</span></span>

<span data-ttu-id="fef49-120">その他の強力な OneNote の機能を利用できます。</span><span class="sxs-lookup"><span data-stu-id="fef49-120">Tap into other powerful OneNote features.</span></span> <span data-ttu-id="fef49-121">この Microsoft Graph の OneNote API では、イメージに対する OCR の実行、フルテキスト検索のサポート、クライアントの自動同期、イメージの処理、名刺キャプチャ、オンライン製品一覧やレシピ一覧の抽出などを実行できます。</span><span class="sxs-lookup"><span data-stu-id="fef49-121">The OneNote APIs in Microsoft Graph run OCR on images, support full-text search, auto-syncs clients, process images, and extract business card captures and online product and recipe listings.</span></span> <span data-ttu-id="fef49-122">メモや軽量メディアのクラウドでのデジタル メモリ ストアとして、またはドメイン固有データのデータ フィードとして OneNote を使用します。</span><span class="sxs-lookup"><span data-stu-id="fef49-122">Use OneNote as your digital memory store in the cloud for notes and lightweight media, or as a data feed for domain-specific data.</span></span> 

### <a name="reach-millions-of-onenote-users-on-all-major-platforms"></a><span data-ttu-id="fef49-123">すべての主要プラットフォームの数百万人に上る OneNote ユーザーが利用できる
</span><span class="sxs-lookup"><span data-stu-id="fef49-123">Reach millions of OneNote users on all major platforms</span></span>

<span data-ttu-id="fef49-124">OneNote を使用すると、アプリの使用量が増加します。</span><span class="sxs-lookup"><span data-stu-id="fef49-124">Use OneNote to increase your app usage.</span></span> <span data-ttu-id="fef49-125">OneNote は新しい Windows デバイスにプレインストールされており、ほとんどのプラットフォームでオンライン、および Office 365 の一部として利用可能です。</span><span class="sxs-lookup"><span data-stu-id="fef49-125">OneNote is preinstalled on new Windows devices, and is available for most platforms, online, and as part of Office 365.</span></span> <span data-ttu-id="fef49-126">機能の豊富な OneNote 環境を利用するアプリを公開すると、広範なクロスプラットフォーム市場の潜在的な可能性にアクセスできるようになります。</span><span class="sxs-lookup"><span data-stu-id="fef49-126">When you publish apps that use the feature-rich OneNote environment, you have access to broad cross-platform market potential.</span></span>

<!-- Might be good to show a few examples of Microsoft Graph API calls here, similar to what we have in the featured scenarios topic: featured_scenarios..md You could have an H2 section called "What can I do with OneNote APIs in Microsoft Graph?"-->

## <a name="what-can-i-do-with-onenote-apis-in-microsoft-graph"></a><span data-ttu-id="fef49-127">Microsoft Graph の OneNote API で実行できること</span><span class="sxs-lookup"><span data-stu-id="fef49-127">What can I do with OneNote APIs in Microsoft Graph?</span></span>

<span data-ttu-id="fef49-128">OneNote のリソースの操作で最もよく使用される要求の一部を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fef49-128">The following are some of the most popular requests for working with OneNote resources.</span></span>

|<span data-ttu-id="fef49-129">操作</span><span class="sxs-lookup"><span data-stu-id="fef49-129">Operation</span></span>|<span data-ttu-id="fef49-130">URL</span><span class="sxs-lookup"><span data-stu-id="fef49-130">URL</span></span>|
|:--------|:--|
|<span data-ttu-id="fef49-131">自分のノートブックを取得する</span><span class="sxs-lookup"><span data-stu-id="fef49-131">GET my notebooks</span></span>|[https://graph.microsoft.com/v1.0/me/onenote/notebooks](https://developer.microsoft.com/graph/graph-explorer?request=me/onenote/notebooks&version=1.0)|
|<span data-ttu-id="fef49-132">自分のセクションを取得する</span><span class="sxs-lookup"><span data-stu-id="fef49-132">GET my sections</span></span>|[https://graph.microsoft.com/v1.0/me/onenote/sections](https://developer.microsoft.com/graph/graph-explorer?request=me/onenote/sections&version=1.0)|
|<span data-ttu-id="fef49-133">自分のページを取得する</span><span class="sxs-lookup"><span data-stu-id="fef49-133">GET my pages</span></span>|[https://graph.microsoft.com/v1.0/me/onenote/pages](https://developer.microsoft.com/graph/graph-explorer?request=me/onenote/pages&version=1.0)|

## <a name="learn-more-about-onenote-apis"></a><span data-ttu-id="fef49-134">OneNote API に関する詳細情報</span><span class="sxs-lookup"><span data-stu-id="fef49-134">Learn more about OneNote APIs</span></span>

<span data-ttu-id="fef49-135">OneNote のコンテンツ更新機能については、Microsoft Graph API の詳細情報をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="fef49-135">Take an in-depth look at Microsoft Graph APIs to learn about the OneNote content updating capabilities.</span></span> <span data-ttu-id="fef49-136">次の一覧の各トピックは、新しい OneNote ページを作成し、既存のページを新しいコンテンツで更新する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="fef49-136">The topics in the following list show you how to create new OneNote pages and update existing pages with new content.</span></span> <span data-ttu-id="fef49-137">Microsoft Graph を使用した OneNote ノートブックの更新に関するベスト プラクティスも参照してください。</span><span class="sxs-lookup"><span data-stu-id="fef49-137">You'll also learn about best practices in using Microsoft Graph to update OneNote notebooks.</span></span> 


### <a name="work-with-onenote"></a><span data-ttu-id="fef49-138">OneNote での作業</span><span class="sxs-lookup"><span data-stu-id="fef49-138">Work with OneNote</span></span>

* [<span data-ttu-id="fef49-139">OneNote REST API を使用する</span><span class="sxs-lookup"><span data-stu-id="fef49-139">Use the OneNote REST API</span></span>](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0)
* [<span data-ttu-id="fef49-140">ベスト プラクティス</span><span class="sxs-lookup"><span data-stu-id="fef49-140">Best practices</span></span>](onenote-best-practices.md)
* [<span data-ttu-id="fef49-141">ブランドのガイドライン</span><span class="sxs-lookup"><span data-stu-id="fef49-141">Branding guidelines</span></span>](onenote-branding.md)
* [<span data-ttu-id="fef49-142">OneNote クライアントを開く</span><span class="sxs-lookup"><span data-stu-id="fef49-142">Open the OneNote client</span></span>](open-onenote-client.md)
* [<span data-ttu-id="fef49-143">OneNote ページでノート シールを使用する</span><span class="sxs-lookup"><span data-stu-id="fef49-143">Use note tags in OneNote pages</span></span>](onenote-note-tags.md)
* [<span data-ttu-id="fef49-144">Microsoft Graph の OneNote API のエラー コード</span><span class="sxs-lookup"><span data-stu-id="fef49-144">Error codes for OneNote APIs in Microsoft Graph</span></span>](onenote-error-codes.md)

### <a name="work-with-onenote-pages"></a><span data-ttu-id="fef49-145">OneNote ページでの作業</span><span class="sxs-lookup"><span data-stu-id="fef49-145">Work with OneNote pages</span></span>

* [<span data-ttu-id="fef49-146">OneNote ページの入出力 HTML</span><span class="sxs-lookup"><span data-stu-id="fef49-146">Input and output HTML in OneNote pages</span></span>](onenote-input-output-html.md)
* [<span data-ttu-id="fef49-147">Microsoft Graph によって OneNote コンテンツと構造を取得する</span><span class="sxs-lookup"><span data-stu-id="fef49-147">Get OneNote content and structure with Microsoft Graph</span></span>](onenote-get-content.md)
* [<span data-ttu-id="fef49-148">OneNote ページを作成する</span><span class="sxs-lookup"><span data-stu-id="fef49-148">Create OneNote pages</span></span>](onenote-create-page.md)
* [<span data-ttu-id="fef49-149">OneNote ページ コンテンツを更新する</span><span class="sxs-lookup"><span data-stu-id="fef49-149">Update OneNote page content</span></span>](onenote-update-page.md)

### <a name="work-with-onenote-page-content"></a><span data-ttu-id="fef49-150">OneNote ページ コンテンツを使用する</span><span class="sxs-lookup"><span data-stu-id="fef49-150">Work with OneNote page content</span></span>

* [<span data-ttu-id="fef49-151">OneNote ページで絶対配置要素を作成する</span><span class="sxs-lookup"><span data-stu-id="fef49-151">Create absolute positioned elements in OneNote pages</span></span>](onenote-abs-pos.md)
* [<span data-ttu-id="fef49-152">OneNote ページに画像、ビデオ、ファイルを追加する</span><span class="sxs-lookup"><span data-stu-id="fef49-152">Add images, videos, and files to OneNote pages</span></span>](onenote-images-files.md)
* [<span data-ttu-id="fef49-153">OneNote API div タグを使用してキャプチャからデータを抽出する</span><span class="sxs-lookup"><span data-stu-id="fef49-153">Use OneNote API div tags to extract data from captures</span></span>](onenote-extract-data.md)

## <a name="see-also"></a><span data-ttu-id="fef49-154">関連項目</span><span class="sxs-lookup"><span data-stu-id="fef49-154">See also</span></span>
<span data-ttu-id="fef49-155">OneNote サービス固有の REST エンドポイントにのみ公開されている、OneNote その他の機能の一部について説明します。</span><span class="sxs-lookup"><span data-stu-id="fef49-155">Find out about a few other OneNote features that are exposed only on the OneNote service-specific REST endpoint.</span></span>

- [<span data-ttu-id="fef49-156">OneNote の開発</span><span class="sxs-lookup"><span data-stu-id="fef49-156">OneNote development</span></span>](https://docs.microsoft.com/ja-JP/previous-versions/office/office-365-api/how-to/onenote-landing)
- [<span data-ttu-id="fef49-157">クラス ノートブックの操作</span><span class="sxs-lookup"><span data-stu-id="fef49-157">Work with class notebooks</span></span>](https://docs.microsoft.com/ja-JP/previous-versions/office/office-365-api/how-to/onenote-classnotebook)
- [<span data-ttu-id="fef49-158">非同期クラス ノートブックの操作</span><span class="sxs-lookup"><span data-stu-id="fef49-158">Work with asynchronous class notebooks</span></span>](https://docs.microsoft.com/ja-JP/previous-versions/office/office-365-api/how-to/onenote-classnotebook-asynchronous)
- [<span data-ttu-id="fef49-159">スタッフ ノートブックの操作</span><span class="sxs-lookup"><span data-stu-id="fef49-159">Work with staff notebooks</span></span>](https://docs.microsoft.com/ja-JP/previous-versions/office/office-365-api/how-to/onenote-staffnotebook)
- [<span data-ttu-id="fef49-160">ノートブック、セクション、ページのコピー</span><span class="sxs-lookup"><span data-stu-id="fef49-160">Copy notebooks, sections, and pages</span></span>](https://docs.microsoft.com/ja-JP/previous-versions/office/office-365-api/how-to/onenote-copy)
- [<span data-ttu-id="fef49-161">OneNote エンティティのアクセス許可を管理する</span><span class="sxs-lookup"><span data-stu-id="fef49-161">Manage permissions on OneNote entities</span></span>](https://docs.microsoft.com/ja-JP/previous-versions/office/office-365-api/how-to/onenote-manage-perms)
- [<span data-ttu-id="fef49-162">Web ページで OneNote 保存ダイアログを使用する</span><span class="sxs-lookup"><span data-stu-id="fef49-162">Use the OneNote save dialog on your webpages</span></span>](https://docs.microsoft.com/ja-JP/previous-versions/office/office-365-api/how-to/onenote-save-dialog)
- [<span data-ttu-id="fef49-163">Webhooks の購読</span><span class="sxs-lookup"><span data-stu-id="fef49-163">Subscribe to webhooks</span></span>](https://docs.microsoft.com/ja-JP/previous-versions/office/office-365-api/how-to/onenote-sync)

## <a name="api-reference"></a><span data-ttu-id="fef49-164">API リファレンス</span><span class="sxs-lookup"><span data-stu-id="fef49-164">API reference</span></span>
<span data-ttu-id="fef49-165">このサービスの API リファレンスをお探しですか?</span><span class="sxs-lookup"><span data-stu-id="fef49-165">Looking for the API reference for this service?</span></span>

- [<span data-ttu-id="fef49-166">Microsoft Graph v1.0 の OneNote API</span><span class="sxs-lookup"><span data-stu-id="fef49-166">OneNote API in Microsoft Graph v1.0</span></span>](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0)
- [<span data-ttu-id="fef49-167">Microsoft Graph ベータ版の OneNote API</span><span class="sxs-lookup"><span data-stu-id="fef49-167">OneNote API in Microsoft Graph beta</span></span>](/graph/api/resources/onenote-api-overview?view=graph-rest-beta)

## <a name="next-steps"></a><span data-ttu-id="fef49-168">次のステップ</span><span class="sxs-lookup"><span data-stu-id="fef49-168">Next steps</span></span>

<span data-ttu-id="fef49-169">[Microsoft Graph Explorer](https://developer.microsoft.com/graph/graph-explorer) を使用して、自分の OneNote ノートブックで OneNote API を試してみます。</span><span class="sxs-lookup"><span data-stu-id="fef49-169">Use the [Microsoft Graph Explorer](https://developer.microsoft.com/graph/graph-explorer) to try out the OneNote APIs with your own OneNote notebooks.</span></span>

<span data-ttu-id="fef49-170">Graph Explorer から OneNote API 呼び出しを行うには、左側の列にある **[その他のサンプルを表示]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="fef49-170">To make OneNote API calls from the Graph Explorer, choose **Show more samples** in the column on the left.</span></span> <span data-ttu-id="fef49-171">メニューを使用して、OneNote を **[オン]** に切り替えます。</span><span class="sxs-lookup"><span data-stu-id="fef49-171">Use the menu to toggle OneNote **On**.</span></span> <span data-ttu-id="fef49-172">また、適切なアクセス許可を有効にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="fef49-172">You will also need to enable the appropriate permissions.</span></span> <span data-ttu-id="fef49-173">左側のメニューのアカウント名の下で、**[アクセス許可の修正]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="fef49-173">Under your account name in the menu on the left, choose **modify permissions**.</span></span> <span data-ttu-id="fef49-174">OneNote のアクセス許可の詳細については、「[メモのアクセス許可](permissions-reference.md#notes-permissions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fef49-174">For more information about OneNote permissions, see [Notes permissions](permissions-reference.md#notes-permissions).</span></span>

<span data-ttu-id="fef49-175">Microsoft Graph の OneNote API を使い始めるには、[OneNote 参照コンテンツ](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0)に関する記事をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="fef49-175">To get started with OneNote APIs in Microsoft Graph, see the [OneNote reference content](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0).</span></span>

