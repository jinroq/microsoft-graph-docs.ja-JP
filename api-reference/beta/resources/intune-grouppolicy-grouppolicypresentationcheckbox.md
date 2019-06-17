---
title: groupPolicyPresentationCheckBox リソースの種類
description: ADMX checkBox 要素と ADMX boolean 要素を表します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cbcff2437270ef7c56846f0945e856a1cc62ba03
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34982967"
---
# <a name="grouppolicypresentationcheckbox-resource-type"></a>groupPolicyPresentationCheckBox リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

ADMX checkBox 要素と ADMX boolean 要素を表します。


[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[GroupPolicyPresentationCheckBoxes の一覧を表示する](../api/intune-grouppolicy-grouppolicypresentationcheckbox-list.md)|[Grouppolicypresentationcheckbox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md)コレクション|[Grouppolicypresentationcheckbox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[GroupPolicyPresentationCheckBox の取得](../api/intune-grouppolicy-grouppolicypresentationcheckbox-get.md)|[groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md)|[Grouppolicypresentationcheckbox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[GroupPolicyPresentationCheckBox の作成](../api/intune-grouppolicy-grouppolicypresentationcheckbox-create.md)|[groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md)|新しい[Grouppolicypresentationcheckbox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md)オブジェクトを作成します。|
|[GroupPolicyPresentationCheckBox の削除](../api/intune-grouppolicy-grouppolicypresentationcheckbox-delete.md)|None|[Grouppolicypresentationcheckbox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md)を削除します。|
|[GroupPolicyPresentationCheckBox の更新](../api/intune-grouppolicy-grouppolicypresentationcheckbox-update.md)|[groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md)|[Grouppolicypresentationcheckbox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|label|String|任意のプレゼンテーションエンティティのローカライズされたテキストラベル。 既定値は空白です。 [GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。|
|id|String|エンティティのキー。 [GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。|
|lastModifiedDateTime|DateTimeOffset|エンティティが最後に変更された日付と時刻。 [GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。|
|defaultChecked|Boolean|チェックボックスの既定値。 既定値は false です。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|definition|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|プレゼンテーションに関連付けられたグループポリシーの定義。 [GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationCheckBox"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationCheckBox",
  "label": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "defaultChecked": true
}
```





