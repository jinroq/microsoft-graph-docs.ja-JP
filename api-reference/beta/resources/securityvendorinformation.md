---
title: securityVendorInformation リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでは、これらの API の使用はサポートされていません。"
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 7f48c27ba94d8419ce244143a48cf6ab04dd080e
ms.sourcegitcommit: 88ddd033de0f36eedade277d57c922ebd0db5bba
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/02/2019
ms.locfileid: "30364585"
---
# <a name="securityvendorinformation-resource-type"></a>securityVendorInformation リソースの種類

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

セキュリティ製品/サービスベンダー、プロバイダ、およびサブプロバイダに関する詳細情報が含まれています (たとえば、ベンダー = Microsoft; provider = Windows Defender ATP; subprovider = AppLocker)。

## <a name="properties"></a>プロパティ

| プロパティ   | 型|説明|
|:---------------|:--------|:----------|
|供給 |String|特定のプロバイダー (製品/サービス-ベンダー会社ではない)。たとえば、windowsdefenderatp のようになります。|
|providerversion|String|通知を生成したプロバイダーまたはサブプロバイダのバージョン (存在する場合)。 **Required**|
|subprovider|String|特定のサブプロバイダ (集計プロバイダーの場合)。たとえば、windowsdefenderatp。|
|ベンダ |String|通知ベンダーの名前 (Microsoft、Dell、焼討アイなど)。 **Required**|

## <a name="json-representation"></a>JSON 表記

folllowing は、リソースの JSON 表記です。
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
<!--
{
  "type": "#page.annotation",
  "description": "securityVendorInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/securityvendorinformation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
