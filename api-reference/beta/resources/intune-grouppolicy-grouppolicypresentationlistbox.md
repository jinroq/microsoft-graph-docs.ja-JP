---
title: grouppolicypresentationlistbox リソースの種類
description: admx listBox 要素と admx list 要素を表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6c2318a827e4056fac2f6b984ddf4e43405a06c2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32575766"
---
# <a name="grouppolicypresentationlistbox-resource-type"></a>grouppolicypresentationlistbox リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

admx listBox 要素と admx list 要素を表します。


[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト grouppolicypresentationlistboxes ボックス](../api/intune-grouppolicy-grouppolicypresentationlistbox-list.md)|[grouppolicypresentationlistbox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)コレクション|[grouppolicypresentationlistbox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[grouppolicypresentationlistbox の取得](../api/intune-grouppolicy-grouppolicypresentationlistbox-get.md)|[grouppolicypresentationlistbox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)|[grouppolicypresentationlistbox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[grouppolicypresentationlistbox の作成](../api/intune-grouppolicy-grouppolicypresentationlistbox-create.md)|[grouppolicypresentationlistbox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)|新しい[grouppolicypresentationlistbox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)オブジェクトを作成します。|
|[grouppolicypresentationlistbox の削除](../api/intune-grouppolicy-grouppolicypresentationlistbox-delete.md)|なし|[grouppolicypresentationlistbox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)を削除します。|
|[grouppolicypresentationlistbox の更新](../api/intune-grouppolicy-grouppolicypresentationlistbox-update.md)|[grouppolicypresentationlistbox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)|[grouppolicypresentationlistbox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|label|String|任意のプレゼンテーションエンティティのローカライズされたテキストラベル。 既定値は空白です。 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。|
|id|String|エンティティのキー。 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。|
|lastModifiedDateTime|DateTimeOffset|エンティティが最後に変更された日付と時刻。 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。|
|explicitValue|Boolean|このオプションが指定されている場合、ユーザーはレジストリサブキーの値とレジストリサブキー名を指定する必要があります。 リストボックスに2つの列が表示されます。1つは名前用、もう1つはデータ用です。 既定値は false です。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|definition|[grouppolicydefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|プレゼンテーションに関連付けられたグループポリシーの定義。 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。|

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





