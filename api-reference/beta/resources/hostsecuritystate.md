---
title: hostsecuritystate リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでは、これらの API の使用はサポートされていません。"
localization_priority: Normal
ms.openlocfilehash: 670a052fa3d63da0b78ba620dbc6530a8ab122dc
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340306"
---
# <a name="hostsecuritystate-resource-type"></a>hostsecuritystate リソースの種類

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ホストに関するステートフルな情報を含みます (デバイス、コンピューターなどを含む)。

## <a name="properties"></a>プロパティ

| プロパティ   | 型|説明|
|:---------------|:--------|:----------|
|fqdn|String|ホストの FQDN (完全修飾ドメイン名) (たとえば、machine.company.com)。|
|isAzureAadJoined|Boolean|ホストが Azure Active Directory ドメインサービスにドメインに参加している場合は True。|
|isAzureAadRegistered|Boolean|ホストが Azure Active Directory デバイス登録 (byod devices、enterprise によって完全に管理されていない) に登録されている場合は、True。|
|isHybridAzureDomainJoined|Boolean|ホストがオンプレミスの Active Directory ドメインに参加しているドメインである場合は True。|
|netBiosName|String|DNS ドメイン名を除いたローカルホスト名。|
|hp-ux|String|ホストオペレーティングシステム。 (たとえば、Windows10、MacOS、RHEL など)。|
|privateIpAddress|String|プライベート (ルーティング可能ではない) IPv4 または IPv6 アドレス ( [RFC 1918](https://tools.ietf.org/html/rfc1918)を参照) 通知時。|
|publicipaddress|String|通知時に公開ルーティング可能な IPv4 または IPv6 アドレス ( [RFC 1918](https://tools.ietf.org/html/rfc1918)を参照)。|
|riskScore|String|プロバイダーが生成/計算するホストのリスクスコア。  推奨値の範囲0-1。パーセンテージに相当します。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.hostSecurityState"
}-->

```json
{
  "fqdn": "String",
  "isAzureAadJoined": true,
  "isAzureAadRegistered": true,
  "isHybridAzureDomainJoined": true,
  "netBiosName": "String",
  "os": "String",
  "privateIpAddress": "String",
  "publicIpAddress": "String",
  "riskScore": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "hostSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
