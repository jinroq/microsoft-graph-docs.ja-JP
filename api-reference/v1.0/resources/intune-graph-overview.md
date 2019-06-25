---
title: Intune Graph API の使用
description: " Intune ハイブリッド展開はサポートされていません。 "
author: tfitzmac
localization_priority: Priority
ms.prod: intune
ms.openlocfilehash: 0c30436c80af8621b1c633d12a11489f7e586f00
ms.sourcegitcommit: 7c03131291113c343a98bb0234d31bd4535a4050
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/22/2019
ms.locfileid: "35133853"
---
# <a name="working-with-intune-in-microsoft-graph"></a>Microsoft Graph での Intune の操作  

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing)を持っている必要があります。

Intune 用 Microsoft Graph API を使用すると、テナントの Intune の情報へのプログラムによるアクセスが可能となります。API は **Azure Portal** で使用できるものと同じ Intune 操作を実行します。  

モバイル デバイス管理 (MDM) のシナリオの場合、Intune 用 Microsoft Graph API はスタンドアロンの展開をサポートします。Intune の[ハイブリッド展開](https://docs.microsoft.com/ja-JP/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management)はサポートされていません。 

## <a name="using-the-microsoft-graph-api-for-intune"></a>Intune 用 Microsoft Graph API の使用

Intune は、豊富なエンティティ情報とリレーションシップのナビゲーションを使用して、他のクラウド サービスと同じ方法で Microsoft Graph API にデータを提供します。 Microsoft Graph API を使用して、他のサービスからの情報と Intune を結合し、IT プロフェッショナルやエンド ユーザー向けの豊富なサービス間アプリケーションをビルドします。     

以下に、アプリケーションがユーザーのデバイスにインストールされているかどうかを判断する方法の例を示します。 

1. Azure Active Directory から、ユーザーに登録されているデバイスのリストを取得します。 

    https://graph.microsoft.com/users/{user}/ownedDevices 

2. 次に、テナントのアプリケーションのリストを表示します。 

    https://graph.microsoft.com/deviceAppManagement/mobileApps  

3. アプリケーションから ID を取得し、アプリケーション (そしてユーザー) のインストール状態を確認します。

    https://graph.microsoft.com/deviceAppManagement/mobileApps/{id}/deviceStatuses/

## <a name="accessing-the-microsoft-graph-api-for-intune"></a>Intune 用 Microsoft Graph API へのアクセス

Intune は、[委任されたアクセス許可](https://docs.microsoft.com/graph/auth-v2-user)と[アプリケーションのアクセス許可](https://docs.microsoft.com/graph/auth-v2-service)の両方をサポートします。 委任されたアクセス許可は、読み取り操作と書き込み操作の両方でサポートされています。 アプリケーションのアクセス許可は、現在、読み取り操作でのみサポートされています。 委任されたアクセス許可およびアプリケーションのアクセス許可は、シングル テナント アプリケーションおよびマルチテナント アプリケーションの両方をサポートします。 Microsoft Graph で使用できるアクセス許可の詳細については、「[Microsoft Graph のアクセス許可のリファレンス](https://docs.microsoft.com/graph/permissions-reference)」を参照してください。

## <a name="using-permissions"></a>アクセス許可の使用

Microsoft Graph API は、アクセス許可によってリソースへのアクセスを制御します。 開発者は、Intune リソースにアクセスするために必要となるアクセス許可を指定する必要があります。 通常は Azure Active Directory ポータルでアクセス許可を指定します。 詳細については、「[Microsoft Graph のアクセス許可リファレンス](https://docs.microsoft.com/ja-JP/graph/permissions-reference)」を参照してください。

## <a name="next-steps"></a>次のステップ

- Microsoft Graph の Intune API に [Azure AD を使用してアクセスする方法](https://docs.microsoft.com/ja-JP/intune/intune-graph-apis)について確認します。  
- [PowerShell Intune サンプル](https://github.com/microsoftgraph/powershell-intune-samples)について調べます。これは、サンプルを操作しながら Intune 用 Microsoft Graph API の使用方法を示します。
