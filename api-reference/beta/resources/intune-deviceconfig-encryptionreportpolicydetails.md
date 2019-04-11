---
title: encryptionreportpolicydetails リソースの種類
description: 暗号化レポートのポリシーの詳細
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9c9903b54483fc6f77cd183abee0e54b10acf9cc
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31771013"
---
# <a name="encryptionreportpolicydetails-resource-type"></a>encryptionreportpolicydetails リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

暗号化レポートのポリシーの詳細

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|policyid|文字列|暗号化レポートのポリシー Id|
|policyName|文字列|暗号化レポートのポリシー名|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.encryptionReportPolicyDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.encryptionReportPolicyDetails",
  "policyId": "String",
  "policyName": "String"
}
```





