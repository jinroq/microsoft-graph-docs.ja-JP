---
title: アプリの移行計画チェックリスト
description: Azure AD Graph から Microsoft Graph にアプリを移行するためのチェックリスト
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 78b6ba30d84a2ca71ae8998df1321b2b8e0ba331
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33630224"
---
# <a name="app-migration-planning-checklist"></a><span data-ttu-id="73e0f-103">アプリの移行計画チェックリスト</span><span class="sxs-lookup"><span data-stu-id="73e0f-103">App migration planning checklist</span></span>

<span data-ttu-id="73e0f-104">移行を計画するには、次のチェックリストを使用します。</span><span class="sxs-lookup"><span data-stu-id="73e0f-104">Use the following checklist to plan your migration:</span></span>

## <a name="step-1-review-the-differences-between-the-apis"></a><span data-ttu-id="73e0f-105">手順 1: Api 間の相違点を確認する</span><span class="sxs-lookup"><span data-stu-id="73e0f-105">Step 1: Review the differences between the APIs</span></span>

<span data-ttu-id="73e0f-106">多くの点で、Microsoft Graph は以前の Azure AD Graph に似ています。</span><span class="sxs-lookup"><span data-stu-id="73e0f-106">In many respects, Microsoft Graph is similar to the earlier Azure AD Graph.</span></span> <span data-ttu-id="73e0f-107">多くの場合、コード内のエンドポイントサービスの名前とバージョンを変更するだけで、すべてが引き続き機能します。</span><span class="sxs-lookup"><span data-stu-id="73e0f-107">In many cases, simply change the endpoint service name and version in your code, and everything should continue to work.</span></span>

<span data-ttu-id="73e0f-108">ただし、違いがあります。</span><span class="sxs-lookup"><span data-stu-id="73e0f-108">Nonetheless, there are differences.</span></span> <span data-ttu-id="73e0f-109">特定のリソース、プロパティ、メソッド、およびコア機能が変更されました。</span><span class="sxs-lookup"><span data-stu-id="73e0f-109">Certain resources, properties, methods, and core capabilities have changed.</span></span>

<span data-ttu-id="73e0f-110">具体的には、次の領域の相違点を確認します。</span><span class="sxs-lookup"><span data-stu-id="73e0f-110">Specifically, look for differences in the following areas:</span></span>

- <span data-ttu-id="73e0f-111">2つのサービス間の[呼び出し構文の要求](migrate-azure-ad-graph-request-differences.md)</span><span class="sxs-lookup"><span data-stu-id="73e0f-111">[Request call syntax](migrate-azure-ad-graph-request-differences.md) between the two services</span></span>
- <span data-ttu-id="73e0f-112">[機能の相違](migrate-azure-ad-graph-feature-differences.md)(ディレクトリ拡張、バッチ処理、差分クエリなど)</span><span class="sxs-lookup"><span data-stu-id="73e0f-112">[Feature differences](migrate-azure-ad-graph-feature-differences.md), such as directory extensions, batching, differential queries, and so on</span></span>
- <span data-ttu-id="73e0f-113">[エンティティリソース名](migrate-azure-ad-graph-resource-differences.md)とその種類</span><span class="sxs-lookup"><span data-stu-id="73e0f-113">[Entity resource names](migrate-azure-ad-graph-resource-differences.md) and their types</span></span>
- <span data-ttu-id="73e0f-114">要求オブジェクトと応答オブジェクトの[プロパティ](migrate-azure-ad-graph-property-differences.md)</span><span class="sxs-lookup"><span data-stu-id="73e0f-114">[Properties](migrate-azure-ad-graph-property-differences.md) of request and response objects</span></span>
- <span data-ttu-id="73e0f-115">パラメーターと型を含む[メソッド](migrate-azure-ad-graph-method-differences.md)</span><span class="sxs-lookup"><span data-stu-id="73e0f-115">[Methods](migrate-azure-ad-graph-method-differences.md), including parameters and types</span></span>

## <a name="step-2-examine-api-use"></a><span data-ttu-id="73e0f-116">手順 2: API の使用を調べる</span><span class="sxs-lookup"><span data-stu-id="73e0f-116">Step 2: Examine API use</span></span>

<span data-ttu-id="73e0f-117">アプリで使用されている Api、必要なアクセス許可、既知の相違点の一覧との比較を[調べ](migrate-azure-ad-graph-audit-api-use.md)ます。</span><span class="sxs-lookup"><span data-stu-id="73e0f-117">[Examine the APIs](migrate-azure-ad-graph-audit-api-use.md) used by your app, the permissions they require, and compare to the list of known differences.</span></span>  

<span data-ttu-id="73e0f-118">アプリが必要とする Api が Microsoft Graph v2.0 で一般的に使用可能になっており、これらの Api が同じように動作することを確認します。</span><span class="sxs-lookup"><span data-stu-id="73e0f-118">Verify that the APIs your app needs are generally available in Microsoft Graph v1.0 and that these APIs work the same way.</span></span>

<span data-ttu-id="73e0f-119">場合によっては、新しい機能が以前の方法で置き換えられるように設計されていることがあります。</span><span class="sxs-lookup"><span data-stu-id="73e0f-119">In some cases, new capabilities and features are designed to replace earlier approaches.</span></span>

