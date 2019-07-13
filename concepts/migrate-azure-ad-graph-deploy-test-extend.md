---
title: 移行したアプリの展開、テスト、拡張
description: 'Microsoft Graph API (REST) を使用するように Azure Active Directory (Azure AD) アプリを移行する方法について説明します。ここでは、手順 3: 展開、テスト、拡張について説明します。'
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6b5236f6b7be140e1040a3169edded6e162b5e7a
ms.sourcegitcommit: ca55fc5f5711966eaa41da31cd1ae99820e9e586
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/13/2019
ms.locfileid: "35645255"
---
# <a name="deploy-test-and-extend"></a><span data-ttu-id="67dca-103">展開、テスト、拡張</span><span class="sxs-lookup"><span data-stu-id="67dca-103">Deploy, test, and extend</span></span>

<span data-ttu-id="67dca-104">これは、[アプリを移行するプロセス](migrate-azure-ad-graph-planning-checklist.md)の手順4です。</span><span class="sxs-lookup"><span data-stu-id="67dca-104">This is step 4 of the [process to migrate apps](migrate-azure-ad-graph-planning-checklist.md).</span></span>

1.  <span data-ttu-id="67dca-105">**テスト方法**</span><span class="sxs-lookup"><span data-stu-id="67dca-105">**Test throughly**</span></span>

    <span data-ttu-id="67dca-106">アプリを更新したら、十分にテストして、予期したとおりに動作することと、回帰がまったく導入されていないことを確認してください。</span><span class="sxs-lookup"><span data-stu-id="67dca-106">Once you've updated your app, test it thoroughly to verify that it works as expected and that you haven't introduced any regressions.</span></span>  

    <span data-ttu-id="67dca-107">複数の環境、データセット、およびエンドユーザーのペルソナ (たとえば、異なる役割、権利、および責任を持つ資格情報) を使用していることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="67dca-107">Be sure to use multiple environments, data sets, and end-user personas, e.g. credentials with different roles, rights, and responsibilities.</span></span> <span data-ttu-id="67dca-108">新しいテストユーザーが初めてアプリを取得し、既存のユーザー (既に同意しているユーザー) がアプリを再度使用しようとしたときに、ライフサイクル全体を参照します。</span><span class="sxs-lookup"><span data-stu-id="67dca-108">Go through the entire lifecycle, by having a new test user acquire the app for the first time, as well as an existing user (who already consented) trying to use the app again.</span></span>

2.  <span data-ttu-id="67dca-109">**段階的な更新プログラムを展開する**</span><span class="sxs-lookup"><span data-stu-id="67dca-109">**Deploy staged updates**</span></span>

    <span data-ttu-id="67dca-110">更新プログラムを段階的に展開することを検討してください。</span><span class="sxs-lookup"><span data-stu-id="67dca-110">Consider deploying your updates in stages.</span></span>  <span data-ttu-id="67dca-111">少数のフレンドリユーザーに限定されたロールアウトは、やっかいの問題やその他の潜在的な問題を特定するのに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="67dca-111">A limited roll-out to a small set of friendly users can help identify glitches and other potentially-embarrassing issues.</span></span>  <span data-ttu-id="67dca-112">これにより、初期の受信やフィードバックを監視することもできます。</span><span class="sxs-lookup"><span data-stu-id="67dca-112">This also gives you a chance to monitor initial reception and feedback.</span></span>

    <span data-ttu-id="67dca-113">初期ロールアウトがうまくいく場合は、より多くのユーザーに展開するときの進行状況を監視します。</span><span class="sxs-lookup"><span data-stu-id="67dca-113">If the initial roll-out goes well, monitor progress as you deploy to larger audiences.</span></span>

3.  <span data-ttu-id="67dca-114">**新しい値を探す**</span><span class="sxs-lookup"><span data-stu-id="67dca-114">**Explore new value**</span></span>

    <span data-ttu-id="67dca-115">Microsoft Graph への切り替えが完了したので、すぐに使用できるようになるデータセットや機能の多くは、すぐにロック解除することができなくなりました。</span><span class="sxs-lookup"><span data-stu-id="67dca-115">Now you've made the switch to Microsoft Graph, it's never been easier for you to unlock many more datasets and features that are now at your fingertips.</span></span> <span data-ttu-id="67dca-116">定期的に新しいデータセットと機能をチェックします。</span><span class="sxs-lookup"><span data-stu-id="67dca-116">Check for new datasets and capabilities regularly.</span></span>  

    - <span data-ttu-id="67dca-117">[Microsoft Graph で可能なこと](/graph/examples)を確認する</span><span class="sxs-lookup"><span data-stu-id="67dca-117">Take a look at [what you can do with Microsoft Graph](/graph/examples)</span></span>
    - <span data-ttu-id="67dca-118">Microsoft graph に関する最新ニュース、およびいくつかの豊富な学習シリーズについては、 [Microsoft graph のブログ](/graph/blogs)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="67dca-118">Explore the [Microsoft Graph blog](/graph/blogs) for the latest news about Microsoft Graph and some great learning series.</span></span>
    - <span data-ttu-id="67dca-119">[Changelog](/greaph/changelog)は、サービスおよびドキュメントの更新を要約します。</span><span class="sxs-lookup"><span data-stu-id="67dca-119">The [changelog](/greaph/changelog) summarizes service and document updates.</span></span> <span data-ttu-id="67dca-120">これらの更新プログラムをフォローすると、ベータ版 (プレビュー) と v2.0 (GA) に昇格した新しい Api を追跡するのに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="67dca-120">Following these updates will help you track new APIs introduced to /beta (preview) and those promoted to v1.0 (GA).</span></span>  <span data-ttu-id="67dca-121">これらの新しい Api は、より多くの価値と新しいエクスペリエンスをアプリに追加するための新しい方法を提供します。</span><span class="sxs-lookup"><span data-stu-id="67dca-121">These new APIs can provide new ways for you to add more value and new experiences to your apps.</span></span>  

