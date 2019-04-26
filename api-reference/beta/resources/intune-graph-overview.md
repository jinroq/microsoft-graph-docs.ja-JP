---
title: Intune Graph API の使用 - Microsoft Graph API
description: テナント組織、そのデバイス、アプリ、アクセス、リソースを管理するために使用できる、Intune エンドポイント用 Microsoft Graph API (REST) の一覧を示します。
author: tfitzmac
localization_priority: Priority
ms.prod: intune
ms.openlocfilehash: fc254772a5b4db131a5cda45fc83b336bf12f993
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32575962"
---
# <a name="working-with-intune-in-microsoft-graph"></a>Microsoft Graph での Intune の操作  

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでは、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://www.microsoft.com/ja-JP/cloud-platform/microsoft-intune-pricing)を持っている必要があります。

Intune 用 Microsoft Graph API を使用すると、テナントの Intune の情報へのプログラムによるアクセスが可能となります。API は **Azure Portal** で使用できるものと同じ Intune 操作を実行します。  

モバイル デバイス管理 (MDM) のシナリオの場合、Intune 用 Microsoft Graph API はスタンドアロンの展開をサポートします。Intune の[ハイブリッド展開](https://docs.microsoft.com/ja-JP/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management)はサポートされていません。 

## <a name="using-the-microsoft-graph-api-for-intune"></a>Intune 用 Microsoft Graph API の使用

Intune は、豊富なエンティティ情報とリレーションシップのナビゲーションを使用して、他のクラウド サービスと同じ方法で Microsoft Graph にデータを提供します。 Microsoft Graph を使用して、他のサービスからの情報と Intune を結合し、IT プロフェッショナルやエンド ユーザー向けの豊富なサービス間アプリケーションをビルドします。     

以下に、アプリケーションがユーザーのデバイスにインストールされているかどうかを判断する方法の例を示します。 

1. Azure Active Directory から、ユーザーに登録されているデバイスのリストを取得します。 

    https://graph.microsoft.com/beta/users/{user}/ownedDevices 

2. 次に、テナントのアプリケーションのリストを表示します。 

    https://graph.microsoft.com/beta/deviceAppManagement/mobileApps  

3. アプリケーションから ID を取得し、アプリケーション (そしてユーザー) のインストール状態を確認します。

    https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{id}/deviceStatuses/


## <a name="using-microsoft-graph-permissions"></a>Microsoft Graph アクセス許可の使用

Microsoft Graph では、アクセス許可によってリソースへのアクセスを制御します。 開発者は、Intune リソースにアクセスするために必要となるアクセス許可を指定する必要があります。 通常は Azure Active Directory ポータルでアクセス許可を指定します。 詳細については、「[Microsoft Graph のアクセス許可リファレンス](https://docs.microsoft.com/ja-JP/graph/permissions-reference)」を参照してください。

## <a name="next-steps"></a>次のステップ

- Microsoft Graph の Intune API に [Azure AD を使用してアクセスする方法](https://docs.microsoft.com/ja-JP/intune/intune-graph-apis)について確認します。  
- [PowerShell Intune サンプル](https://github.com/microsoftgraph/powershell-intune-samples)について調べます。これは、サンプルを操作しながら Intune 用 Microsoft Graph API の使用方法を示します。

