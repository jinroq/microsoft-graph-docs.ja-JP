---
title: groupPolicyPresentationListBox リソースの種類
description: ADMX リスト ボックス要素と ADMX リスト要素を表します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2cde4a73456975629af81de676e593c3fec3e211
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430509"
---
# <a name="grouppolicypresentationlistbox-resource-type"></a>groupPolicyPresentationListBox リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

ADMX リスト ボックス要素と ADMX リスト要素を表します。


[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト groupPolicyPresentationListBoxes](../api/intune-grouppolicy-grouppolicypresentationlistbox-list.md)|[groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)コレクション|[GroupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)オブジェクトのプロパティと関係を一覧表示します。|
|[GroupPolicyPresentationListBox を取得します。](../api/intune-grouppolicy-grouppolicypresentationlistbox-get.md)|[groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)|[GroupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)オブジェクトのプロパティと関係を参照してください。|
|[GroupPolicyPresentationListBox を作成します。](../api/intune-grouppolicy-grouppolicypresentationlistbox-create.md)|[groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)|新しい[groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)オブジェクトを作成します。|
|[GroupPolicyPresentationListBox を削除します。](../api/intune-grouppolicy-grouppolicypresentationlistbox-delete.md)|なし|の[groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)を削除します。|
|[GroupPolicyPresentationListBox を更新します。](../api/intune-grouppolicy-grouppolicypresentationlistbox-update.md)|[groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)|[GroupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|label|String|プレゼンテーションの任意のエンティティのローカライズされたテキスト ラベルです。 既定値は空です。 [GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承されました。|
|id|String|エンティティのキー。 [GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承されました。|
|lastModifiedDateTime|DateTimeOffset|日付と時刻、エンティティが最後に修正されました。 [GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承されました。|
|explicitValue|Boolean|True ユーザー レジストリ サブキーの値とレジストリ サブキー名を指定してくださいこのオプションを指定します。 リスト ボックスでは、名前とデータの 2 つの列を表示します。 既定値は、false を指定します。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|definition|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|プレゼンテーションに関連付けられているグループ ポリシーの定義です。 [GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承されました。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationListBox"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationListBox",
  "label": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "explicitValue": true
}
```