<span data-ttu-id="73e0f-120">[Graph エクスプローラー](https://aka.ms/ge)を使用して、新しい通話をテストし、新しいアプローチを開発します。</span><span class="sxs-lookup"><span data-stu-id="73e0f-120">Use the [Graph Explorer](https://aka.ms/ge) to experiment with new calls and to develop new approaches.</span></span> <span data-ttu-id="73e0f-121">最良の結果を得るには、テストテナントでテストユーザーの資格情報を使用してサインインし、API が重要なデータセットを処理する内容を確認します。</span><span class="sxs-lookup"><span data-stu-id="73e0f-121">For best results, sign in using the credentials of a test user in a test tenant so that you see what the API does over important data sets.</span></span>

## <a name="step-3-review-app-details"></a><span data-ttu-id="73e0f-122">手順 3: アプリの詳細を確認する</span><span class="sxs-lookup"><span data-stu-id="73e0f-122">Step 3: Review app details</span></span>

  - <span data-ttu-id="73e0f-123">[アプリの登録](migrate-azure-ad-graph-app-registration.md)と同意の変更 (none である必要があります)。</span><span class="sxs-lookup"><span data-stu-id="73e0f-123">[App registration](migrate-azure-ad-graph-app-registration.md) and consent changes (which should be none).</span></span>
  - <span data-ttu-id="73e0f-124">トークンの取得と[認証のライブラリ](migrate-azure-ad-graph-authentication-library.md)。</span><span class="sxs-lookup"><span data-stu-id="73e0f-124">Token acquisition and [authentication libraries](migrate-azure-ad-graph-authentication-library.md).</span></span>
  - <span data-ttu-id="73e0f-125">.NET アプリケーションの場合、[クライアントライブラリ](migrate-azure-ad-graph-client-libraries.md)を使用します。</span><span class="sxs-lookup"><span data-stu-id="73e0f-125">For .NET applications, use of [client libraries](migrate-azure-ad-graph-client-libraries.md).</span></span>

## <a name="step-4-deploy-test-and-extend-your-app"></a><span data-ttu-id="73e0f-126">手順 4: アプリの展開、テスト、拡張</span><span class="sxs-lookup"><span data-stu-id="73e0f-126">Step 4: Deploy, test, and extend your app</span></span>

<span data-ttu-id="73e0f-127">すべてのユーザーに対してアプリを更新する前に、十分にテストして、お客様の対象者にロールアウトすることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="73e0f-127">Before updating your app for everyone, ensure you test thoroughly and stage your rollout to your customer audience.</span></span>

<span data-ttu-id="73e0f-128">Microsoft Graph への切り替えが完了したので、すぐに使用できるようになるデータセットや機能の多くは、すぐにロック解除することができなくなりました。</span><span class="sxs-lookup"><span data-stu-id="73e0f-128">Now you've made the switch to Microsoft Graph, it's never been easier for you to unlock many more datasets and features that are now at your fingertips.</span></span> <span data-ttu-id="73e0f-129">いくつかの[例](/graph/examples)を見て、考えられることを知ることができます。</span><span class="sxs-lookup"><span data-stu-id="73e0f-129">You can get a taste of what's possible by looking at some [examples](/graph/examples).</span></span>

<span data-ttu-id="73e0f-130">現在[AD 認証ライブラリ](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-libraries)(ADAL) を使用している場合は、 [Microsoft 認証ライブラリ](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries)(msal) に切り替えることを検討してください。</span><span class="sxs-lookup"><span data-stu-id="73e0f-130">If you're currently using the [AD authentication library](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-libraries) (ADAL), consider switching to the [Microsoft authentication library](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) (MSAL).</span></span>

## <a name="next-steps"></a><span data-ttu-id="73e0f-131">次のステップ</span><span class="sxs-lookup"><span data-stu-id="73e0f-131">Next Steps</span></span>

- <span data-ttu-id="73e0f-132">[Resquest 呼び出し構文](migrate-azure-ad-graph-request-differences.md)について説明し、「手順 1: API の違いを確認する」を開始します。</span><span class="sxs-lookup"><span data-stu-id="73e0f-132">Learn about [resquest call syntax](migrate-azure-ad-graph-request-differences.md) to start step 1: reviewing API differences.</span></span>
- <span data-ttu-id="73e0f-133">[Microsoft Graph](/graph/overview)の概念とプラクティスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="73e0f-133">Explore [Microsoft Graph](/graph/overview) concepts and practices.</span></span>
- <span data-ttu-id="73e0f-134">[Graph エクスプローラー](https://aka.ms/ge)を使用して、Microsoft graph を試してみてください。</span><span class="sxs-lookup"><span data-stu-id="73e0f-134">Use [Graph Explorer](https://aka.ms/ge) to experiment with Microsoft Graph.</span></span>
- <span data-ttu-id="73e0f-135">進捗状況の更新とタイムラインの詳細については、「 [Microsoft Graph」または「AZURE AD Graph](https://dev.office.com/blogs/microsoft-graph-or-azure-ad-graph) In The Office デベロッパーセンター」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="73e0f-135">To learn more about progress updates and timelines, see [Microsoft Graph or the Azure AD Graph](https://dev.office.com/blogs/microsoft-graph-or-azure-ad-graph) in the Office Dev Center.</span></span>
