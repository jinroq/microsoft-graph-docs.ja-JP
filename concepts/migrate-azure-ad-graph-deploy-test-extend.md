---
title: 移行したアプリの展開、テスト、拡張
description: 'Microsoft Graph API (REST) を使用するように Azure Active Directory (Azure AD) アプリを移行する方法について説明します。ここでは、手順 3: 展開、テスト、拡張について説明します。'
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f8a63c14ef27648a1d586551ebe12e18a5f263a9
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33630252"
---
# <a name="deploy-test-and-extend"></a>展開、テスト、拡張

これは、[アプリを移行するプロセス](migrate-azure-ad-graph-planning-checklist.md)の手順4です。

1.  **テスト方法**

    アプリを更新したら、十分にテストして、予期したとおりに動作することと、回帰がまったく導入されていないことを確認してください。  

    複数の環境、データセット、およびエンドユーザーのペルソナ (たとえば、異なる役割、権利、および責任を持つ資格情報) を使用していることを確認してください。 新しいテストユーザーが初めてアプリを取得し、既存のユーザー (既に同意しているユーザー) がアプリを再度使用しようとしたときに、ライフサイクル全体を参照します。

2.  **段階的な更新プログラムを展開する**

    更新プログラムを段階的に展開することを検討してください。  少数のフレンドリユーザーに限定されたロールアウトは、やっかいの問題やその他の潜在的な問題を特定するのに役立ちます。  これにより、初期の受信やフィードバックを監視することもできます。

    初期ロールアウトがうまくいく場合は、より多くのユーザーに展開するときの進行状況を監視します。

3.  **新しい値を探す**

    Microsoft Graph への切り替えが完了したので、すぐに使用できるようになるデータセットや機能の多くは、すぐにロック解除することができなくなりました。 定期的に新しいデータセットと機能をチェックします。  

    - [Microsoft Graph で可能なこと](/graph/examples)を確認する
    - Microsoft graph に関する最新ニュース、およびいくつかの豊富な学習シリーズについては、 [Microsoft graph のブログ](/graph/blogs)を参照してください。
    - [Changelog](/greaph/changelog)は、サービスおよびドキュメントの更新を要約します。 これらの更新プログラムをフォローすると、ベータ版 (プレビュー) と v2.0 (GA) に昇格した新しい Api を追跡するのに役立ちます。  これらの新しい Api は、より多くの価値と新しいエクスペリエンスをアプリに追加するための新しい方法を提供します。  

## <a name="see-also"></a>関連項目

移行プロセスで問題が発生したり、ヘルプが必要になった場合は、次の操作を実行できます。

- [チェックリスト](migrate-azure-ad-graph-overview.md)をもう一度確認する
- [Stackoverflow](https://stackoverflow.com/questions/tagged/microsoft-graph)に質問を投稿する
- Microsoft Graph サンプルを見直して、既存のアプリケーションコードと比較します。
  - **REST API を使用するアプリ**:[クイックスタートとサンプル](/graph/get-started)を参照して、選択したプラットフォームを選択し、クイックスタートで実行するか、適切なサンプルを検索します。
  - **.Net クライアントライブラリを使用するアプリ**: レビュー[コンソール-サンプル](https://github.com/microsoftgraph/console-csharp-snippets-sample)、または[dotnetcore-console](https://github.com/microsoftgraph/dotnetcore-console-sample) -サンプル

## <a name="next-steps"></a>次のステップ

- [クイックスタートとサンプル](/graph/get-started)を使用すると、短時間ですばやく開始できます。
- [クライアントライブラリと sdk](https://developer.microsoft.com/graph/get-started)を活用してカスタムアプリケーションを開発する 
- [Microsoft Graph](/graph/overview)の概念とプラクティスについて説明します。
- [Graph エクスプローラー](https://aka.ms/ge)を使用して、Microsoft graph を試してみてください。
