---
title: Microsoft Intune での共有リソース-Microsoft Graph API
description: テナント組織の複数のワークフローをサポートする Intune エンドポイント (REST) の Microsoft Graph API の一覧を示します。
localization_priority: Normal
author: rolyon
ms.prod: intune
ms.openlocfilehash: d627ebb67876c89136ba6e4e63e9879e3a0ed8d2
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33939904"
---
# <a name="shared-resources-in-microsoft-intune"></a>Microsoft Intune での共有リソース

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでは、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing)を持っている必要があります。

これらのエンドポイントは、Intune ワークフロー用の複数の Microsoft Graph API で使用されます。  特定のリソースを使用するために必要な目的、およびアクセス許可は、基になる呼び出しの特定のワークフローおよびコンテキストによって異なります。  さらに、特定のワークフローに対してのみ、特定のメソッド、プロパティ、およびアクションがサポートされます。

次の Graph リソースは、Intune ワークフロー間で共有されます。

- [アクションの状態](intune-shared-actionstate.md)
- [すべてのデバイスの割り当て先](intune-shared-alldevicesassignmenttarget.md)
- [すべてのライセンス ユーザーの割り当て先](intune-shared-alllicensedusersassignmenttarget.md)
- [コンプライアンスのステータス](intune-shared-compliancestatus.md)
- [デバイスおよびアプリ管理の割り当て先](intune-shared-deviceandappmanagementassignmenttarget.md)
- [デバイス アプリの管理](intune-shared-deviceappmanagement.md)
- [デバイス カテゴリ](intune-shared-devicecategory.md)
- [デバイスの登録のタイプ](intune-shared-deviceenrollmenttype.md)
- [デバイスの管理](intune-shared-devicemanagement.md)
- [デバイスのプラットフォームの種類](intune-shared-deviceplatformtype.md)
- [デバイスのタイプ](intune-shared-devicetype.md)
- [有効化](intune-shared-enablement.md)
- [除外グループの割り当て先](intune-shared-exclusiongroupassignmenttarget.md)
- [グループの割り当て先](intune-shared-groupassignmenttarget.md)
- [インストール目的](intune-shared-installintent.md)
- [IP 範囲](intune-shared-iprange.md)
- [IPv4 の範囲](intune-shared-ipv4range.md)
- [IPv6 の範囲](intune-shared-ipv6range.md)
- [キー/値のペア](intune-shared-keyvaluepair.md)
- [MIME コンテンツ](intune-shared-mimecontent.md)
- [モバイル アプリのトラブルシューティング イベント](intune-shared-mobileapptroubleshootingevent.md)
- [プロキシ化されたドメイン](intune-shared-proxieddomain.md)
- [Report](intune-shared-report.md)
- [レポートのルート](intune-shared-reportroot.md)
- [アプリの状態の結果](intune-shared-resultantappstate.md)
- [RGB カラー](intune-shared-rgbcolor.md)
- [アカウントの種類として実行](intune-shared-runasaccounttype.md)
- [実行状態](intune-shared-runstate.md)
- [保存 UI 状態生成オプション](intune-shared-saveduistategenerationoptions.md)
- [URI](intune-shared-uri.md)
- [ユーザー](intune-shared-user.md)
- [VPP トークン アカウントのタイプ](intune-shared-vpptokenaccounttype.md)
- [VPP トークンのアクションのエラーの理由](intune-shared-vpptokenactionfailurereason.md)
- [Windows ドメイン参加の構成](intune-shared-windowsdomainjoinconfiguration.md)
