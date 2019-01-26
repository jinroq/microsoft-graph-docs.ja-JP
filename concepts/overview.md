---
title: Microsoft Graph の概要
description: Microsoft Graph は、Microsoft 365 のデータとインテリジェンスにアクセスするための入り口です。 Microsoft Graph は、Office 365、Enterprise Mobility + Security、および Windows 10 の大量のデータを活用するために使用できる統合型プログラミング モデルを提供します。
author: jthake-msft
localization_priority: Priority
ms.openlocfilehash: b8256cebe9e8e706a655221c3e1acc5947f9eecd
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573712"
---
# <a name="overview-of-microsoft-graph"></a>Microsoft Graph の概要

Microsoft Graph は、Microsoft 365 のデータとインテリジェンスにアクセスするための入り口です。 Microsoft Graph は、Office 365、Enterprise Mobility + Security、および Windows 10 の大量のデータを活用するために使用できる統合型プログラミング モデルを提供します。 

Microsoft Graph API を使用して、数百万人のユーザーのデータを操作する組織やコンシューマー向けのアプリを作成できます。 Microsoft Graph では、1 つのエンドポイント (`https://graph.microsoft.com`) を介して豊富なリソース、リレーションシップ、およびインテリジェンスのすべてに接続できます。

## <a name="whats-in-the-graph"></a>Graph の内容
Microsoft Graph は、次のデータにアクセスするための REST API とクライアント ライブラリを公開しています。

- Azure Active Directory
- Office 365 サービス: SharePoint、OneDrive、Outlook/Exchange、Microsoft Teams、OneNote、Planner、および Excel
- Enterprise Mobility + Security サービス: Identity Manager、Intune、Advanced Threat Analytics、および Advanced Threat Protection。
- Windows 10 サービス: アクティビティとデバイス
- 教育

詳細については、「[Microsoft Graph の主要なサービスおよび機能](overview-major-services.md)」を参照してください。

Microsoft Graph は、リレーションシップを使用してこれらのサービス間ですべてのリソースを接続します。 たとえば、ユーザーは [memberOf](/graph/api/user-list-memberof?view=graph-rest-1.0) リレーションシップを介してグループに接続したり、[manager](/graph/api/user-list-manager?view=graph-rest-1.0) リレーションシップを介して別のユーザーに接続したりできます。 アプリはこれらのリレーションシップをスキャンして、これらの接続されたリソースにアクセスし、API を介してそれらのアクションを実行することができます。

また、Microsoft Graph のデータに関する貴重なインサイトとインテリジェンスを得ることもできます。 たとえば、特定のユーザーに人気のあるファイルを[人気上昇中](/graph/api/resources/insights-trending?view=graph-rest-beta)にしたり、ユーザーに最も関連性の高い[人物](/graph/api/user-list-people?view=graph-rest-beta)を取得したりできます。

Microsoft Graph のリレーションシップが持つ可能性を見つけてください。

![Graph の一部である主要なリソースとリレーションシップを示すイメージ](images/microsoft-graph.png)

## <a name="what-can-you-do-with-microsoft-graph"></a>Microsoft Graph でできること 

Microsoft Graph を使用すると、ユーザーの固有のコンテキストに関するエクスペリエンスを構築し、生産性を高めることができます。次のアプリを想像してみてください。

- 出席者にプロファイル情報を提供することで、次の会議の調査や準備に役立ちます。情報には、出席者の役職や仕事仲間、作業中の最新のドキュメントやプロジェクトに関する情報などが含まれます。
- 予定表をスキャンして、次のチームミーティングに最適な時間を提案します。
- OneDrive の Excel ファイルから最新の売上予測チャートを取得し、リアルタイムで予測を更新します。これらをすべて携帯電話から行います。
- 予定表の変更に対応し、会議に時間がかかりすぎているときに警告を送信したり、出席者との関連度に基づいて、見逃しや委任が可能な会議を提示したりします。
- たとえば、個人の OneDrive に送信する必要のある写真と OneDrive for Business に送信する必要のあるビジネスの領収書を分類するなどにより、携帯電話で個人情報や仕事情報を整理するのに役立ちます。

Microsoft Graph API を使用すると、これ以上のことができます。

