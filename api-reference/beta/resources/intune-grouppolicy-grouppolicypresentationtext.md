---
title: grouppolicypresentationtext リソースの種類
description: ADMX text 要素を表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3fd411b0a8fc8e9ed623a0070e1f670a146970cc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32575864"
---
# <a name="grouppolicypresentationtext-resource-type"></a>grouppolicypresentationtext リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

ADMX text 要素を表します。


[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[grouppolicypresentationtexts を一覧表示する](../api/intune-grouppolicy-grouppolicypresentationtext-list.md)|[grouppolicypresentationtext](../resources/intune-grouppolicy-grouppolicypresentationtext.md)コレクション|[grouppolicypresentationtext](../resources/intune-grouppolicy-grouppolicypresentationtext.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[grouppolicypresentationtext の取得](../api/intune-grouppolicy-grouppolicypresentationtext-get.md)|[grouppolicypresentationtext](../resources/intune-grouppolicy-grouppolicypresentationtext.md)|[grouppolicypresentationtext](../resources/intune-grouppolicy-grouppolicypresentationtext.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[grouppolicypresentationtext の作成](../api/intune-grouppolicy-grouppolicypresentationtext-create.md)|[grouppolicypresentationtext](../resources/intune-grouppolicy-grouppolicypresentationtext.md)|新しい[grouppolicypresentationtext](../resources/intune-grouppolicy-grouppolicypresentationtext.md)オブジェクトを作成します。|
|[grouppolicypresentationtext の削除](../api/intune-grouppolicy-grouppolicypresentationtext-delete.md)|なし|[grouppolicypresentationtext](../resources/intune-grouppolicy-grouppolicypresentationtext.md)を削除します。|
|[grouppolicypresentationtext の更新](../api/intune-grouppolicy-grouppolicypresentationtext-update.md)|[grouppolicypresentationtext](../resources/intune-grouppolicy-grouppolicypresentationtext.md)|[grouppolicypresentationtext](../resources/intune-grouppolicy-grouppolicypresentationtext.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|label|String|任意のプレゼンテーションエンティティのローカライズされたテキストラベル。 既定値は空白です。 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。|
|id|String|エンティティのキー。 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。|
|lastModifiedDateTime|DateTimeOffset|エンティティが最後に変更された日付と時刻。 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|definition|[grouppolicydefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|プレゼンテーションに関連付けられたグループポリシーの定義。 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationText"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationText",
  "label": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```





