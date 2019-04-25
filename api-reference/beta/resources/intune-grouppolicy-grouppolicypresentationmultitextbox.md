---
title: grouppolicypresentationmultitextbox リソースの種類
description: admx multitextbox 要素と admx multitextbox 要素を表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0f17177b55d6033b35c4476e9df61150e785ba45
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32575878"
---
# <a name="grouppolicypresentationmultitextbox-resource-type"></a>grouppolicypresentationmultitextbox リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

admx multitextbox 要素と admx multitextbox 要素を表します。


[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[grouppolicypresentationmultitextboxes ボックスのリスト](../api/intune-grouppolicy-grouppolicypresentationmultitextbox-list.md)|[grouppolicypresentationmultitextbox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)コレクション|[grouppolicypresentationmultitextbox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[grouppolicypresentationmultitextbox の取得](../api/intune-grouppolicy-grouppolicypresentationmultitextbox-get.md)|[grouppolicypresentationmultitextbox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)|[grouppolicypresentationmultitextbox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[grouppolicypresentationmultitextbox の作成](../api/intune-grouppolicy-grouppolicypresentationmultitextbox-create.md)|[grouppolicypresentationmultitextbox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)|新しい[grouppolicypresentationmultitextbox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)オブジェクトを作成します。|
|[grouppolicypresentationmultitextbox の削除](../api/intune-grouppolicy-grouppolicypresentationmultitextbox-delete.md)|なし|[grouppolicypresentationmultitextbox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)を削除します。|
|[grouppolicypresentationmultitextbox の更新](../api/intune-grouppolicy-grouppolicypresentationmultitextbox-update.md)|[grouppolicypresentationmultitextbox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)|[grouppolicypresentationmultitextbox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|label|String|任意のプレゼンテーションエンティティのローカライズされたテキストラベル。 既定値は空白です。 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。|
|id|String|エンティティのキー。 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。|
|lastModifiedDateTime|DateTimeOffset|エンティティが最後に変更された日付と時刻。 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。|
|必須|Boolean|テキストボックスに値を入力する必要があります。 既定値は False です。|
|maxLength|Int64|テキストの最大文字数を指定する符号なし整数。 既定値は1023です。|
|maxstrings|Int64|文字列の最大数を指定する符号なし整数。 既定値は 0 です。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|definition|[grouppolicydefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|プレゼンテーションに関連付けられたグループポリシーの定義。 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationMultiTextBox"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationMultiTextBox",
  "label": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "required": true,
  "maxLength": 1024,
  "maxStrings": 1024
}
```





