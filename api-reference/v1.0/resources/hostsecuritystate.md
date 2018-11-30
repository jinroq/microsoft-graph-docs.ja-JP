---
title: hostSecurityState リソースの種類
description: ステートフルなホスト (デバイス、コンピューターを含む) について説明します。
ms.openlocfilehash: 3649553ae0f96222a09825e8819dfd0d199f8454
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023003"
---
# <a name="hostsecuritystate-resource-type"></a>hostSecurityState リソースの種類

ステートフルなホスト (デバイス、コンピューターを含む) について説明します。

## <a name="properties"></a>プロパティ

| プロパティ   | 型|説明|
|:---------------|:--------|:----------|
|fqdn|String|FQDN (完全修飾ドメイン名) のホスト (たとえば、 `machine.company.com`)。|
|isAzureAadJoined|ブール値|ホストが Azure Active Directory ドメイン サービスに参加しているドメインである場合は true。|
|isAzureAadRegistered|ブール値|Azure Active Directory デバイスの登録 (BYOD - は、完全に管理されているデバイスの企業が) を持つホストが登録されている場合は true。|
|isHybridAzureDomainJoined|ブール値|ホストが、オンプレミスの Active Directory ドメインに参加しているドメインである場合は true。|
|あります。|String|ローカル ホスト名、DNS ドメインの名前を持たない。|
|os|String|ホストのオペレーティング ・ システムです。 (たとえば、Windows10、MacOS、RHEL など)。|
|privateIpAddress|String|(ルーティングできない) プライベートの IPv4 または IPv6 アドレス ( [RFC 1918](https://tools.ietf.org/html/rfc1918)参照) 時の警告です。|
|publicIpAddress|String|公的にルーティング可能な IPv4 アドレスまたは IPv6 アドレス ( [RFC 1918](https://tools.ietf.org/html/rfc1918)参照) 警告の時にします。|
|riskScore|String|ホストのプロバイダーによって生成されると計算されるリスク ・ スコアです。  0 - 1 パーセントに相当する値の範囲をお勧めします。|

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
<!-- {
  "type": "#page.annotation",
  "description": "hostSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
