---
title: アプリの移行計画チェックリスト
description: Azure AD Graph から Microsoft Graph にアプリを移行するためのチェックリスト
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 905a692e6a4fddf71b6488e1695957cba5b182ae
ms.sourcegitcommit: 9cee9d8229fc84dd7ef97670ff27c145e1a78408
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/18/2019
ms.locfileid: "35778265"
---
# <a name="app-migration-planning-checklist"></a>アプリの移行計画チェックリスト

移行を計画するには、次のチェックリストを使用します。

## <a name="step-1-review-the-differences-between-the-apis"></a>手順 1: Api 間の相違点を確認する

多くの点で、Microsoft Graph は以前の Azure AD Graph に似ています。 多くの場合、コード内のエンドポイントサービスの名前とバージョンを変更するだけで、すべてが引き続き機能します。

ただし、違いがあります。 特定のリソース、プロパティ、メソッド、およびコア機能が変更されました。

具体的には、次の領域の相違点を確認します。

- 2つのサービス間の[呼び出し構文の要求](migrate-azure-ad-graph-request-differences.md)
- [機能の相違](migrate-azure-ad-graph-feature-differences.md)(ディレクトリ拡張、バッチ処理、差分クエリなど)
- [エンティティリソース名](migrate-azure-ad-graph-resource-differences.md)とその種類
- 要求オブジェクトと応答オブジェクトの[プロパティ](migrate-azure-ad-graph-property-differences.md)
- パラメーターと型を含む[メソッド](migrate-azure-ad-graph-method-differences.md)

## <a name="step-2-examine-api-use"></a>手順 2: API の使用を調べる

アプリで使用されている Api、必要なアクセス許可、既知の相違点の一覧との比較を[調べ](migrate-azure-ad-graph-audit-api-use.md)ます。  

アプリが必要とする Api が Microsoft Graph v2.0 で一般的に使用可能になっており、これらの Api が同じように動作することを確認します。

場合によっては、新しい機能が以前の方法で置き換えられるように設計されていることがあります。

[Graph エクスプローラー](https://aka.ms/ge)を使用して、新しい通話をテストし、新しいアプローチを開発します。 最良の結果を得るには、テストテナントでテストユーザーの資格情報を使用してサインインし、API が重要なデータセットを処理する内容を確認します。

## <a name="step-3-review-app-details"></a>手順 3: アプリの詳細を確認する

- [アプリの登録](migrate-azure-ad-graph-app-registration.md)と同意の変更 (none である必要があります)。
- トークンの取得と[認証のライブラリ](migrate-azure-ad-graph-authentication-library.md)。
- .NET アプリケーションの場合、[クライアントライブラリ](migrate-azure-ad-graph-client-libraries.md)を使用します。

## <a name="step-4-deploy-test-and-extend-your-app"></a>手順 4: アプリの展開、テスト、拡張

すべてのユーザーに対してアプリを更新する前に、十分にテストして、お客様の対象者にロールアウトすることを確認してください。

Microsoft Graph への切り替えが完了したので、すぐに使用できるようになるデータセットや機能の多くは、すぐにロック解除することができなくなりました。 いくつかの[例](/graph/examples)を見て、考えられることを知ることができます。

現在[AD 認証ライブラリ](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-libraries)(ADAL) を使用している場合は、 [Microsoft 認証ライブラリ](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries)(msal) に切り替えることを検討してください。

## <a name="next-steps"></a>次のステップ

- [Resquest 呼び出し構文](migrate-azure-ad-graph-request-differences.md)について説明し、「手順 1: API の違いを確認する」を開始します。
- [Microsoft Graph](/graph/overview)の概念とプラクティスについて説明します。
- [Graph エクスプローラー](https://aka.ms/ge)を使用して、Microsoft graph を試してみてください。
- 進捗状況の更新とタイムラインの詳細については、「 [Microsoft Graph」または「AZURE AD Graph](https://dev.office.com/blogs/microsoft-graph-or-azure-ad-graph) In The Office デベロッパーセンター」を参照してください。