>**注:** Microsoft Graph API を使用する場合、「[Microsoft Graph 使用条件](https://developer.microsoft.com/graph/docs/misc/terms-of-use)」と「[Microsoft のプライバシーに関する声明](https://go.microsoft.com/fwlink/?LinkId=521839)」に同意することになります。

### <a name="popular-requests"></a>一般的な要求

Microsoft Graph API を使用するための一般的なシナリオをいくつか確認します。 リンクから [Graph エクスプローラー](https://developer.microsoft.com/graph/graph-explorer)に移動できます。

| **操作** | **URL** |
|:--------------------------|:----------------------------------------|
|   自分のプロファイルの取得 |    [`https://graph.microsoft.com/v1.0/me`](https://developer.microsoft.com/graph/graph-explorer/?request=me&version=v1.0) |
|   自分のファイルの取得 | [`https://graph.microsoft.com/v1.0/me/drive/root/children`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fdrive%2Froot%2Fchildren&version=v1.0) |
|   自分の写真の取得	 | [`https://graph.microsoft.com/v1.0/me/photo/$value`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fphoto%2F%24value&version=v1.0) |
|   自分のメールの取得 |   [`https://graph.microsoft.com/v1.0/me/messages`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fmessages&version=v1.0) |
|   自分にとって重要度の高いメールの取得 | [`https://graph.microsoft.com/v1.0/me/messages?$filter=importance%20eq%20'high'`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fmessages%3F%24filter%3Dimportance%2520eq%2520'high'&version=v1.0) |
|   自分の予定表イベントの取得 |    [`https://graph.microsoft.com/v1.0/me/events`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fevents&version=v1.0) |
|   自分の上司の取得  | [`https://graph.microsoft.com/v1.0/me/manager`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fmanager&version=v1.0) |
|   foo.txt ファイルを最後に変更したユーザーの取得 |  [`https://graph.microsoft.com/v1.0/me/drive/root/children/foo.txt/lastModifiedByUser`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fdrive%2Froot%2Fchildren%2Ffoo.txt%2FlastModifiedByUser&version=v1.0) |
|   自分がメンバーになっている Office365 グループの取得| [`https://graph.microsoft.com/v1.0/me/memberOf/$/microsoft.graph.group?$filter=groupTypes/any(a:a%20eq%20'unified')`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2FmemberOf%2F%24%2Fmicrosoft.graph.group%3F%24filter%3DgroupTypes%2Fany(a%3Aa%2520eq%2520'unified')&version=v1.0) |
|   自分の所属組織のユーザーの取得     | [`https://graph.microsoft.com/v1.0/users`](https://developer.microsoft.com/graph/graph-explorer/?request=users&version=v1.0) |
|   自分の組織内のグループの取得 | [`https://graph.microsoft.com/v1.0/groups`](https://developer.microsoft.com/graph/graph-explorer/?request=groups&version=v1.0) |
|   自分に関連付けられたユーザーの取得    | [`https://graph.microsoft.com/v1.0/me/people`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fpeople&version=beta)  |
|   自分の周りで人気上昇中の項目の取得 |  [`https://graph.microsoft.com/beta/me/insights/trending`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Finsights%2Ftrending&version=beta) |
|   自分のノートの取得 |  [`https://graph.microsoft.com/v1.0/me/onenote/notebooks`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fonenote%2Fnotebooks&version=beta) |

## <a name="access-microsoft-graph-at-scale"></a>Microsoft Graph への大量アクセス


Microsoft Graph データ接続では、Office 365 のデータに対して、従来のトランザクション単位ではなく一括でのアクセスが可能です。 Office 365 のバルク データでは、Azure ツールを使用して、次を実行するインテリジェントなアプリを構築できます。

- 組織内にいる、あなたのトピックに関する専門家で、場所が最も近い人を探す 
- ナレッジ ベース作成を自動化する
- 会議室の使用状況に関する洞察を得るために、会議出席依頼を分析する
- 生産性および通信のデータから不正行為を検出する

## <a name="when-should-i-use-microsoft-graph-data-connect"></a>Microsoft Graph データ接続を使用するタイミング

Microsoft Graph データ接続は、Microsoft Graph API を通じて利用可能なデータとやりとりする新たな方法を提供します。 Office 365 データへのスケーラブルなアクセスの提供に加え、Microsoft Graph データ接続は、インテリジェントなアプリケーションの構築を効率化する独自の各種機能を備えています。これらの機能はすべて Microsoft クラウド内で使用できます。

|**機能**| **Microsoft Graph API** | **Microsoft Graph データ接続** |
|:----------|:------------------------|:--------------------------------------|
| **アクセス スコープ** | 1 人のユーザーまたはテナント全体 | 多数のユーザーまたはグループ |
| **アクセス パターン** | リアルタイム | 定期的なスケジュール |
| **データ操作** | データ マスターに対する操作 | データのキャッシュに対する操作 |
| **データ保護** | データは Microsoft 365 内にある間は保護される | データ保護対象は Azure サブスクリプション内のデータのキャッシュにも拡大される |
| **ユーザーの同意** | 自分<br>リソースの種類 | なし |
| **管理者の同意** | 組織全体<br>リソースの種類 | ユーザーのグループを選択<br>リソースの種類とプロパティ<br>ユーザーを除外 |
| **アクセス ツール** | RESTful Web クエリ | Azure Data Factory |

Microsoft Graph データ接続の詳細については、[Microsoft Graph データ接続](data-connect-overview.md)を参照してください。 使用を開始するには、[Microsoft Graph データ接続の概要](data-connect-concept-overview.md)を参照してください。 

## <a name="next-steps"></a>次のステップ

- [おすすめのシナリオ](https://developer.microsoft.com/graph/examples)を確認します。
- [Graph エクスプローラー](https://developer.microsoft.com/graph/graph-explorer)でサンプルの要求を試します。
- [クイック スタート](https://developer.microsoft.com/graph/quick-start)を使用して、すぐに実行できるサンプル アプリをセットアップします。
- 目次の「**詳細情報**」を見て、さまざまなシナリオで使用できるサービスや機能についての詳細情報を参照します。 
- アプリで[認証トークンを取得する](auth-overview.md)方法を検索します。
- [API の使用](use-the-api.md)を開始します。


