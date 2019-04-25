---
title: customsubjectoff・ベンダーのリソースの種類
description: カスタムサブジェクトの別名定義
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 03507d4e912af011db011283a95887590ab79801
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549370"
---
# <a name="customsubjectalternativename-resource-type"></a>customsubjectoff・ベンダーのリソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

カスタムサブジェクトの別名定義

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|santype|[subjectAlternativeNameType](../resources/intune-deviceconfig-subjectalternativenametype.md)|カスタム SAN の種類。 可能な値は、`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService` です。|
|name|String|ユーザー設定の SAN 名|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.customSubjectAlternativeName"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.customSubjectAlternativeName",
  "sanType": "String",
  "name": "String"
}
```





