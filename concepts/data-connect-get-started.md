---
title: Microsoft Graph データ接続を始める
description: 'Microsoft Graph データ接続を使用する前に、Office 365 管理者は 2 つの処理を行う必要があります。どちらも、管理者が Privileged Access Management (PAM) を通じてデータ移動を制御する機能を有効にします。 '
author: ajacks-msft
localization_priority: Priority
ms.prod: data-connect
ms.openlocfilehash: 8372653d8904ba247975a649e6709b2206a4d6d3
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33599787"
---
# <a name="get-started-with-microsoft-graph-data-connect"></a>Microsoft Graph データ接続を始める

Microsoft Graph データ接続を使用する前に、Office 365 管理者は 2 つの処理を行う必要があります。どちらも、管理者が Privileged Access Management (PAM) を通じてデータ移動を制御する機能を有効にします。 

1. Microsoft 365 管理ポータルの **[サービスとアドイン]** ページを通じて、Microsoft Graph データ接続にオプトインすることに同意します。 これにより、Microsoft Azure へのデータ移動要求が許可されます (つまり、データのフル コントロール権は保持されたまま、Azure リソースからのアクセスが許可されます)。 特定のパイプラインに対する承認が後で行われないかぎり、データは転送されません。
2. Office 365 サブスクリプションの承認者グループを設定します。 承認者グループが空でないことを確認します。 グループ内のユーザーのみが、データ移動要求を承認できます。

## <a name="next-steps"></a>次の手順

おめでとうございます。 Azure のツールを使用してインテリジェントなアプリケーションの構築を開始する準備が整いました。 手順の詳細については、[Microsoft Graph データ接続のトレーニング モジュール](https://github.com/microsoftgraph/msgraph-training-dataconnect/blob/master/Lab.md)を参照してください。 Microsoft Graph データ接続の機能の詳細については、[データセット、区域、およびシンク](/concepts/data-connect-datasets.md) または、データ接続がサポートする [ユーザー選択とフィルター処理](/concepts/data-connect-filtering.md)を参照してください。 
