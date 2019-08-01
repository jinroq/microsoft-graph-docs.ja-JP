---
title: Microsoft Intune での共有リソース
description: これらのエンドポイントは、Intune ワークフロー用の複数の Microsoft Graph API で使用されます。  特定のリソースを使用するために必要な目的、およびアクセス許可は、基になる呼び出しの特定のワークフローおよびコンテキストによって異なります。  さらに、特定のワークフローに対してのみ、特定のメソッド、プロパティ、およびアクションがサポートされます。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: 7f04077278a3765a27abd30f02bcc2361c7cd08e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037017"
---
# <a name="shared-resources-in-microsoft-intune"></a>Microsoft Intune での共有リソース

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing)を持っている必要があります。

これらのエンドポイントは、Intune ワークフロー用の複数の Microsoft Graph API で使用されます。  特定のリソースを使用するために必要な目的、およびアクセス許可は、基になる呼び出しの特定のワークフローおよびコンテキストによって異なります。  さらに、特定のワークフローに対してのみ、特定のメソッド、プロパティ、およびアクションがサポートされます。

次の Graph リソースは、Intune ワークフロー間で共有されます。  

- [すべてのデバイスの割り当て先](intune-shared-alldevicesassignmenttarget.md)
- [すべてのライセンス ユーザーの割り当て先](intune-shared-alllicensedusersassignmenttarget.md)
- [コンプライアンスのステータス](intune-shared-compliancestatus.md)
- [デバイスおよびアプリ管理の割り当て先](intune-shared-deviceandappmanagementassignmenttarget.md)
- [デバイス アプリの管理](intune-shared-deviceappmanagement.md)
- [デバイス カテゴリ](intune-shared-devicecategory.md)
- [デバイスの管理](intune-shared-devicemanagement.md)
- [除外グループの割り当て先](intune-shared-exclusiongroupassignmenttarget.md)
- [グループの割り当て先](intune-shared-groupassignmenttarget.md)
- [インストール目的](intune-shared-installintent.md)
- [MIME コンテンツ](intune-shared-mimecontent.md)
- [Report](intune-shared-report.md)
- [レポートのルート](intune-shared-reportroot.md)
- [保存 UI 状態生成オプション](intune-shared-saveduistategenerationoptions.md)
- [URI](intune-shared-uri.md)
- [ユーザー](intune-shared-user.md)
- [VPP トークン アカウントのタイプ](intune-shared-vpptokenaccounttype.md)
