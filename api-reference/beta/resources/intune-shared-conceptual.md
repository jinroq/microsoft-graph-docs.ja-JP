---
title: Microsoft Intune 内の共有リソース
description: これらのエンドポイントは、Intune ワークフローの複数の Microsoft グラフ API で使用されます。  意図、目的、および特定のリソースを使用する必要なアクセス許可は、特定のワークフローと基になる呼び出しのコンテキストによって異なります。  さらに、特定のメソッド、プロパティ、およびアクションが特定のワークフローに対してのみサポートします。
ms.openlocfilehash: a0e896b2aed219679ec45804dc94b22b7cb9d727
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073899"
---
# <a name="shared-resources-in-microsoft-intune"></a>Microsoft Intune 内の共有リソース

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing)を持っている必要があります。

これらのエンドポイントは、Intune ワークフローの複数の Microsoft グラフ API で使用されます。  意図、目的、および特定のリソースを使用する必要なアクセス許可は、特定のワークフローと基になる呼び出しのコンテキストによって異なります。  さらに、特定のメソッド、プロパティ、およびアクションが特定のワークフローに対してのみサポートします。

Intune ワークフローとの間は、次のグラフのリソースを共有します。

- [動作状態](intune-shared-actionstate.md)
- [すべてのデバイスの割り当て先](intune-shared-alldevicesassignmenttarget.md)
- [すべてのライセンス ユーザーの割り当て先](intune-shared-alllicensedusersassignmenttarget.md)
- [準拠の状態](intune-shared-compliancestatus.md)
- [デバイスおよびアプリ管理の割り当て先](intune-shared-deviceandappmanagementassignmenttarget.md)
- [デバイス アプリの管理](intune-shared-deviceappmanagement.md)
- [デバイス カテゴリ](intune-shared-devicecategory.md)
- [デバイス登録の種類](intune-shared-deviceenrollmenttype.md)
- [デバイスの管理](intune-shared-devicemanagement.md)
- [デバイス プラットフォームの種類](intune-shared-deviceplatformtype.md)
- [デバイスの種類](intune-shared-devicetype.md)
- [有効化](intune-shared-enablement.md)
- [除外グループの割り当て先](intune-shared-exclusiongroupassignmenttarget.md)
- [グループの割り当て先](intune-shared-groupassignmenttarget.md)
- [目的をインストールします。](intune-shared-installintent.md)
- [IP 範囲](intune-shared-iprange.md)
- [IPv4 の範囲](intune-shared-ipv4range.md)
- [IPv6 の範囲](intune-shared-ipv6range.md)
- [キー/値のペア](intune-shared-keyvaluepair.md)
- [MIME コンテンツ](intune-shared-mimecontent.md)
- [プロキシ化されたドメイン](intune-shared-proxieddomain.md)
- [Report](intune-shared-report.md)
- [レポートのルート](intune-shared-reportroot.md)
- [結果のアプリケーションの状態](intune-shared-resultantappstate.md)
- [RGB カラー](intune-shared-rgbcolor.md)
- [実行アカウントの種類として](intune-shared-runasaccounttype.md)
- [状態を実行します。](intune-shared-runstate.md)
- [UI 状態の生成オプションを保存](intune-shared-saveduistategenerationoptions.md)
- [URI](intune-shared-uri.md)
- [User](intune-shared-user.md)
- [VPP トークン アカウントの種類](intune-shared-vpptokenaccounttype.md)
- [VPP トークンの操作の失敗の理由](intune-shared-vpptokenactionfailurereason.md)
- [Windows ドメインの結合の構成](intune-shared-windowsdomainjoinconfiguration.md)
