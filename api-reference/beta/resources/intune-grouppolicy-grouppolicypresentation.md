---
title: groupPolicyPresentation リソースの種類
description: グループポリシー定義の追加オプションを表示するための基本エンティティ。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 00151ec7c75a071df9c6485a68749cce07e6f91a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32575829"
---
# <a name="grouppolicypresentation-resource-type"></a>groupPolicyPresentation リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

グループポリシー定義の追加オプションを表示するための基本エンティティ。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[groupPolicyPresentation を取得する](../api/intune-grouppolicy-grouppolicypresentation-get.md)|[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[groupPolicyPresentation の更新](../api/intune-grouppolicy-grouppolicypresentation-update.md)|[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|label|String|任意のプレゼンテーションエンティティのローカライズされたテキストラベル。 既定値は空白です。|
|id|String|エンティティのキー。|
|lastModifiedDateTime|DateTimeOffset|エンティティが最後に変更された日付と時刻。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|definition|[grouppolicydefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|プレゼンテーションに関連付けられたグループポリシーの定義。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentation",
  "label": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```





