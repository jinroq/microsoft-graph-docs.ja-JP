---
title: Intune のデバイスとアプリの API の概要
description: 'Microsoft Intune は、企業が組織内のデバイスとアプリを管理するのに役立ちます。 Microsoft Graph で Intune API を使用して、デバイスとアプリを管理したり、好みのツールを使用しながら Intune を構成したりできます。 '
ms.openlocfilehash: fced71d317aa5f2aebfd2c44237ea9087a6be4f6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092488"
---
# <a name="intune-devices-and-apps-api-overview"></a>Intune のデバイスとアプリの API の概要

Microsoft Intune は、企業が組織内のデバイスとアプリを管理するのに役立ちます。 Microsoft Graph で Intune API を使用して、デバイスとアプリを管理したり、好みのツールを使用しながら Intune を構成したりできます。 

ISV の場合は、Intune API を使用してクライアントのテナントを管理することもできます。

## <a name="why-integrate-with-intune"></a>Intune と統合する理由

Microsoft Graph で Intune API を使用して、Intune のデバイスとアプリに関する情報へのアクセス、デバイスの管理、アプリの管理、および Intune の自動化を行うことができます。

### <a name="manage-devices"></a>デバイスを管理する

Intune API を使用して次の作業を実行できます。

- パスワードの複雑さと期間、暗号化、脅威保護のレベルなどの[デバイス コンプライアンス](/graph/api/resources/intune-deviceconfig-devicecomplianceactionitem?view=graph-rest-1.0) ポリシーを定義し、適用する   (サポートされるポリシーは、オペレーティング システムとバージョンによって異なる)
- デバイスのプラットフォームが Windows、Android、Mac、iOS のどれであるかに関係なく、[企業データを保護](/graph/api/resources/intune-mam-windowsinformationprotectionpolicy?view=graph-rest-1.0)する
- オペレーティング システムのプラットフォームとバージョン、ドメインのメンバーシップ、構成設定の管理を含む[デバイス構成](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-1.0)ポリシーを作成し、展開する
- 制限付きのダウンロード、ネットワーク アクセサリのアクセス、ファイル転送を含むデバイスの[アクセス制御](/graph/api/resources/intune-onboarding-onpremisesconditionalaccesssettings?view=graph-rest-1.0)ポリシーを作成し、展開する
- デバイスの検索、パスワードの変更、デバイスのワイプなどの[リモート アクション](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0)を実行する

### <a name="manage-apps"></a>アプリの管理 

Intune API を使用して、次のアプリ管理タスクを実行できます。

- [アプリをデバイスに](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-1.0)展開する、またはアプリの展開を禁止する
- [電子ブック](/graph/api/resources/intune-books-ebookinstallsummary?view=graph-rest-1.0)と関連サービスへのアクセスを管理する
- アプリ構成設定、アプリ保護設定、およびアプリ使用ポリシーを定義し、展開する

### <a name="automate-intune"></a>Intune の自動化

Intune API を使用して、Intune の次の作業を自動化します。

- [ロール ベース](/graph/api/resources/intune-rbac-conceptual?view=graph-rest-1.0)のアクセス制御を定義し、割り当てる
- コンプライアンス、使用状況、およびアクセスを監査し、レポートする
- [通信費](/graph/api/resources/intune-tem-conceptual?view=graph-rest-1.0)を管理する

## <a name="api-reference"></a>API リファレンス
このサービスの API リファレンスをお探しですか?

- [Microsoft Graph v1.0 の Intune API](/graph/api/resources/intune-graph-overview?view=graph-rest-1.0)
- [Microsoft Graph ベータ版の Intune API](/graph/api/resources/intune-graph-overview?view=graph-rest-beta)

## <a name="next-steps"></a>次のステップ

- [Azure AD を使用して Intune API にアクセス](https://docs.microsoft.com/intune/intune-graph-apis)します。
- [PowerShell Intune サンプル](https://github.com/microsoftgraph/powershell-intune-samples)を使用して、一般的なタスクの実行方法を確認します。
- [Intune REST API の使用](/graph/api/resources/intune-graph-overview?view=graph-rest-1.0)方法を確認します。
- [Changelog](changelog.md) で Intune API の最新情報を確認します。
- Microsoft Graph の使用方法についてのさらに多くのアイデアについては、[サンプル](https://developer.microsoft.com/graph/graph/examples)を参照してください。
