---
title: grouppolicydefinitionfile リソースの種類
description: エンティティは、ADMX (管理用テンプレート) XML ファイルを表します。 ADMX ファイルには、グループポリシー定義のコレクションと、カテゴリパスごとの場所が含まれています。 グループポリシー定義ファイルには、言語に依存する ADML (管理用テンプレート) の言語ファイルによってサポートされている言語も含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 494a2f8ff80b3a7f8ee9db9fea4d795494c19a92
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30161335"
---
# <a name="grouppolicydefinitionfile-resource-type"></a>grouppolicydefinitionfile リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

エンティティは、ADMX (管理用テンプレート) XML ファイルを表します。 ADMX ファイルには、グループポリシー定義のコレクションと、カテゴリパスごとの場所が含まれています。 グループポリシー定義ファイルには、言語に依存する ADML (管理用テンプレート) の言語ファイルによってサポートされている言語も含まれています。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[grouppolicydefinitionfile の取得](../api/intune-grouppolicy-grouppolicydefinitionfile-get.md)|[grouppolicydefinitionfile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|[grouppolicydefinitionfile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[grouppolicydefinitionfile の更新](../api/intune-grouppolicy-grouppolicydefinitionfile-update.md)|[grouppolicydefinitionfile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|[grouppolicydefinitionfile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|displayName|String|ADMX ファイルのローカライズされたフレンドリ名。|
|説明|String|ADMX ファイルのポリシー設定のローカライズされた説明。 既定値は empty です。|
|languageCodes|String collection|ADMX ファイルでサポートされている言語コード。|
|targetprefix|String|ADMX ファイル内の名前空間を参照する論理名を指定します。|
|targetNamespace|String|ADMX ファイル内の名前空間を識別するために使用する URI を指定します。|
|msrtcsip-policytype|[groupPolicyType](../resources/intune-grouppolicy-grouppolicytype.md)|グループポリシーの種類を指定します。 使用可能な値は、`admxBacked`、`admxIngested` です。|
|id|String|エンティティのキー。|
|lastModifiedDateTime|DateTimeOffset|エンティティが最後に変更された日付と時刻。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|定義|[grouppolicydefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)コレクション|ファイルに関連付けられたグループポリシーの定義。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyDefinitionFile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionFile",
  "displayName": "String",
  "description": "String",
  "languageCodes": [
    "String"
  ],
  "targetPrefix": "String",
  "targetNamespace": "String",
  "policyType": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```




