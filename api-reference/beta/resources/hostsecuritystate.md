---
title: hostSecurityState リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。"
localization_priority: Normal
ms.openlocfilehash: d6f566a2bd42163c570fe837d2419057c62664bb
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526698"
---
# <a name="hostsecuritystate-resource-type"></a>hostSecurityState リソースの種類

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ステートフルなホスト (デバイス、コンピューターを含む) について説明します。

## <a name="properties"></a>プロパティ

| プロパティ   | 型|説明|
|:---------------|:--------|:----------|
|fqdn|String|ホストの FQDN (完全修飾ドメイン名) (machine.company.com など)。|
|isAzureAadJoined|ブール値|ホストが Azure Active Directory ドメイン サービスに参加しているドメインである場合は true。|
|isAzureAadRegistered|ブール値|Azure Active Directory デバイスの登録 (BYOD - は、完全に管理されているデバイスの企業が) を持つホストが登録されている場合は true。|
|isHybridAzureDomainJoined|ブール値|ホストが、オンプレミスの Active Directory ドメインに参加しているドメインである場合は true。|
|あります。|String|ローカル ホスト名、DNS ドメインの名前を持たない。|
|I-5.|String|ホストのオペレーティング ・ システムです。 (たとえば、Windows10、MacOS、RHEL など)。|
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
<!--
{
  "type": "#page.annotation",
  "description": "hostSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/hostsecuritystate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
