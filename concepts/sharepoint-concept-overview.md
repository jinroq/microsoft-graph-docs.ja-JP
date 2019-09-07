---
title: SharePoint のサイトおよびコンテンツ API の概要
description: SharePoint は、インテリジェントなモバイル イントラネットです。 SharePoint によりユーザーは、コンテンツ、知識、アプリケーションを共有および管理して、チームワークを推進したり、情報を検索したり、組織を通じて共同作業をしたりできます。 Microsoft Graph で SharePoint REST API を使用することにより、ソリューションを SharePoint のサイトおよびコンテンツに統合することができます。
localization_priority: Priority
ms.prod: sharepoint
scenarios: getting-started
ms.openlocfilehash: 38d9b0973c1d3f1ee9c7fb0e58129d675d674955
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/07/2019
ms.locfileid: "36792878"
---
# <a name="sharepoint-sites-and-content-api-overview"></a>SharePoint のサイトおよびコンテンツ API の概要

SharePoint は、インテリジェントなモバイル イントラネットです。 SharePoint によりユーザーは、コンテンツ、知識、アプリケーションを共有および管理して、チームワークを推進したり、情報を検索したり、組織を通じて共同作業をしたりできます。 Microsoft Graph で SharePoint REST API を使用することにより、ソリューションを SharePoint のサイトおよびコンテンツに統合することができます。

## <a name="why-integrate-with-sharepoint-sites-and-content"></a>SharePoint のサイトおよびコンテンツを統合する理由

SharePoint のサイトは、チームのコラボレーションとコミュニケーションを強化します。 Office 365 のグループ、Microsoft Teams、およびポータルは、すべて SharePoint に基づいているため、Microsoft Graph を使用することにより、保存場所に関係なくデータにアクセスすることができます。 Microsoft Graph で SharePoint API を使用することにより、次のものにアクセスできます:

- ユーザーが同僚と共同作業するコンテンツを保存するチーム サイト。
- ユーザーが、情報豊富なコンテンツ ページを組織内で共有するために公開する場所となるコミュニケーション サイトおよびポータル。

### <a name="unleash-your-data-with-sharepoint-lists"></a>SharePoint のリストによりデータを最大限活用する

[リスト][リスト]は、SharePoint におけるデータ ストレージの基盤となるものです。
[リストを作成][作成]して、シンプルな顧客連絡先リストからカスタム ビジネス アプリケーションに至るまで、さまざまなビジネス データを保存します。フロントエンドとして PowerApps が使用されます。
[列][]を使用してスキーマを定義すると、SharePoint により、そのデータの整合性が保護され、インデックス作成、クエリ、検索の豊富な機能が提供されます。

### <a name="bring-the-power-of-lists-to-your-teams-files"></a>チームのファイルにリストの強力な機能を提供

SharePoint は、ドキュメント ライブラリと呼ばれる特殊な[リスト タイプ][]にファイルを保存します。
[OneDrive API][] を使用することにより 1 つの[ドライブ][]としてライブラリを操作したり、SharePoint API を使用することにより[リスト][]として操作したりできます。
通常のリストと同じように、ドキュメント ライブラリのスキーマを拡張して、カスタム列によりビジネス ニーズをサポートすることができます。

### <a name="light-up-your-app-with-your-users-sharepoint-intranet-data"></a>ユーザーの SharePoint イントラネット データによりアプリをライトアップ

Microsoft Graph により、ユーザーにとって最も重要なデータをアプリ内の前面に打ち出すことができます。
ユーザーのデータを保存したリストに対する[クエリ][]により、常に最新の状態を保ちます。
アプリのための独自のリストを[作成][]し、ユーザーが他の SharePoint エクスペリエンスでそのデータにアクセスするようにしたり、あるいは一切を非表示にしたりします。

### <a name="use-microsoft-graph-to-extend-sharepoint"></a>Microsoft Graph を使用して SharePoint を拡張する

プラットフォームとして SharePoint は、拡張や統合のためのいくつかのモデルを提供します:

- [SharePoint Framework][] は、SharePoint ページでホスト可能なクライアント サイドのテクノロジおよびオープン ソース ツールを使用して Web パーツを作成する手段を提供します。
- [SharePoint アドイン][]は、カスタム コードをサーバー上で実行することなく SharePoint サイトに追加することのできる自己完結型拡張機能です。

アプリが SharePoint ページ内で実行される際、Microsoft Graph を使用することにより、Office 365 を通じて容易にデータにアクセスすることができます。

それらのモデルに関する詳細については、「[SharePoint デベロッパー センター][]」または「[SharePoint 開発者向けドキュメント][]」を参照してください。

## <a name="api-reference"></a>API リファレンス
このサービスの API リファレンスをお探しですか?

- [Microsoft Graph v1.0 の SharePoint API](/graph/api/resources/sharepoint?view=graph-rest-1.0)
- [Microsoft Graph ベータ版の SharePoint API](/graph/api/resources/sharepoint?view=graph-rest-beta)

## <a name="next-steps"></a>次の手順

Microsoft Graph の SharePoint を利用する手始めとして、[サイトの使用](/graph/api/resources/sharepoint?view=graph-rest-1.0)についてご確認ください。

[list]: /graph/api/resources/list?view=graph-rest-1.0
[列]: /graph/api/resources/columndefinition?view=graph-rest-1.0
[リスト タイプ]: /graph/api/resources/listinfo?view=graph-rest-1.0
[作成]: /graph/api/list-create?view=graph-rest-1.0
[クエリ]: /graph/api/listitem-get?view=graph-rest-1.0
[ドライブ]: /graph/api/resources/drive?view=graph-rest-1.0
[OneDrive API]: /graph/api/resources/onedrive?view=graph-rest-1.0
[SharePoint Framework]: https://docs.microsoft.com/sharepoint/dev/spfx/sharepoint-framework-overview
[SharePoint アドイン]: https://docs.microsoft.com/sharepoint/dev/sp-add-ins/sharepoint-add-ins
[SharePoint デベロッパー センター]: https://developer.microsoft.com/sharepoint
[SharePoint 開発者向けドキュメント]: https://aka.ms/spdev-docs
[SharePoint]: /graph/api/resources/sharepoint?view=graph-rest-1.0
