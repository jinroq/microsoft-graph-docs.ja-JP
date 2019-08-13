---
title: windowsNetworkIsolationPolicy リソースの種類
description: Windows ネットワーク分離ポリシー
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 515d1b89631b33907aef0ef19bbc3f28181dc5d8
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36370768"
---
# <a name="windowsnetworkisolationpolicy-resource-type"></a>windowsNetworkIsolationPolicy リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Windows ネットワーク分離ポリシー

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|enterpriseNetworkDomainNames|文字列コレクション|これは、エンタープライズの境界を構成するドメインのリストです。 デバイスに送信されるこれらのドメインのいずれかのデータは、エンタープライズデータとして保護されています。 これらの場所は、エンタープライズデータの共有先として安全であると見なされます。|
|enterpriseCloudResources|[proxiedDomain](../resources/intune-shared-proxieddomain.md) コレクション|クラウドでホストされている、保護する必要があるエンタープライズリソースドメインの一覧が含まれています。 これらのリソースへの接続は、エンタープライズ データと見なされます。 プロキシがクラウド リソースとペアリング済みの場合、クラウド リソースへのトラフィックは、指定されたプロキシ サーバー (ポート 80) を介してエンタープライズ ネットワーク経由でルーティングされます。 この目的で使用されるプロキシサーバーも、EnterpriseInternalProxyServers ポリシーを使用して構成する必要があります。 このコレクションには、最大で 500 個の要素を含めることができます。|
|enterpriseIPRanges|[ipRange](../resources/intune-shared-iprange.md) コレクション|エンタープライズ ネットワーク内のコンピューターを定義するエンタープライズ IP の範囲を設定します。 これらのコンピューターからのデータはエンタープライズの一部と見なされ、保護されます。 これらの場所は、エンタープライズデータの共有先として安全であると見なされます。 このコレクションには、最大で 500 個の要素を含めることができます。|
|enterpriseInternalProxyServers|文字列コレクション|これは、内部プロキシ サーバーのコンマ区切りのリストです。 例: "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59"。 これらのプロキシは、管理者により、インターネット上の特定のリソースに接続するように構成されています。 それらはエンタープライズ ネットワークの場所にあると見なされます。 プロキシは、EnterpriseCloudResources ポリシーを構成する場合にのみ使用され、これらのプロキシを介して一致するクラウドリソースにトラフィックを強制します。|
|enterpriseIPRangesAreAuthoritative|Boolean|構成済みのリストを承諾し、ヒューリスティックを使用した他のサブネットの検索を行わないよう、クライアントに指示するブール値。 既定値は false です。|
|enterpriseProxyServers|文字列コレクション|これは、プロキシ サーバーのリストです。 この一覧にないサーバーは、非エンタープライズとみなされます。|
|enterpriseProxyServersAreAuthoritative|Boolean|プロキシの構成済みリストを承諾し、他の作業プロキシの検出を試みないよう、クライアントに指示するブール値。 既定値は false です|
|neutralDomainResources|文字列コレクション|作業または個人のリソースに使用できるドメイン名のリスト。|

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



