---
title: groupPolicyPresentationListBox リソースの種類
description: ADMX listBox 要素と ADMX list 要素を表します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d24b70809eb08828b2cc037a7986c6d7b5e255ef
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34985340"
---
# <a name="grouppolicypresentationlistbox-resource-type"></a>groupPolicyPresentationListBox リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

ADMX listBox 要素と ADMX list 要素を表します。


[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト groupPolicyPresentationListBoxes ボックス](../api/intune-grouppolicy-grouppolicypresentationlistbox-list.md)|[Grouppolicypresentationlistbox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)コレクション|[Grouppolicypresentationlistbox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[GroupPolicyPresentationListBox の取得](../api/intune-grouppolicy-grouppolicypresentationlistbox-get.md)|[groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)|[Grouppolicypresentationlistbox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[GroupPolicyPresentationListBox の作成](../api/intune-grouppolicy-grouppolicypresentationlistbox-create.md)|[groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)|新しい[Grouppolicypresentationlistbox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)オブジェクトを作成します。|
|[GroupPolicyPresentationListBox の削除](../api/intune-grouppolicy-grouppolicypresentationlistbox-delete.md)|None|[Grouppolicypresentationlistbox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)を削除します。|
|[GroupPolicyPresentationListBox の更新](../api/intune-grouppolicy-grouppolicypresentationlistbox-update.md)|[groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)|[Grouppolicypresentationlistbox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|label|String|任意のプレゼンテーションエンティティのローカライズされたテキストラベル。 既定値は空白です。 [GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。|
|id|String|エンティティのキー。 [GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。|
|lastModifiedDateTime|DateTimeOffset|エンティティが最後に変更された日付と時刻。 [GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。|
|explicitValue|Boolean|このオプションが指定されている場合、ユーザーはレジストリサブキーの値とレジストリサブキー名を指定する必要があります。 リストボックスに2つの列が表示されます。1つは名前用、もう1つはデータ用です。 既定値は false です。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|definition|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|プレゼンテーションに関連付けられたグループポリシーの定義。 [GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。|

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





