---
title: Microsoft Graph のクイック スタートのよくあるご質問
description: この FAQ は、Microsoft Graph のクイック スタートに関連する質問に回答します。
author: jasonjoh
ms.author: jasonjoh
localization_priority: Normal
ms.openlocfilehash: bd1405f4805bb9740fb7119adcf2f877236d19cf
ms.sourcegitcommit: b523648530fcc8c2a3ded35b419be8047b9fcd10
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/20/2019
ms.locfileid: "35084090"
---
# <a name="microsoft-graph-quick-start-faq"></a><span data-ttu-id="4aac7-103">Microsoft Graph のクイック スタートのよくあるご質問</span><span class="sxs-lookup"><span data-stu-id="4aac7-103">Microsoft Graph quick start FAQ</span></span>

<span data-ttu-id="4aac7-104">この FAQ は、[Microsoft Graph Quick Starts](https://developer.microsoft.com/graph/quick-start) に関連する質問に回答します。</span><span class="sxs-lookup"><span data-stu-id="4aac7-104">This FAQ answers questions related to the [Microsoft Graph Quick Starts](https://developer.microsoft.com/graph/quick-start).</span></span>

## <a name="general-design"></a><span data-ttu-id="4aac7-105">一般設計</span><span class="sxs-lookup"><span data-stu-id="4aac7-105">General design</span></span>

<span data-ttu-id="4aac7-106">クイック スタートのサンプルでは、Microsoft Graph の機能にアクセスする方法を示します。</span><span class="sxs-lookup"><span data-stu-id="4aac7-106">The quick start samples show you how to access the power of Microsoft Graph.</span></span> <span data-ttu-id="4aac7-107">これらのサンプルでは、1 つの認証で 2 つのサービス (Microsoft アカウントと Outlook) にアクセスします。</span><span class="sxs-lookup"><span data-stu-id="4aac7-107">These samples access two services with one authentication: Microsoft account and Outlook.</span></span> <span data-ttu-id="4aac7-108">クイック スタートを行うたびに、Microsoft アカウントのユーザー プロファイルの情報にアクセスし、予定表でイベントを表示します。</span><span class="sxs-lookup"><span data-stu-id="4aac7-108">Each quick start accesses information from Microsoft account users' profiles and displays events from their calendar.</span></span>

<span data-ttu-id="4aac7-109">クイック スタートには、次の 4 つのステップがあります。</span><span class="sxs-lookup"><span data-stu-id="4aac7-109">The quick starts involve four steps:</span></span>

- <span data-ttu-id="4aac7-110">プラットフォームを選択する、</span><span class="sxs-lookup"><span data-stu-id="4aac7-110">Select your platform</span></span>
- <span data-ttu-id="4aac7-111">アプリ ID (クライアント ID) を取得する、</span><span class="sxs-lookup"><span data-stu-id="4aac7-111">Get your app ID (client ID)</span></span>
- <span data-ttu-id="4aac7-112">サンプルをビルドする、</span><span class="sxs-lookup"><span data-stu-id="4aac7-112">Build the sample</span></span>
- <span data-ttu-id="4aac7-113">サインインして、予定表でイベントを表示する</span><span class="sxs-lookup"><span data-stu-id="4aac7-113">Sign in, and view events on your calendar</span></span>

<span data-ttu-id="4aac7-114">クイック スタートを完了すると、すぐに実行できるアプリがあります。</span><span class="sxs-lookup"><span data-stu-id="4aac7-114">When you complete the quick start, you have an app that's ready to run.</span></span>

## <a name="general-quick-start-sample-questions"></a><span data-ttu-id="4aac7-115">クイック スタートのサンプルに関する一般的な質問</span><span class="sxs-lookup"><span data-stu-id="4aac7-115">General quick start sample questions</span></span>

<!-- markdownlint-disable MD026 -->

<span data-ttu-id="4aac7-116">このセクションでは、クイック スタートのサンプルの内容に関する質問に回答します。</span><span class="sxs-lookup"><span data-stu-id="4aac7-116">This section answers questions about the contents of the quick start samples.</span></span>

### <a name="can-i-get-the-quick-start-code-without-downloading-through-the-quick-start-page"></a><span data-ttu-id="4aac7-117">クイック スタート ページでダウンロードしなくても、クイック スタートのコードを入手できますか。</span><span class="sxs-lookup"><span data-stu-id="4aac7-117">Can I get the quick start code without downloading through the quick start page?</span></span>

<span data-ttu-id="4aac7-118">もちろんです。</span><span class="sxs-lookup"><span data-stu-id="4aac7-118">Absolutely!</span></span> <span data-ttu-id="4aac7-119">各クイック スタートのダウンロードは、[Microsoft Graph のチュートリアル](tutorials.md)に基づいているため、以下の 2 つの方法で同じソース コードを取得できます。</span><span class="sxs-lookup"><span data-stu-id="4aac7-119">Each quick start download is based on a [Microsoft Graph tutorial](tutorials.md), so you have two other options to get the same source code:</span></span>

- <span data-ttu-id="4aac7-120">ステップ バイ ステップのチュートリアルに従って、自分でコードをビルドする。</span><span class="sxs-lookup"><span data-stu-id="4aac7-120">Build the code yourself by following the step-by-step tutorial.</span></span>
- <span data-ttu-id="4aac7-121">対応する GitHub リポジトリからコンプリートされたプロジェクトをダウンロードし、README の指示に従って、サンプルを構成して実行する。</span><span class="sxs-lookup"><span data-stu-id="4aac7-121">Download the completed project from the corresponding GitHub repository and follow the instructions in the README to configure and run the sample.</span></span>

> [!NOTE]
> <span data-ttu-id="4aac7-122">現在、クイック スタートがある各プラットフォームのチュートリアルを作成している段階です。</span><span class="sxs-lookup"><span data-stu-id="4aac7-122">Note: We are in the process of generating tutorials for each of the platforms that currently have a quick start.</span></span> <span data-ttu-id="4aac7-123">クイック スタートの中には、まだ対応するチュートリアルが存在しないものもあります。</span><span class="sxs-lookup"><span data-stu-id="4aac7-123">Some of the quick starts do not have corresponding tutorials yet.</span></span>

#### <a name="tutorials-and-github-repositories"></a><span data-ttu-id="4aac7-124">チュートリアルおよび GitHub リポジトリ</span><span class="sxs-lookup"><span data-stu-id="4aac7-124">Tutorials and GitHub repositories</span></span>

<span data-ttu-id="4aac7-125">以下の表では、クイック スタートのサンプルごとに、対応するチュートリアルと GitHub レポジトリをリストしています。</span><span class="sxs-lookup"><span data-stu-id="4aac7-125">The following table lists the corresponding tutorial and GitHub repository for each quick start sample.</span></span>

| <span data-ttu-id="4aac7-126">クイック スタート</span><span class="sxs-lookup"><span data-stu-id="4aac7-126">Quick start</span></span> | <span data-ttu-id="4aac7-127">チュートリアル</span><span class="sxs-lookup"><span data-stu-id="4aac7-127">Tutorial</span></span> | <span data-ttu-id="4aac7-128">GitHub リポジトリ</span><span class="sxs-lookup"><span data-stu-id="4aac7-128">GitHub repository</span></span> |
|-------------|----------|-------------------|
| <span data-ttu-id="4aac7-129">Android</span><span class="sxs-lookup"><span data-stu-id="4aac7-129">Android</span></span> | [<span data-ttu-id="4aac7-130">チュートリアル</span><span class="sxs-lookup"><span data-stu-id="4aac7-130">Tutorial</span></span>](/graph/tutorials/android) | [<span data-ttu-id="4aac7-131">GitHub</span><span class="sxs-lookup"><span data-stu-id="4aac7-131">GitHub</span></span>](https://github.com/microsoftgraph/android-java-connect-sample) |
| <span data-ttu-id="4aac7-132">Angular</span><span class="sxs-lookup"><span data-stu-id="4aac7-132">Angular</span></span> | [<span data-ttu-id="4aac7-133">チュートリアル</span><span class="sxs-lookup"><span data-stu-id="4aac7-133">Tutorial</span></span>](/graph/tutorials/angular) | [<span data-ttu-id="4aac7-134">GitHub</span><span class="sxs-lookup"><span data-stu-id="4aac7-134">GitHub</span></span>](https://github.com/microsoftgraph/msgraph-training-angularspa) |
| <span data-ttu-id="4aac7-135">ASP.NET MVC</span><span class="sxs-lookup"><span data-stu-id="4aac7-135">ASP.NET MVC</span></span> | [<span data-ttu-id="4aac7-136">チュートリアル</span><span class="sxs-lookup"><span data-stu-id="4aac7-136">Tutorial</span></span>](/graph/tutorials/aspnet) | [<span data-ttu-id="4aac7-137">GitHub</span><span class="sxs-lookup"><span data-stu-id="4aac7-137">GitHub</span></span>](https://github.com/microsoftgraph/msgraph-training-aspnetmvcapp) |
| <span data-ttu-id="4aac7-138">iOS Swift</span><span class="sxs-lookup"><span data-stu-id="4aac7-138">iOS Swift</span></span> | <span data-ttu-id="4aac7-139">なし</span><span class="sxs-lookup"><span data-stu-id="4aac7-139">None</span></span> | [<span data-ttu-id="4aac7-140">GitHub</span><span class="sxs-lookup"><span data-stu-id="4aac7-140">GitHub</span></span>](https://github.com/microsoftgraph/ios-swift-connect-sample) |
| <span data-ttu-id="4aac7-141">iOS Objective-C</span><span class="sxs-lookup"><span data-stu-id="4aac7-141">iOS Objective-C</span></span> | <span data-ttu-id="4aac7-142">なし</span><span class="sxs-lookup"><span data-stu-id="4aac7-142">None</span></span> | [<span data-ttu-id="4aac7-143">GitHub</span><span class="sxs-lookup"><span data-stu-id="4aac7-143">GitHub</span></span>](https://github.com/microsoftgraph/ios-objectivec-connect-rest-sample) |
| <span data-ttu-id="4aac7-144">Node.js</span><span class="sxs-lookup"><span data-stu-id="4aac7-144">Node.js</span></span> | [<span data-ttu-id="4aac7-145">チュートリアル</span><span class="sxs-lookup"><span data-stu-id="4aac7-145">Tutorial</span></span>](/graph/tutorials/node) | [<span data-ttu-id="4aac7-146">GitHub</span><span class="sxs-lookup"><span data-stu-id="4aac7-146">GitHub</span></span>](https://github.com/microsoftgraph/msgraph-training-nodeexpressapp) |
| <span data-ttu-id="4aac7-147">PHP</span><span class="sxs-lookup"><span data-stu-id="4aac7-147">PHP</span></span> | [<span data-ttu-id="4aac7-148">チュートリアル</span><span class="sxs-lookup"><span data-stu-id="4aac7-148">Tutorial</span></span>](/graph/tutorials/php) | [<span data-ttu-id="4aac7-149">GitHub</span><span class="sxs-lookup"><span data-stu-id="4aac7-149">GitHub</span></span>](https://github.com/microsoftgraph/msgraph-training-phpapp) |
| <span data-ttu-id="4aac7-150">Python</span><span class="sxs-lookup"><span data-stu-id="4aac7-150">Python</span></span> | [<span data-ttu-id="4aac7-151">チュートリアル</span><span class="sxs-lookup"><span data-stu-id="4aac7-151">Tutorial</span></span>](/graph/tutorials/python) | [<span data-ttu-id="4aac7-152">GitHub</span><span class="sxs-lookup"><span data-stu-id="4aac7-152">GitHub</span></span>](https://github.com/microsoftgraph/msgraph-training-pythondjangoapp) |
| <span data-ttu-id="4aac7-153">Ruby</span><span class="sxs-lookup"><span data-stu-id="4aac7-153">Ruby</span></span> | [<span data-ttu-id="4aac7-154">チュートリアル</span><span class="sxs-lookup"><span data-stu-id="4aac7-154">Tutorial</span></span>](/graph/tutorials/ruby) | [<span data-ttu-id="4aac7-155">GitHub</span><span class="sxs-lookup"><span data-stu-id="4aac7-155">GitHub</span></span>](https://github.com/microsoftgraph/msgraph-training-rubyrailsapp) |
| <span data-ttu-id="4aac7-156">UWP</span><span class="sxs-lookup"><span data-stu-id="4aac7-156">UWP</span></span> | [<span data-ttu-id="4aac7-157">チュートリアル</span><span class="sxs-lookup"><span data-stu-id="4aac7-157">Tutorial</span></span>](/graph/tutorials/uwp) | [<span data-ttu-id="4aac7-158">GitHub</span><span class="sxs-lookup"><span data-stu-id="4aac7-158">GitHub</span></span>](https://github.com/microsoftgraph/msgraph-training-uwp) |
| <span data-ttu-id="4aac7-159">Xamarin</span><span class="sxs-lookup"><span data-stu-id="4aac7-159">Xamarin</span></span> | <span data-ttu-id="4aac7-160">なし</span><span class="sxs-lookup"><span data-stu-id="4aac7-160">None</span></span> | [<span data-ttu-id="4aac7-161">GitHub</span><span class="sxs-lookup"><span data-stu-id="4aac7-161">GitHub</span></span>](https://github.com/microsoftgraph/xamarin-csharp-connect-sample) |

### <a name="why-dont-any-of-the-quick-start-samples-show-advanced-authentication-use-cases"></a><span data-ttu-id="4aac7-162">どのクイック スタートのサンプルも、高度な認証のユース ケースを示していないのはなぜですか。</span><span class="sxs-lookup"><span data-stu-id="4aac7-162">Why don't any of the quick start samples show advanced authentication use cases?</span></span>

<span data-ttu-id="4aac7-163">クイック スタートのサンプルでは、認証と Microsoft Graph API 呼び出しの概要を示しています。</span><span class="sxs-lookup"><span data-stu-id="4aac7-163">The quick start samples give you an introduction to authentication and Microsoft Graph API calls.</span></span> <span data-ttu-id="4aac7-164">他の認証フローの詳細については、[Azure Active Directory](/azure/active-directory/develop/authentication-scenarios) のドキュメントを参照してください。</span><span class="sxs-lookup"><span data-stu-id="4aac7-164">You can learn more about other authentication flows in the [Azure Active Directory](/azure/active-directory/develop/authentication-scenarios) documentation.</span></span>

### <a name="what-if-i-run-into-an-unexpected-error-or-problem-with-a-quick-start"></a><span data-ttu-id="4aac7-165">クイック スタートで予期しないエラーや問題が生じた場合、どうしたらよいですか。</span><span class="sxs-lookup"><span data-stu-id="4aac7-165">What if I run into an unexpected error or problem with a quick start?</span></span>

<span data-ttu-id="4aac7-166">クイック スタートが正しく機能しない場合は、対応する GitHub レポジトリで案件をオープンしてください。</span><span class="sxs-lookup"><span data-stu-id="4aac7-166">If you have trouble getting the quick start to work properly, please open an issue on the corresponding GitHub repository.</span></span>

## <a name="known-issues"></a><span data-ttu-id="4aac7-167">既知の問題</span><span class="sxs-lookup"><span data-stu-id="4aac7-167">Known issues</span></span>

### <a name="aspnet-quick-start-displays-an-error-when-running-it-cannot-find-a-part-of-the-path-graph-tutorialgraph-tutorialbinroslyncscexe"></a><span data-ttu-id="4aac7-168">ASP.NET クイックスタートを実行すると、エラーが表示されます。パス「[...]\Graph Tutorial\graph-tutorial\bin\roslyn\csc.exe」の一部が見つかりません。</span><span class="sxs-lookup"><span data-stu-id="4aac7-168">ASP.NET quick start displays an error when running it: Cannot find a part of the path '[...]\Graph Tutorial\graph-tutorial\bin\roslyn\csc.exe'.</span></span>

<span data-ttu-id="4aac7-169">これは、[Visual Studio と Roslyn コンパイラの問題](https://github.com/dotnet/roslyn/issues/15556)が原因で発生します。</span><span class="sxs-lookup"><span data-stu-id="4aac7-169">This is caused by an [issue with Visual Studio and the Roslyn compiler](https://github.com/dotnet/roslyn/issues/15556).</span></span> <span data-ttu-id="4aac7-170">エラーを解決するには、次のいずれかのオプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="4aac7-170">One of the following options should resolve the error.</span></span>

- <span data-ttu-id="4aac7-171">ソリューション エクスプローラーでプロジェクトをアンロード / 再読み込みする</span><span class="sxs-lookup"><span data-stu-id="4aac7-171">Branding101 project in Solution Explorer</span></span>
- <span data-ttu-id="4aac7-172">ソリューションをクリーン / 再構築する</span><span class="sxs-lookup"><span data-stu-id="4aac7-172">Clean/Rebuild solution</span></span>
- <span data-ttu-id="4aac7-173">NuGet パッケージをアップグレードする</span><span class="sxs-lookup"><span data-stu-id="4aac7-173">Upgrade NuGet packages</span></span>

### <a name="im-getting-aadsts50011-the-reply-url-specified-in-the-request-does-not-match-the-reply-urls-configured-for-the-application-when-running-a-quick-start"></a><span data-ttu-id="4aac7-174">クイック スタートを実行すると、「AADSTS 50011: リクエストに指定された返信 URL がアプリケーションに設定された返信 URL と一致しません」と表示されます。</span><span class="sxs-lookup"><span data-stu-id="4aac7-174">I'm getting "AADSTS50011: The reply url specified in the request does not match the reply urls configured for the application" when running a quick start.</span></span>

<span data-ttu-id="4aac7-175">これは、クイック スタートのアプリケーション登録に問題があることを示します。</span><span class="sxs-lookup"><span data-stu-id="4aac7-175">This indicates a problem with the application registration for the quick start.</span></span> <span data-ttu-id="4aac7-176">[Microsoft Graph クイック スタート ページ](https://developer.microsoft.com/graph/quick-start)からクイック スタートをダウンロードすると、アプリケーションの登録が自動的に作成されます。また、サンプル プロジェクトで使用される既定の URL と一致する、返信 URL (リダイレクト URL とも呼ばれる) を構成します。</span><span class="sxs-lookup"><span data-stu-id="4aac7-176">When you download a quick start from the [Microsoft Graph Quick Starts page](https://developer.microsoft.com/graph/quick-start), we create the application registration for you, and configure a reply URL (also known as a redirect URL) that matches the default URL used by the sample project.</span></span> <span data-ttu-id="4aac7-177">URL を変更すると、アプリの登録は一致しなくなり、このエラーが発生する場合があります。</span><span class="sxs-lookup"><span data-stu-id="4aac7-177">If you change the URL, the app registration will no longer match and could cause this error.</span></span> <span data-ttu-id="4aac7-178">このエラーを解決するには、クイック スタート プロジェクトの付属の README.md ファイルを確認して、アプリの登録を作成し、サンプル コードでそれを構成する手順を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4aac7-178">To resolve this error, consult the README.md file included with the quick start project for instructions on how to create an app registration and configure it in the sample code.</span></span>

## <a name="didnt-find-what-you-need"></a><span data-ttu-id="4aac7-179">必要な情報が見つかりませんか。</span><span class="sxs-lookup"><span data-stu-id="4aac7-179">Didn't find what you need?</span></span>

<span data-ttu-id="4aac7-180">1 つまたは複数のクイック スタートで生じた疑問や問題が、この「よくあるご質問」に記載されていない場合は、以下の「**フィードバック**」セクションでお知らせください。</span><span class="sxs-lookup"><span data-stu-id="4aac7-180">If this FAQ didn't address a question or problem you encountered with one or more of the quick starts, please let us know using the **Feedback** section below.</span></span>
