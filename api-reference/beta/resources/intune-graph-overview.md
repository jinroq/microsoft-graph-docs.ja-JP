---
title: Intune Graph API の使用
description: " Intune ハイブリッド展開はサポートされていません。 "
author: tfitzmac
ms.openlocfilehash: cecce61dba0ddfc044c2e06e0e16d68401fcafb5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27357247"
---
# <a name="working-with-intune-in-microsoft-graph"></a>Microsoft Graph での Intune の操作  

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing)を持っている必要があります。

Intune 用 Microsoft Graph API を使用すると、テナントの Intune の情報へのプログラムによるアクセスが可能となります。API は **Azure Portal** で使用できるものと同じ Intune 操作を実行します。  

モバイル デバイス管理 (MDM) の場合は、Intune の Microsoft グラフ API は、スタンドアロン導入をサポートしています。Intune[ハイブリッド展開](https://docs.microsoft.com/en-us/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management)はサポートされていません。 

## <a name="using-the-microsoft-graph-api-for-intune"></a>Intune の Graph API を使用します。

Intune は、他のクラウド サービスには、エンティティの豊富な情報との関係のナビゲーションを使用して、データをグラフと同じ方法で提供します。Intune IT プロフェッショナルやエンドユーザーのサービス間の豊富なアプリケーションを構築するのに他のサービスから情報を結合するのにには、Microsoft Graph を使用します。     

次の使用例は、アプリケーションがユーザーのデバイスにインストールされているかどうかを判断する方法を示しています。 

1. Azure Active Directory から、ユーザーに登録されているデバイスのリストを取得します。 

    https://graph.microsoft.com/beta/users/{user}/ownedDevices 

2. 次に、テナントのアプリケーションのリストを表示します。 

    https://graph.microsoft.com/beta/deviceAppManagement/mobileApps  

3. アプリケーションから ID を取得し、アプリケーション (そしてユーザー) のインストール状態を確認します。

    https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{id}/deviceStatuses/


## <a name="using-microsoft-graph-permissions"></a>Graph のアクセス許可を使用します。

Microsof のグラフでは、アクセス許可を使用してリソースへのアクセスを制御します。 開発者は、Intune リソースにアクセスするアクセス許可を指定してください。 通常、Active Directory の Azure ポータルのアクセス許可を指定します。 詳細については、 [Microsoft Graph のアクセス許可のリファレンス](https://docs.microsoft.com/en-us/graph/permissions-reference)を参照してください。

## <a name="next-steps"></a>次のステップ

- Intune の Microsoft グラフ API にアクセスするのには[Azure AD を使用する方法](https://docs.microsoft.com/en-us/intune/intune-graph-apis)について説明します。  
- Intune の作業例のコンテキストで Microsoft グラフ API を使用する方法を表示する[PowerShell Intune のサンプル](https://github.com/microsoftgraph/powershell-intune-samples)を表示します。