## <a name="see-also"></a><span data-ttu-id="67dca-122">関連項目</span><span class="sxs-lookup"><span data-stu-id="67dca-122">See also</span></span>

<span data-ttu-id="67dca-123">移行プロセスで問題が発生したり、ヘルプが必要になった場合は、次の操作を実行できます。</span><span class="sxs-lookup"><span data-stu-id="67dca-123">If you run into problems or need help during the migration process, you can:</span></span>

- <span data-ttu-id="67dca-124">[チェックリスト](migrate-azure-ad-graph-overview.md)をもう一度確認する</span><span class="sxs-lookup"><span data-stu-id="67dca-124">Review the [checklist](migrate-azure-ad-graph-overview.md) again</span></span>
- <span data-ttu-id="67dca-125">[Stackoverflow](https://stackoverflow.com/questions/tagged/microsoft-graph)に質問を投稿する</span><span class="sxs-lookup"><span data-stu-id="67dca-125">Post questions to [StackOverflow](https://stackoverflow.com/questions/tagged/microsoft-graph)</span></span>
- <span data-ttu-id="67dca-126">Microsoft Graph サンプルを見直して、既存のアプリケーションコードと比較します。</span><span class="sxs-lookup"><span data-stu-id="67dca-126">Review Microsoft Graph samples to contrast and compare with your existing application code:</span></span>
  - <span data-ttu-id="67dca-127">**REST API を使用するアプリ**:[クイックスタートとサンプル](https://developer.microsoft.com/graph/get-started)を参照して、選択したプラットフォームを選択し、クイックスタートで実行するか、適切なサンプルを検索します。</span><span class="sxs-lookup"><span data-stu-id="67dca-127">**Apps that use the REST API**: explore [quick starts and samples](https://developer.microsoft.com/graph/get-started), choosing your platform of choice and run through the quick start or search for an appropriate sample</span></span>
  - <span data-ttu-id="67dca-128">**.Net クライアントライブラリを使用するアプリ**: レビュー[コンソール-サンプル](https://github.com/microsoftgraph/console-csharp-snippets-sample)、または[dotnetcore-console](https://github.com/microsoftgraph/dotnetcore-console-sample) -サンプル</span><span class="sxs-lookup"><span data-stu-id="67dca-128">**App that use the .NET client library**: review [console-csharp-snippets-sample](https://github.com/microsoftgraph/console-csharp-snippets-sample) and/or [dotnetcore-console-sample](https://github.com/microsoftgraph/dotnetcore-console-sample)</span></span>

## <a name="next-steps"></a><span data-ttu-id="67dca-129">次のステップ</span><span class="sxs-lookup"><span data-stu-id="67dca-129">Next Steps</span></span>

- <span data-ttu-id="67dca-130">[クイックスタートとサンプル](/graph/get-started)を使用すると、短時間ですばやく開始できます。</span><span class="sxs-lookup"><span data-stu-id="67dca-130">Use [quick starts and samples](/graph/get-started) to come up to speed quickly.</span></span>
- <span data-ttu-id="67dca-131">[クライアントライブラリと sdk](https://developer.microsoft.com/graph/get-started)を活用してカスタムアプリケーションを開発する</span><span class="sxs-lookup"><span data-stu-id="67dca-131">Leverage [client libraries and SDKs](https://developer.microsoft.com/graph/get-started) to develop custom applications</span></span> 
- <span data-ttu-id="67dca-132">[Microsoft Graph](/graph/overview)の概念とプラクティスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="67dca-132">Explore [Microsoft Graph](/graph/overview) concepts and practices.</span></span>
- <span data-ttu-id="67dca-133">[Graph エクスプローラー](https://aka.ms/ge)を使用して、Microsoft graph を試してみてください。</span><span class="sxs-lookup"><span data-stu-id="67dca-133">Use [Graph Explorer](https://aka.ms/ge) to experiment with Microsoft Graph.</span></span>
