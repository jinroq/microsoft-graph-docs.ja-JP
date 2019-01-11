---
title: windowsNetworkIsolationPolicy リソースの種類
description: Windows ネットワークの分離のポリシー
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 82026ba4d82b85a0275f83bb729b495e17ff5d5c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834616"
---
# <a name="windowsnetworkisolationpolicy-resource-type"></a>windowsNetworkIsolationPolicy リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Windows ネットワークの分離のポリシー
## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|enterpriseNetworkDomainNames|String コレクション|これは、エンタープライズの境界を構成するドメインのリストです。 デバイスに送信されるこれらのドメインの 1 つのデータはエンタープライズ データと見なされ、保護します。 これらの場所は安全なエンタープライズ ・ データを共有する先と見なされます。|
|enterpriseCloudResources|[proxiedDomain](../resources/intune-shared-proxieddomain.md) コレクション|保護する必要のあるクラウドでホストされているエンタープライズ リソースのドメインの一覧が含まれています。 これらのリソースへの接続は、エンタープライズ データと見なされます。 プロキシがクラウド リソースとペアリング済みの場合、クラウド リソースへのトラフィックは、指定されたプロキシ サーバー (ポート 80) を介してエンタープライズ ネットワーク経由でルーティングされます。 EnterpriseInternalProxyServers ポリシーを使用してこの目的に使用されるプロキシ サーバーを構成することもする必要があります。 このコレクションには、最大で 500 個の要素を含めることができます。|
|enterpriseIPRanges|[ipRange](../resources/intune-shared-iprange.md) コレクション|エンタープライズ ネットワーク内のコンピューターを定義するエンタープライズ IP の範囲を設定します。 これらのコンピューターからのデータはエンタープライズの一部と見なされ、保護されます。 これらの場所は安全なエンタープライズ ・ データを共有する先と見なされます。 このコレクションには、最大で 500 個の要素を含めることができます。|
|enterpriseInternalProxyServers|String コレクション|これは、内部プロキシ サーバーのコンマ区切りのリストです。 例: "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59"。 これらのプロキシは、管理者により、インターネット上の特定のリソースに接続するように構成されています。 それらはエンタープライズ ネットワークの場所にあると見なされます。 プロキシは、一致したクラウド リソースのこれらのプロキシを経由するトラフィックを強制的に EnterpriseCloudResources のポリシーを構成する際に活用できるのみ。|
|enterpriseIPRangesAreAuthoritative|Boolean|構成済みのリストを承諾し、ヒューリスティックを使用した他のサブネットの検索を行わないよう、クライアントに指示するブール値。 既定では false を指定します。|
|enterpriseProxyServers|String コレクション|これは、プロキシ サーバーのリストです。 任意のサーバー一覧とは見なされません非エンタープライズです。|
|enterpriseProxyServersAreAuthoritative|Boolean|プロキシの構成済みリストを承諾し、他の作業プロキシの検出を試みないよう、クライアントに指示するブール値。 既定値は false です|
|neutralDomainResources|String コレクション|作業時間またはリソースの個人に使用できるドメイン名のリストです。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsNetworkIsolationPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsNetworkIsolationPolicy",
  "enterpriseNetworkDomainNames": [
    "String"
  ],
  "enterpriseCloudResources": [
    {
      "@odata.type": "microsoft.graph.proxiedDomain",
      "ipAddressOrFQDN": "String",
      "proxy": "String"
    }
  ],
  "enterpriseIPRanges": [
    {
      "@odata.type": "microsoft.graph.iPv6Range",
      "lowerAddress": "String",
      "upperAddress": "String"
    }
  ],
  "enterpriseInternalProxyServers": [
    "String"
  ],
  "enterpriseIPRangesAreAuthoritative": true,
  "enterpriseProxyServers": [
    "String"
  ],
  "enterpriseProxyServersAreAuthoritative": true,
  "neutralDomainResources": [
    "String"
  ]
}
```





