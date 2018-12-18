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

> **注:** 既にクイック スタートがある各プラットフォームのチュートリアルを作成している段階です。 クイック スタートの中には、まだ対応するチュートリアルが存在しないものもあります。

#### <a name="tutorials-and-github-repositories"></a>チュートリアルおよび GitHub リポジトリ

以下の表では、クイック スタートのサンプルごとに、対応するチュートリアルと GitHub レポジトリをリストしています。

| クイック スタート | チュートリアル | GitHub リポジトリ |
|-------------|----------|-------------------|
| Android | なし | [GitHub](https://github.com/microsoftgraph/android-java-connect-sample) |
| Angular | [チュートリアル](/graph/tutorials/angular) | [GitHub](https://github.com/microsoftgraph/msgraph-training-angularspa) |
| ASP.NET MVC | [チュートリアル](/graph/tutorials/aspnet) | [GitHub](https://github.com/microsoftgraph/msgraph-training-aspnetmvcapp) |
| iOS Swift | なし | [GitHub](https://github.com/microsoftgraph/ios-swift-connect-sample) |
| iOS Objective-C | なし | [GitHub](https://github.com/microsoftgraph/ios-objectivec-connect-rest-sample) |
| Node.js | [チュートリアル](/graph/tutorials/node) | [GitHub](https://github.com/microsoftgraph/msgraph-training-nodeexpressapp) |
| PHP | [チュートリアル](/graph/tutorials/php) | [GitHub](https://github.com/microsoftgraph/msgraph-training-phpapp) |
| Python | [チュートリアル](/graph/tutorials/python) | [GitHub](https://github.com/microsoftgraph/msgraph-training-pythondjangoapp) |
| Ruby | [チュートリアル](/graph/tutorials/ruby) | [GitHub](https://github.com/microsoftgraph/msgraph-training-rubyrailsapp) |
| UWP | [チュートリアル](/graph/tutorials/uwp) | [GitHub](https://github.com/microsoftgraph/msgraph-training-uwp) |
| Xamarin | なし | [GitHub](https://github.com/microsoftgraph/uwp-csharp-connect-sample) |

### <a name="why-dont-any-of-the-quick-start-samples-show-advanced-authentication-use-cases"></a>どのクイック スタートのサンプルも、高度な認証のユース ケースを示していないのはなぜですか。

クイック スタートのサンプルでは、認証と Microsoft Graph API 呼び出しの概要を示しています。 他の認証フローの詳細については、[Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/authentication-scenarios) のドキュメントを参照してください。

### <a name="what-if-i-run-into-an-unexpected-error-or-problem-with-a-quick-start"></a>クイック スタートで予期しないエラーや問題が生じた場合、どうしたらよいですか。

クイック スタートが正しく機能しない場合は、対応する GitHub レポジトリで案件をオープンしてください。

## <a name="didnt-find-what-you-need"></a>必要な情報が見つかりませんか。

1 つまたは複数のクイック スタートで生じた疑問や問題が、この「よくあるご質問」に記載されていない場合は、以下の「**フィードバック**」セクションでお知らせください。
