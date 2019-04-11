---
title: grouppolicypresentationcheckbox リソースの種類
description: admx checkBox 要素と admx boolean 要素を表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ba86365b83f3f6f961c2907eb4041ed15ce252a8
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31788136"
---
# <a name="grouppolicypresentationcheckbox-resource-type"></a>grouppolicypresentationcheckbox リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

admx checkBox 要素と admx boolean 要素を表します。


[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[grouppolicypresentationcheckboxes の一覧を表示する](../api/intune-grouppolicy-grouppolicypresentationcheckbox-list.md)|[grouppolicypresentationcheckbox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md)コレクション|[grouppolicypresentationcheckbox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[grouppolicypresentationcheckbox の取得](../api/intune-grouppolicy-grouppolicypresentationcheckbox-get.md)|[grouppolicypresentationcheckbox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md)|[grouppolicypresentationcheckbox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[grouppolicypresentationcheckbox の作成](../api/intune-grouppolicy-grouppolicypresentationcheckbox-create.md)|[grouppolicypresentationcheckbox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md)|新しい[grouppolicypresentationcheckbox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md)オブジェクトを作成します。|
|[grouppolicypresentationcheckbox の削除](../api/intune-grouppolicy-grouppolicypresentationcheckbox-delete.md)|なし|[grouppolicypresentationcheckbox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md)を削除します。|
|[grouppolicypresentationcheckbox の更新](../api/intune-grouppolicy-grouppolicypresentationcheckbox-update.md)|[grouppolicypresentationcheckbox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md)|[grouppolicypresentationcheckbox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|label|文字列|任意のプレゼンテーションエンティティのローカライズされたテキストラベル。 既定値は空白です。 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。|
|id|String|エンティティのキー。 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。|
|lastModifiedDateTime|DateTimeOffset|エンティティが最後に変更された日付と時刻。 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。|
|defaultchecked|Boolean|チェックボックスの既定値。 既定値は false です。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|definition|[grouppolicydefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|プレゼンテーションに関連付けられたグループポリシーの定義。 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。|

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





