---
title: OneNote API の概要
description: OneNote は、顧客が Web、電話、タブレット、またはデスクトップ上で文字、スケッチ、音声を入力することで、家庭、学校、または職場用のアイデアやメモを追跡できるデジタル ノートブックです。 自由にメモを整理し、デバイスを切り替えて作業の中断箇所から再開し、他のユーザーとリアルタイムでメモの共同作業を行えます。
author: Jewan-microsoft
localization_priority: Priority
ms.prod: onenote
scenarios: getting-started
ms.openlocfilehash: 69aa0d83d9625559c7731391f6ad504bd86403f0
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/07/2019
ms.locfileid: "36792612"
---
# <a name="onenote-api-overview"></a>OneNote API の概要

OneNote は、顧客が Web、電話、タブレット、またはデスクトップ上で文字、スケッチ、音声を入力することで、家庭、学校、または職場用のアイデアやメモを追跡できるデジタル ノートブックです。 自由にメモを整理し、デバイスを切り替えて作業の中断箇所から再開し、他のユーザーとリアルタイムでメモの共同作業を行えます。

> [!VIDEO https://www.youtube-nocookie.com/embed/VXd4OeQU1ek]

## <a name="why-integrate-with-onenote"></a>OneNote と統合する理由

アプリを OneNote に統合すると、複数のプラットフォームで利用できる便利な機能を作成し、世界中の数百万人のユーザーに届けることができます。 Microsoft Graph を使用して OneNote のノートブック、セクション、ページにアクセスし、ユーザーによるアイデアや情報の計画や整理を支援するソリューションを作成することができます。

### <a name="collect-and-organize-notes-and-ideas"></a>メモやアイデアを収集して整理する  

コンテンツを追加したり、アレンジしたりできるキャンバスとして OneNote を使用します。 Microsoft Graph を使用すると、学生がメモを取って調査すること、家族が計画とアイデアを共有すること、買い物客が画像を共有することを可能にするアプリを簡単に作成できます。 アプリでは、みんなが必要とする情報を集め、OneNote に送り、それらを整理することができます。

### <a name="capture-information-in-many-formats"></a>さまざまな形式で情報をキャプチャする

HTML、埋め込み画像 (ローカルやパブリック URL にある)、ビデオ、オーディオ、メール メッセージ、その他の一般的なファイル タイプをキャプチャします。 OneNote では、Web ページや PDF ファイルをスナップショットとして表示することもできます。 Microsoft Graph は、OneNote ページ レイアウト用に標準 HTML および CSS のセットをサポートします。そのため、表、インライン イメージ、基本書式を使用して思いどおりの外観を実現できます。 

### <a name="use-the-onenote-ecosystem-to-enhance-your-core-scenarios"></a>OneNote エコシステムを使用して、コア シナリオを強化する

その他の強力な OneNote の機能を利用できます。 この Microsoft Graph の OneNote API では、イメージに対する OCR の実行、フルテキスト検索のサポート、クライアントの自動同期、イメージの処理、名刺キャプチャ、オンライン製品一覧やレシピ一覧の抽出などを実行できます。 メモや軽量メディアのクラウドでのデジタル メモリ ストアとして、またはドメイン固有データのデータ フィードとして OneNote を使用します。 

### <a name="reach-millions-of-onenote-users-on-all-major-platforms"></a>すべての主要プラットフォームの数百万人に上る OneNote ユーザーが利用できる


OneNote を使用すると、アプリの使用量が増加します。 OneNote は新しい Windows デバイスにプレインストールされており、ほとんどのプラットフォームでオンライン、および Office 365 の一部として利用可能です。 機能の豊富な OneNote 環境を利用するアプリを公開すると、広範なクロスプラットフォーム市場の潜在的な可能性にアクセスできるようになります。

<!-- Might be good to show a few examples of Microsoft Graph API calls here, similar to what we have in the featured scenarios topic: featured_scenarios..md You could have an H2 section called "What can I do with OneNote APIs in Microsoft Graph?"-->

## <a name="what-can-i-do-with-onenote-apis-in-microsoft-graph"></a>Microsoft Graph の OneNote API で実行できること

OneNote のリソースの操作で最もよく使用される要求の一部を次に示します。

|操作|URL|
|:--------|:--|
|自分のノートブックを取得する|[https://graph.microsoft.com/v1.0/me/onenote/notebooks](https://developer.microsoft.com/graph/graph-explorer?request=me/onenote/notebooks&version=1.0)|
|自分のセクションを取得する|[https://graph.microsoft.com/v1.0/me/onenote/sections](https://developer.microsoft.com/graph/graph-explorer?request=me/onenote/sections&version=1.0)|
|自分のページを取得する|[https://graph.microsoft.com/v1.0/me/onenote/pages](https://developer.microsoft.com/graph/graph-explorer?request=me/onenote/pages&version=1.0)|

## <a name="learn-more-about-onenote-apis"></a>OneNote API に関する詳細情報

OneNote のコンテンツ更新機能については、Microsoft Graph API の詳細情報をご覧ください。 次の一覧の各トピックは、新しい OneNote ページを作成し、既存のページを新しいコンテンツで更新する方法を示しています。 Microsoft Graph を使用した OneNote ノートブックの更新に関するベスト プラクティスも参照してください。 


### <a name="work-with-onenote"></a>OneNote での作業

* [OneNote REST API を使用する](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0)
* [ベスト プラクティス](onenote-best-practices.md)
* [ブランドのガイドライン](onenote-branding.md)
* [OneNote クライアントを開く](open-onenote-client.md)
* [OneNote ページでノート シールを使用する](onenote-note-tags.md)
* [Microsoft Graph の OneNote API のエラー コード](onenote-error-codes.md)

### <a name="work-with-onenote-pages"></a>OneNote ページでの作業

* [OneNote ページの入出力 HTML](onenote-input-output-html.md)
* [Microsoft Graph によって OneNote コンテンツと構造を取得する](onenote-get-content.md)
* [OneNote ページを作成する](onenote-create-page.md)
* [OneNote ページ コンテンツを更新する](onenote-update-page.md)

### <a name="work-with-onenote-page-content"></a>OneNote ページ コンテンツを使用する

* [OneNote ページで絶対配置要素を作成する](onenote-abs-pos.md)
* [OneNote ページに画像、ビデオ、ファイルを追加する](onenote-images-files.md)
* [OneNote API div タグを使用してキャプチャからデータを抽出する](onenote-extract-data.md)

## <a name="see-also"></a>関連項目
OneNote サービス固有の REST エンドポイントにのみ公開されている、OneNote その他の機能の一部について説明します。

- [OneNote の開発](https://docs.microsoft.com/ja-JP/previous-versions/office/office-365-api/how-to/onenote-landing)
- [クラス ノートブックの操作](https://docs.microsoft.com/ja-JP/previous-versions/office/office-365-api/how-to/onenote-classnotebook)
- [非同期クラス ノートブックの操作](https://docs.microsoft.com/ja-JP/previous-versions/office/office-365-api/how-to/onenote-classnotebook-asynchronous)
- [スタッフ ノートブックの操作](https://docs.microsoft.com/ja-JP/previous-versions/office/office-365-api/how-to/onenote-staffnotebook)
- [ノートブック、セクション、ページのコピー](https://docs.microsoft.com/ja-JP/previous-versions/office/office-365-api/how-to/onenote-copy)
- [OneNote エンティティのアクセス許可を管理する](https://docs.microsoft.com/ja-JP/previous-versions/office/office-365-api/how-to/onenote-manage-perms)
- [Web ページで OneNote 保存ダイアログを使用する](https://docs.microsoft.com/ja-JP/previous-versions/office/office-365-api/how-to/onenote-save-dialog)
- [Webhooks の購読](https://docs.microsoft.com/ja-JP/previous-versions/office/office-365-api/how-to/onenote-sync)

## <a name="api-reference"></a>API リファレンス
このサービスの API リファレンスをお探しですか?

- [Microsoft Graph v1.0 の OneNote API](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0)
- [Microsoft Graph ベータ版の OneNote API](/graph/api/resources/onenote-api-overview?view=graph-rest-beta)

## <a name="next-steps"></a>次のステップ

[Microsoft Graph Explorer](https://developer.microsoft.com/graph/graph-explorer) を使用して、自分の OneNote ノートブックで OneNote API を試してみます。

Graph Explorer から OneNote API 呼び出しを行うには、左側の列にある **[その他のサンプルを表示]** を選択します。 メニューを使用して、OneNote を **[オン]** に切り替えます。 また、適切なアクセス許可を有効にする必要があります。 左側のメニューのアカウント名の下で、**[アクセス許可の修正]** を選択します。 OneNote のアクセス許可の詳細については、「[メモのアクセス許可](permissions-reference.md#notes-permissions)」を参照してください。

Microsoft Graph の OneNote API を使い始めるには、[OneNote 参照コンテンツ](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0)に関する記事をご覧ください。

