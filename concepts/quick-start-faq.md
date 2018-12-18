---
title: Microsoft Graph のクイック スタートのよくあるご質問
description: この FAQ は、Microsoft Graph のクイック スタートに関連する質問に回答します。
author: jasonjoh
ms.author: jasonjoh
ms.date: 12/13/2018
ms.openlocfilehash: 55630e8fbdbccd8355d2b23e4c839d2ccec2b7d3
ms.sourcegitcommit: f3d479edf03935d0edbbc7668a65f7cde2a56c92
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/15/2018
ms.locfileid: "27283641"
---
# <a name="microsoft-graph-quick-start-faq"></a><span data-ttu-id="870e8-103">Microsoft Graph のクイック スタートのよくあるご質問</span><span class="sxs-lookup"><span data-stu-id="870e8-103">Microsoft Graph quick start FAQ</span></span>

<span data-ttu-id="870e8-104">この FAQ は、[Microsoft Graph Quick Starts](https://developer.microsoft.com/graph/quick-start) に関連する質問に回答します。</span><span class="sxs-lookup"><span data-stu-id="870e8-104">This FAQ answers questions related to the [Microsoft Graph Quick Starts](https://developer.microsoft.com/graph/quick-start).</span></span>

## <a name="general-design"></a><span data-ttu-id="870e8-105">一般設計</span><span class="sxs-lookup"><span data-stu-id="870e8-105">General design</span></span>

<span data-ttu-id="870e8-106">クイック スタートのサンプルでは、Microsoft Graph の機能にアクセスする方法を示します。</span><span class="sxs-lookup"><span data-stu-id="870e8-106">The quick start samples show you how to access the power of Microsoft Graph.</span></span> <span data-ttu-id="870e8-107">これらのサンプルでは、1 つの認証で 2 つのサービス (Microsoft アカウントと Outlook) にアクセスします。</span><span class="sxs-lookup"><span data-stu-id="870e8-107">These samples access two services with one authentication: Microsoft account and Outlook.</span></span> <span data-ttu-id="870e8-108">クイック スタートを行うたびに、Microsoft アカウントのユーザー プロファイルの情報にアクセスし、予定表でイベントを表示します。</span><span class="sxs-lookup"><span data-stu-id="870e8-108">Each quick start accesses information from Microsoft account users' profiles and displays events from their calendar.</span></span>

<span data-ttu-id="870e8-109">クイック スタートには、次の 4 つのステップがあります。</span><span class="sxs-lookup"><span data-stu-id="870e8-109">The quick starts involve four steps:</span></span>

- <span data-ttu-id="870e8-110">プラットフォームを選択する、</span><span class="sxs-lookup"><span data-stu-id="870e8-110">Select your platform</span></span>
- <span data-ttu-id="870e8-111">アプリ ID (クライアント ID) を取得する、</span><span class="sxs-lookup"><span data-stu-id="870e8-111">Get your app ID (client ID)</span></span>
- <span data-ttu-id="870e8-112">サンプルをビルドする、</span><span class="sxs-lookup"><span data-stu-id="870e8-112">Build the sample</span></span>
- <span data-ttu-id="870e8-113">サインインして、予定表でイベントを表示する</span><span class="sxs-lookup"><span data-stu-id="870e8-113">Sign in, and view events on your calendar</span></span>

<span data-ttu-id="870e8-114">クイック スタートを完了すると、すぐに実行できるアプリがあります。</span><span class="sxs-lookup"><span data-stu-id="870e8-114">When you complete the quick start, you have an app that's ready to run.</span></span>

## <a name="general-quick-start-sample-questions"></a><span data-ttu-id="870e8-115">クイック スタートのサンプルに関する一般的な質問</span><span class="sxs-lookup"><span data-stu-id="870e8-115">General quick start sample questions</span></span>

<!-- markdownlint-disable MD026 -->

<span data-ttu-id="870e8-116">このセクションでは、クイック スタートのサンプルの内容に関する質問に回答します。</span><span class="sxs-lookup"><span data-stu-id="870e8-116">This section answers questions about the organization and contents of the quick start samples.</span></span>

### <a name="can-i-get-the-quick-start-code-without-downloading-through-the-quick-start-page"></a><span data-ttu-id="870e8-117">クイック スタート ページでダウンロードしなくても、クイック スタートのコードを入手できますか。</span><span class="sxs-lookup"><span data-stu-id="870e8-117">Can I get the quick start code without downloading through the quick start page?</span></span>

<span data-ttu-id="870e8-118">もちろんです。</span><span class="sxs-lookup"><span data-stu-id="870e8-118">Absolutely.</span></span> <span data-ttu-id="870e8-119">各クイック スタートのダウンロードは、[Microsoft Graph のチュートリアル](tutorials.md)に基づいているため、以下の 2 つの方法で同じソース コードを取得できます。</span><span class="sxs-lookup"><span data-stu-id="870e8-119">Each quick start download is based on a [Microsoft Graph tutorial](tutorials.md), so you have two other options to get the same source code:</span></span>

- <span data-ttu-id="870e8-120">ステップ バイ ステップのチュートリアルに従って、自分でコードをビルドする。</span><span class="sxs-lookup"><span data-stu-id="870e8-120">Build the code yourself by following the step-by-step tutorial.</span></span>
- <span data-ttu-id="870e8-121">対応する GitHub リポジトリからコンプリートされたプロジェクトをダウンロードし、README の指示に従って、サンプルを構成して実行する。</span><span class="sxs-lookup"><span data-stu-id="870e8-121">Download the completed project from the corresponding GitHub repository and follow the instructions in the README to configure and run the sample.</span></span>

> <span data-ttu-id="870e8-122">**注:** 既にクイック スタートがある各プラットフォームのチュートリアルを作成している段階です。</span><span class="sxs-lookup"><span data-stu-id="870e8-122">**Note:** We are in the process of generating tutorials for each of the platforms that currently have a quick start.</span></span> <span data-ttu-id="870e8-123">クイック スタートの中には、まだ対応するチュートリアルが存在しないものもあります。</span><span class="sxs-lookup"><span data-stu-id="870e8-123">Some of the quick starts do not have corresponding tutorials yet.</span></span>

#### <a name="tutorials-and-github-repositories"></a><span data-ttu-id="870e8-124">チュートリアルおよび GitHub リポジトリ</span><span class="sxs-lookup"><span data-stu-id="870e8-124">Tutorials and GitHub repositories</span></span>

<span data-ttu-id="870e8-125">以下の表では、クイック スタートのサンプルごとに、対応するチュートリアルと GitHub レポジトリをリストしています。</span><span class="sxs-lookup"><span data-stu-id="870e8-125">The following table lists the corresponding tutorial and GitHub repository for each quick start sample.</span></span>

| <span data-ttu-id="870e8-126">クイック スタート</span><span class="sxs-lookup"><span data-stu-id="870e8-126">Quick start</span></span> | <span data-ttu-id="870e8-127">チュートリアル</span><span class="sxs-lookup"><span data-stu-id="870e8-127">Tutorial</span></span> | <span data-ttu-id="870e8-128">GitHub リポジトリ</span><span class="sxs-lookup"><span data-stu-id="870e8-128">PnP-Transformation GitHub repository</span></span> |
|-------------|----------|-------------------|
| <span data-ttu-id="870e8-129">Android</span><span class="sxs-lookup"><span data-stu-id="870e8-129">Android</span></span> | <span data-ttu-id="870e8-130">なし</span><span class="sxs-lookup"><span data-stu-id="870e8-130">None</span></span> | [<span data-ttu-id="870e8-131">GitHub</span><span class="sxs-lookup"><span data-stu-id="870e8-131">GitHub Help</span></span>](https://github.com/microsoftgraph/android-java-connect-sample) |
| <span data-ttu-id="870e8-132">Angular</span><span class="sxs-lookup"><span data-stu-id="870e8-132">Angular</span></span> | [<span data-ttu-id="870e8-133">チュートリアル</span><span class="sxs-lookup"><span data-stu-id="870e8-133">Tutorial</span></span>](/graph/tutorials/angular) | [<span data-ttu-id="870e8-134">GitHub</span><span class="sxs-lookup"><span data-stu-id="870e8-134">GitHub Help</span></span>](https://github.com/microsoftgraph/msgraph-training-angularspa) |
| <span data-ttu-id="870e8-135">ASP.NET MVC</span><span class="sxs-lookup"><span data-stu-id="870e8-135">ASP.NET MVC</span></span> | [<span data-ttu-id="870e8-136">チュートリアル</span><span class="sxs-lookup"><span data-stu-id="870e8-136">Tutorial</span></span>](/graph/tutorials/aspnet) | [<span data-ttu-id="870e8-137">GitHub</span><span class="sxs-lookup"><span data-stu-id="870e8-137">GitHub Help</span></span>](https://github.com/microsoftgraph/msgraph-training-aspnetmvcapp) |
| <span data-ttu-id="870e8-138">iOS Swift</span><span class="sxs-lookup"><span data-stu-id="870e8-138">iOS (Swift)</span></span> | <span data-ttu-id="870e8-139">なし</span><span class="sxs-lookup"><span data-stu-id="870e8-139">None</span></span> | [<span data-ttu-id="870e8-140">GitHub</span><span class="sxs-lookup"><span data-stu-id="870e8-140">GitHub Help</span></span>](https://github.com/microsoftgraph/ios-swift-connect-sample) |
| <span data-ttu-id="870e8-141">iOS Objective-C</span><span class="sxs-lookup"><span data-stu-id="870e8-141">iOS Objective-C</span></span> | <span data-ttu-id="870e8-142">なし</span><span class="sxs-lookup"><span data-stu-id="870e8-142">None</span></span> | [<span data-ttu-id="870e8-143">GitHub</span><span class="sxs-lookup"><span data-stu-id="870e8-143">GitHub Help</span></span>](https://github.com/microsoftgraph/ios-objectivec-connect-rest-sample) |
| <span data-ttu-id="870e8-144">Node.js</span><span class="sxs-lookup"><span data-stu-id="870e8-144">Node.js</span></span> | [<span data-ttu-id="870e8-145">チュートリアル</span><span class="sxs-lookup"><span data-stu-id="870e8-145">Tutorial</span></span>](/graph/tutorials/node) | [<span data-ttu-id="870e8-146">GitHub</span><span class="sxs-lookup"><span data-stu-id="870e8-146">GitHub Help</span></span>](https://github.com/microsoftgraph/msgraph-training-nodeexpressapp) |
| <span data-ttu-id="870e8-147">PHP</span><span class="sxs-lookup"><span data-stu-id="870e8-147">PHP</span></span> | [<span data-ttu-id="870e8-148">チュートリアル</span><span class="sxs-lookup"><span data-stu-id="870e8-148">Tutorial</span></span>](/graph/tutorials/php) | [<span data-ttu-id="870e8-149">GitHub</span><span class="sxs-lookup"><span data-stu-id="870e8-149">GitHub Help</span></span>](https://github.com/microsoftgraph/msgraph-training-phpapp) |
| <span data-ttu-id="870e8-150">Python</span><span class="sxs-lookup"><span data-stu-id="870e8-150">Python</span></span> | [<span data-ttu-id="870e8-151">チュートリアル</span><span class="sxs-lookup"><span data-stu-id="870e8-151">Tutorial</span></span>](/graph/tutorials/python) | [<span data-ttu-id="870e8-152">GitHub</span><span class="sxs-lookup"><span data-stu-id="870e8-152">GitHub Help</span></span>](https://github.com/microsoftgraph/msgraph-training-pythondjangoapp) |
| <span data-ttu-id="870e8-153">Ruby</span><span class="sxs-lookup"><span data-stu-id="870e8-153">Ruby</span></span> | [<span data-ttu-id="870e8-154">チュートリアル</span><span class="sxs-lookup"><span data-stu-id="870e8-154">Tutorial</span></span>](/graph/tutorials/ruby) | [<span data-ttu-id="870e8-155">GitHub</span><span class="sxs-lookup"><span data-stu-id="870e8-155">GitHub Help</span></span>](https://github.com/microsoftgraph/msgraph-training-rubyrailsapp) |
| <span data-ttu-id="870e8-156">UWP</span><span class="sxs-lookup"><span data-stu-id="870e8-156">UWP</span></span> | [<span data-ttu-id="870e8-157">チュートリアル</span><span class="sxs-lookup"><span data-stu-id="870e8-157">Tutorial</span></span>](/graph/tutorials/uwp) | [<span data-ttu-id="870e8-158">GitHub</span><span class="sxs-lookup"><span data-stu-id="870e8-158">GitHub Help</span></span>](https://github.com/microsoftgraph/msgraph-training-uwp) |
| <span data-ttu-id="870e8-159">Xamarin</span><span class="sxs-lookup"><span data-stu-id="870e8-159">Xamarin</span></span> | <span data-ttu-id="870e8-160">なし</span><span class="sxs-lookup"><span data-stu-id="870e8-160">None</span></span> | [<span data-ttu-id="870e8-161">GitHub</span><span class="sxs-lookup"><span data-stu-id="870e8-161">GitHub Help</span></span>](https://github.com/microsoftgraph/uwp-csharp-connect-sample) |

### <a name="why-dont-any-of-the-quick-start-samples-show-advanced-authentication-use-cases"></a><span data-ttu-id="870e8-162">どのクイック スタートのサンプルも、高度な認証のユース ケースを示していないのはなぜですか。</span><span class="sxs-lookup"><span data-stu-id="870e8-162">Why don't any of the quick start samples show advanced authentication use cases?</span></span>

<span data-ttu-id="870e8-163">クイック スタートのサンプルでは、認証と Microsoft Graph API 呼び出しの概要を示しています。</span><span class="sxs-lookup"><span data-stu-id="870e8-163">The quick start samples give you an introduction to authentication and Microsoft Graph API calls.</span></span> <span data-ttu-id="870e8-164">他の認証フローの詳細については、[Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/authentication-scenarios) のドキュメントを参照してください。</span><span class="sxs-lookup"><span data-stu-id="870e8-164">You can learn more about other authentication flows in the [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/authentication-scenarios) documentation.</span></span>

### <a name="what-if-i-run-into-an-unexpected-error-or-problem-with-a-quick-start"></a><span data-ttu-id="870e8-165">クイック スタートで予期しないエラーや問題が生じた場合、どうしたらよいですか。</span><span class="sxs-lookup"><span data-stu-id="870e8-165">What if I run into an unexpected error or problem with a quick start?</span></span>

<span data-ttu-id="870e8-166">クイック スタートが正しく機能しない場合は、対応する GitHub レポジトリで案件をオープンしてください。</span><span class="sxs-lookup"><span data-stu-id="870e8-166">If you have trouble getting the quick start to work properly, please open an issue on the corresponding GitHub repository.</span></span>

## <a name="didnt-find-what-you-need"></a><span data-ttu-id="870e8-167">必要な情報が見つかりませんか。</span><span class="sxs-lookup"><span data-stu-id="870e8-167">Didn't find what you need?</span></span>

<span data-ttu-id="870e8-168">1 つまたは複数のクイック スタートで生じた疑問や問題が、この「よくあるご質問」に記載されていない場合は、以下の「**フィードバック**」セクションでお知らせください。</span><span class="sxs-lookup"><span data-stu-id="870e8-168">If this FAQ didn't address a question or problem you encountered with one or more of the quick starts, please let us know using the **Feedback** section below.</span></span>
