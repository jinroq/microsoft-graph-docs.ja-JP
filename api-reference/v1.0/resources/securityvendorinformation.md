---
title: securityVendorInformation リソースの種類
description: " subprovider = AppLocker)。"
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: fb5dee36da08332fd5c36f7ee4e578cc9fb7deaa
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549700"
---
# <a name="securityvendorinformation-resource-type"></a>securityVendorInformation リソースの種類

セキュリティ製品/サービスベンダー、プロバイダ、およびサブプロバイダに関する詳細情報が含まれています (たとえば、ベンダー = Microsoft; provider = Windows Defender ATP; subprovider = AppLocker)。

## <a name="properties"></a>プロパティ

| プロパティ   | 型|説明|
|:---------------|:--------|:----------|
|供給 |String|特定のプロバイダー (製品/サービス-ベンダー会社ではない)。たとえば、windowsdefenderatp のようになります。|
|providerversion|String|通知を生成したプロバイダーまたはサブプロバイダのバージョン (存在する場合)。 *必須*|
|subprovider|String|特定のサブプロバイダ (集計プロバイダーの場合)。たとえば、windowsdefenderatp。|
|ベンダ |String|通知ベンダーの名前 (Microsoft、Dell、焼討アイなど)。 *必須*|


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
<!-- {
  "type": "#page.annotation",
  "description": "securityVendorInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
