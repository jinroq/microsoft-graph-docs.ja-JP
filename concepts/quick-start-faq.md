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
# <a name="microsoft-graph-quick-start-faq"></a>Microsoft Graph のクイック スタートのよくあるご質問

この FAQ は、[Microsoft Graph Quick Starts](https://developer.microsoft.com/graph/quick-start) に関連する質問に回答します。

## <a name="general-design"></a>一般設計

クイック スタートのサンプルでは、Microsoft Graph の機能にアクセスする方法を示します。 これらのサンプルでは、1 つの認証で 2 つのサービス (Microsoft アカウントと Outlook) にアクセスします。 クイック スタートを行うたびに、Microsoft アカウントのユーザー プロファイルの情報にアクセスし、予定表でイベントを表示します。

クイック スタートには、次の 4 つのステップがあります。

- プラットフォームを選択する、
- アプリ ID (クライアント ID) を取得する、
- サンプルをビルドする、
- サインインして、予定表でイベントを表示する

クイック スタートを完了すると、すぐに実行できるアプリがあります。

## <a name="general-quick-start-sample-questions"></a>クイック スタートのサンプルに関する一般的な質問

<!-- markdownlint-disable MD026 -->

このセクションでは、クイック スタートのサンプルの内容に関する質問に回答します。

### <a name="can-i-get-the-quick-start-code-without-downloading-through-the-quick-start-page"></a>クイック スタート ページでダウンロードしなくても、クイック スタートのコードを入手できますか。

もちろんです。 各クイック スタートのダウンロードは、[Microsoft Graph のチュートリアル](tutorials.md)に基づいているため、以下の 2 つの方法で同じソース コードを取得できます。

- ステップ バイ ステップのチュートリアルに従って、自分でコードをビルドする。
- 対応する GitHub リポジトリからコンプリートされたプロジェクトをダウンロードし、README の指示に従って、サンプルを構成して実行する。

> [!NOTE]
> 現在、クイック スタートがある各プラットフォームのチュートリアルを作成している段階です。 クイック スタートの中には、まだ対応するチュートリアルが存在しないものもあります。

#### <a name="tutorials-and-github-repositories"></a>チュートリアルおよび GitHub リポジトリ

以下の表では、クイック スタートのサンプルごとに、対応するチュートリアルと GitHub レポジトリをリストしています。

| クイック スタート | チュートリアル | GitHub リポジトリ |
|-------------|----------|-------------------|
| Android | [チュートリアル](/graph/tutorials/android) | [GitHub](https://github.com/microsoftgraph/android-java-connect-sample) |
| Angular | [チュートリアル](/graph/tutorials/angular) | [GitHub](https://github.com/microsoftgraph/msgraph-training-angularspa) |
| ASP.NET MVC | [チュートリアル](/graph/tutorials/aspnet) | [GitHub](https://github.com/microsoftgraph/msgraph-training-aspnetmvcapp) |
| iOS Swift | なし | [GitHub](https://github.com/microsoftgraph/ios-swift-connect-sample) |
| iOS Objective-C | なし | [GitHub](https://github.com/microsoftgraph/ios-objectivec-connect-rest-sample) |
| Node.js | [チュートリアル](/graph/tutorials/node) | [GitHub](https://github.com/microsoftgraph/msgraph-training-nodeexpressapp) |
| PHP | [チュートリアル](/graph/tutorials/php) | [GitHub](https://github.com/microsoftgraph/msgraph-training-phpapp) |
| Python | [チュートリアル](/graph/tutorials/python) | [GitHub](https://github.com/microsoftgraph/msgraph-training-pythondjangoapp) |
| Ruby | [チュートリアル](/graph/tutorials/ruby) | [GitHub](https://github.com/microsoftgraph/msgraph-training-rubyrailsapp) |
| UWP | [チュートリアル](/graph/tutorials/uwp) | [GitHub](https://github.com/microsoftgraph/msgraph-training-uwp) |
| Xamarin | なし | [GitHub](https://github.com/microsoftgraph/xamarin-csharp-connect-sample) |

### <a name="why-dont-any-of-the-quick-start-samples-show-advanced-authentication-use-cases"></a>どのクイック スタートのサンプルも、高度な認証のユース ケースを示していないのはなぜですか。

クイック スタートのサンプルでは、認証と Microsoft Graph API 呼び出しの概要を示しています。 他の認証フローの詳細については、[Azure Active Directory](/azure/active-directory/develop/authentication-scenarios) のドキュメントを参照してください。

### <a name="what-if-i-run-into-an-unexpected-error-or-problem-with-a-quick-start"></a>クイック スタートで予期しないエラーや問題が生じた場合、どうしたらよいですか。

クイック スタートが正しく機能しない場合は、対応する GitHub レポジトリで案件をオープンしてください。

## <a name="known-issues"></a>既知の問題

### <a name="aspnet-quick-start-displays-an-error-when-running-it-cannot-find-a-part-of-the-path-graph-tutorialgraph-tutorialbinroslyncscexe"></a>ASP.NET クイックスタートを実行すると、エラーが表示されます。パス「[...]\Graph Tutorial\graph-tutorial\bin\roslyn\csc.exe」の一部が見つかりません。

これは、[Visual Studio と Roslyn コンパイラの問題](https://github.com/dotnet/roslyn/issues/15556)が原因で発生します。 エラーを解決するには、次のいずれかのオプションを選択します。

- ソリューション エクスプローラーでプロジェクトをアンロード / 再読み込みする
- ソリューションをクリーン / 再構築する
- NuGet パッケージをアップグレードする

### <a name="im-getting-aadsts50011-the-reply-url-specified-in-the-request-does-not-match-the-reply-urls-configured-for-the-application-when-running-a-quick-start"></a>クイック スタートを実行すると、「AADSTS 50011: リクエストに指定された返信 URL がアプリケーションに設定された返信 URL と一致しません」と表示されます。

これは、クイック スタートのアプリケーション登録に問題があることを示します。 [Microsoft Graph クイック スタート ページ](https://developer.microsoft.com/graph/quick-start)からクイック スタートをダウンロードすると、アプリケーションの登録が自動的に作成されます。また、サンプル プロジェクトで使用される既定の URL と一致する、返信 URL (リダイレクト URL とも呼ばれる) を構成します。 URL を変更すると、アプリの登録は一致しなくなり、このエラーが発生する場合があります。 このエラーを解決するには、クイック スタート プロジェクトの付属の README.md ファイルを確認して、アプリの登録を作成し、サンプル コードでそれを構成する手順を参照してください。

## <a name="didnt-find-what-you-need"></a>必要な情報が見つかりませんか。

1 つまたは複数のクイック スタートで生じた疑問や問題が、この「よくあるご質問」に記載されていない場合は、以下の「**フィードバック**」セクションでお知らせください。
