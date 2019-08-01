---
title: securityVendorInformation リソースの種類
description: " subProvider = AppLocker)。"
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 3fb959da2d6af10632f9113a33eb942492b679ef
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034427"
---
# <a name="securityvendorinformation-resource-type"></a>securityVendorInformation リソースの種類

セキュリティ製品/サービスベンダー、プロバイダ、およびサブプロバイダに関する詳細情報が含まれています (たとえば、ベンダー = Microsoft; provider = Windows Defender ATP; subProvider = AppLocker)。

## <a name="properties"></a>プロパティ

| プロパティ   | 型|説明|
|:---------------|:--------|:----------|
|供給 |String|特定のプロバイダー (製品/サービス-ベンダー会社ではない)。たとえば、WindowsDefenderATP のようになります。|
|providerVersion|String|通知を生成したプロバイダーまたはサブプロバイダのバージョン (存在する場合)。 *Required*|
|subProvider|String|特定のサブプロバイダ (集計プロバイダーの場合)。たとえば、WindowsDefenderATP。|
|ベンダ |String|通知ベンダーの名前 (Microsoft、Dell、焼討アイなど)。 *Required*|


## <a name="json-representation"></a>JSON 表記

Folllowing は、リソースの JSON 表記です。
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
