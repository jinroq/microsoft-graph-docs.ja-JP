---
title: securityVendorInformation リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
ms.openlocfilehash: 4016e274a82ad6a28101dbf5b053124b439a3cbf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072234"
---
# <a name="securityvendorinformation-resource-type"></a>securityVendorInformation リソースの種類

 > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

セキュリティ製品やサービスの仕入先、プロバイダー、および subprovider の詳細が含まれています (たとえば、ベンダー = Microsoft; プロバイダー = Windows Defender の分析ツールです。 subProvider AppLocker を =)。

## <a name="properties"></a>プロパティ

| プロパティ   | 型|説明|
|:---------------|:--------|:----------|
|プロバイダー |String|特定のプロバイダー (製品やサービスの仕入先会社ではありません)。たとえば、WindowsDefenderATP です。|
|providerVersion|String|Subprovider、それが存在する場合は、アラートを生成したプロバイダーのバージョンです。 *Required*|
|subProvider|String|特定の subprovider 下にあるプロバイダーを集約)。たとえば、WindowsDefenderATP.SmartScreen です。|
|仕入先 |String|アラート ベンダー (マイクロソフトでは、Dell の FireEye など) の名前。 *Required*|

## <a name="json-representation"></a>JSON 表記

次は、リソースの JSON 表現です。
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.securityVendorInformation"
}-->

```json
{
  "provider": "String",
  "providerVersion": "String",
  "subProvider": "String",
  "vendor": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "securityVendorInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
