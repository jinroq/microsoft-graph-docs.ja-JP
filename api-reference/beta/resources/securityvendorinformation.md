---
title: securityVendorInformation リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 0137abd7a9df0df94f73e18d7efa201008031ff6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939925"
---
# <a name="securityvendorinformation-resource-type"></a>securityVendorInformation リソースの種類

 > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

セキュリティ製品やサービスの仕入先、プロバイダー、および subprovider の詳細が含まれています (たとえば、ベンダー = Microsoft; プロバイダー = Windows Defender の分析ツールです。 subProvider AppLocker を =)。

## <a name="properties"></a>プロパティ

| プロパティ   | 種類|説明|
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
