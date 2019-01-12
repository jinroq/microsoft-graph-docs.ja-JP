---
title: Microsoft Graph データ接続の開始 (プレビュー)
description: 'Microsoft Graph データ接続を使用する前に、Office 365 管理者は 2 つの処理を行う必要があります。どちらも、管理者が Privileged Access Management (PAM) を通じてデータ移動を制御する機能を有効にします。 '
author: ajacks-msft
localization_priority: Priority
ms.prod: data-connect
ms.openlocfilehash: f7426147908a2ded298bee065c05afffc182cd4b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914445"
---
# <a name="get-started-with-microsoft-graph-data-connect-preview"></a>Microsoft Graph データ接続の開始 (プレビュー)

Microsoft Graph データ接続を使用する前に、Office 365 管理者は 2 つの処理を行う必要があります。どちらも、管理者が Privileged Access Management (PAM) を通じてデータ移動を制御する機能を有効にします。 

1. Microsoft 365 管理ポータルの **[サービスとアドイン]** ページを通じて、Microsoft Graph データ接続にオプトインすることに同意します。 これにより、Microsoft Azure へのデータ移動要求が許可されます (つまり、データのフル コントロール権は保持されたまま、Azure リソースからのアクセスが許可されます)。 特定のパイプラインに対する承認が後で行われないかぎり、データは転送されません。
2. Office 365 サブスクリプションの承認者グループを設定します。 承認者グループが空でないことを確認します。 グループ内のユーザーのみが、データ移動要求を承認できます。

詳細なステップバイステップの手順については、[Microsoft Graph データ接続のトレーニング モジュール](https://github.com/microsoftgraph/msgraph-training-dataconnect/blob/master/Lab.md)を参照してください。

## <a name="next-steps"></a>次のステップ

おめでとうございます。 Azure のツールを使用してインテリジェントなアプリケーションの構築を開始する準備が整いました。 サンプル アプリケーションと追加のドキュメントについては、[Microsoft Graph データ接続の GitHub レポ](https://github.com/OfficeDev/MS-Graph-Data-Connect/wiki)を参照してください。 
