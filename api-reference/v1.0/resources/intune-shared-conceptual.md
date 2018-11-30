---
title: Microsoft Intune 内の共有リソース
description: これらのエンドポイントは、Intune ワークフローの複数の Microsoft グラフ API で使用されます。  意図、目的、および特定のリソースを使用する必要なアクセス許可は、特定のワークフローと基になる呼び出しのコンテキストによって異なります。  さらに、特定のメソッド、プロパティ、およびアクションが特定のワークフローに対してのみサポートします。
ms.openlocfilehash: 8355d3b4bcb9b4fdc7fc8c1874641117dad1d583
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024180"
---
# <a name="shared-resources-in-microsoft-intune"></a>Microsoft Intune 内の共有リソース

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing)を持っている必要があります。

これらのエンドポイントは、Intune ワークフローの複数の Microsoft グラフ API で使用されます。  意図、目的、および特定のリソースを使用する必要なアクセス許可は、特定のワークフローと基になる呼び出しのコンテキストによって異なります。  さらに、特定のメソッド、プロパティ、およびアクションが特定のワークフローに対してのみサポートします。

Intune ワークフローとの間は、次のグラフのリソースを共有します。  

- [すべてのデバイスの割り当て先](intune-shared-alldevicesassignmenttarget.md)
- [すべてのライセンス ユーザーの割り当て先](intune-shared-alllicensedusersassignmenttarget.md)
- [準拠の状態](intune-shared-compliancestatus.md)
- [デバイスおよびアプリ管理の割り当て先](intune-shared-deviceandappmanagementassignmenttarget.md)
- [デバイス アプリの管理](intune-shared-deviceappmanagement.md)
- [デバイス カテゴリ](intune-shared-devicecategory.md)
- [デバイスの管理](intune-shared-devicemanagement.md)
- [除外グループの割り当て先](intune-shared-exclusiongroupassignmenttarget.md)
- [グループの割り当て先](intune-shared-groupassignmenttarget.md)
- [目的をインストールします。](intune-shared-installintent.md)
- [MIME コンテンツ](intune-shared-mimecontent.md)
- [Report](intune-shared-report.md)
- [レポートのルート](intune-shared-reportroot.md)
- [UI 状態の生成オプションを保存](intune-shared-saveduistategenerationoptions.md)
- [URI](intune-shared-uri.md)
- [User](intune-shared-user.md)
- [VPP トークン アカウントの種類](intune-shared-vpptokenaccounttype.md)
