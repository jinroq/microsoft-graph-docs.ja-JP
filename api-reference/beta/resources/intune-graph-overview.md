---
title: Intune Graph API の使用
description: " Intune ハイブリッド展開はサポートされていません。 "
ms.openlocfilehash: 2502b5209e9935fc923570947c38c0467534f4ef
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071319"
---
# <a name="working-with-intune-in-microsoft-graph"></a>Microsoft Graph での Intune の操作  

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing)を持っている必要があります。

Intune 用 Microsoft Graph API を使用すると、テナントの Intune の情報へのプログラムによるアクセスが可能となります。API は **Azure Portal** で使用できるものと同じ Intune 操作を実行します。  

モバイル デバイス管理 (MDM) のシナリオの場合、Intune 用 Graph API はスタンドアロンの展開をサポートします。Intune の[ハイブリッド展開](https://docs.microsoft.com/en-us/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management)はサポートされていません。 

## <a name="using-the-intune-graph-api"></a>Intune Graph API の使用

Intune は、他のクラウド サービスには、エンティティの豊富な情報との関係のナビゲーションを使用して、データをグラフと同じ方法で提供します。Intune IT プロフェッショナルやエンドユーザーのサービス間の豊富なアプリケーションを構築するのに他のサービスから情報を結合するのにには、Microsoft Graph を使用します。     

以下に、アプリケーションがユーザーのデバイスにインストールされているかどうかを判断する方法の例を示します。 

1. Azure Active Directory から、ユーザーに登録されているデバイスのリストを取得します。 

    https://graph.microsoft.com/beta/users/{user}/ownedDevices 

2. 次に、テナントのアプリケーションのリストを表示します。 

    https://graph.microsoft.com/beta/deviceAppManagement/mobileApps  

3. アプリケーションから ID を取得し、アプリケーション (そしてユーザー) のインストール状態を確認します。

    https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{id}/deviceStatuses/


## <a name="using-graph-permission-scopes"></a>グラフのためのアクセス許可のスコープを使用します。

Microsof のグラフでは、アクセス許可のスコープを使用するリソースへのアクセスを制御します。 開発者は、Intune リソースにアクセスするために必要となる、アクセス許可のスコープを指定する必要があります。 通常は Azure Active Directory ポータルで必要なアクセス許可のスコープを指定します。 詳細については、「[Microsoft Graph のアクセス許可スコープ](https://developer.microsoft.com/graph/docs/authorization/permission_scopes)」および「[Intune のアクセス許可のスコープ](https://developer.microsoft.com/graph/docs/authorization/permission_scopes#permission-scopes-in-preview)」を参照してください。

## <a name="to-use-the-table-of-contents-on-the-microsoft-graph-site"></a>Graph のサイトの内容のテーブルを使用するには
  
Intune グラフ API とリソースを表示するドキュメントのパーツを検索する (サイトの左側のペイン) の目次を参照できます。

1. ベータ版ドキュメントを開くには、 **/Beta 参照**をクリックします。
2. 下にスクロールし、 **Intune**] をクリックします。
3. API の部分の**Intune**の下のサブセクションをクリックします。 
