---
title: Microsoft Graph Security API を使用したセキュリティ ソリューションの統合
description: この記事で説明されているいずれかのオプションを使用して、Microsoft Graph Security API に接続します。 これらのオプションを使用すると、サポート対象の Microsoft およびパートナーのセキュリティ プロバイダー間で統一された形式のデータを、単一の統合を介して操作できます。
author: preetikr
localization_priority: Priority
ms.prod: security
ms.openlocfilehash: 362dde5c75180bfe1edbf42f49bcbe009af9015a
ms.sourcegitcommit: 496269b62d42cb7a96752a77b0f2e0cb16918f0b
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/21/2019
ms.locfileid: "36484412"
---
# <a name="security-solution-integrations-using-the-microsoft-graph-security-api"></a>Microsoft Graph Security API を使用したセキュリティ ソリューションの統合

次のいずれかのオプションを使用して、Microsoft Graph Security API に接続します。 これらのオプションを使用すると、[サポート対象の Microsoft およびパートナーのセキュリティ プロバイダー](https://aka.ms/graphsecurityalerts)間で統一された形式のデータを、単一の統合を介して操作できます。

- **サポートされている統合オプションを直接使用する** – アプリケーションに直接接続するコードを作成して豊富な分析情報を派生させるなど、[サポートされている統合オプションの一覧](https://docs.microsoft.com/graph/security-concept-overview#why-use-the-microsoft-graph-security-api)を参照してください。 [サンプル](https://aka.ms/graphsecurityapicode) を活用して、始めましょう。
- **Microsoft のパートナーによってビルドされたネイティブの統合およびコネクタを使用する** – これらの統合を使用するには、[Microsoft Graph Security API のパートナー ソリューション](https://aka.ms/graphsecuritypartnerships) を参照してください。  
- **Microsoft によってビルドされたコネクタを使用する** – セキュリティ インシデントと管理 (SIEM)、セキュリティ レスポンスとオーケストレーション (SOAR)、インシデント追跡とサービス管理 (ITSM)、レポートなどのさまざまなソリューションを通じて API に接続するために使用される[コネクタの一覧](https://aka.ms/graphsecuritysolutionsconnectors) を参照してください。  

## <a name="list-of-connectors-from-microsoft"></a>Microsoft のコネクタの一覧

| ソリューションの種類 | 名前 | コネクタ | アナウンス |
|:-----|:--------|:--------|:----------|
| SIEM |Splunk |[ Splunk 向け Microsoft Graph Security API アドオン](https://aka.ms/graphsecuritysplunkaddon) | [ブログ投稿](https://aka.ms/graphsecuritysplunkaddonblogpost) |
| SOAR | Azure Logic Apps / Microsoft Flow | [Azure Logic Apps、Microsoft Flow および PowerApps 用の Microsoft Graph セキュリティ コネクタ](https://aka.ms/graphsecurityconnectors) | [ブログ投稿](https://aka.ms/graphsecurityconnectorsblogpost) |
| オートメーション | PowerShell モジュール | [Microsoft Graph セキュリティ PowerShell モジュール](https://aka.ms/graphsecuritypowershellmodule) | [ブログ投稿](https://aka.ms/graphsecuritypowershellmodulepost) |
| レポート | Power BI | [Power BI 用の Microsoft Graph セキュリティ コネクタ](https://aka.ms/graphsecuritypowerbiconnectordoc) | [ブログ投稿](https://aka.ms/graphsecuritypowerbiconnectorblogpost) |

ソリューションにネイティブの統合をサポートするか、Microsoft Graph Security API のデータ プロバイダーになりたい場合は、[パートナーシップの機会](https://docs.microsoft.com/graph/security-partner-overview)を確認します。
