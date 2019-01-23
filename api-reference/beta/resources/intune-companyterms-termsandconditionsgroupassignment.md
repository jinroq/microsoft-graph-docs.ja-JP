---
title: termsAndConditionsGroupAssignment リソースの種類
description: TermsAndConditionsGroupAssignment エンティティの割り当てを表す、条項および条件 (T&C) を指定する特定のグループ ポリシー。 グループ内のユーザーは、デバイスを Intune に登録するためには使用条件に同意する必要があります。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0cdb629c380898af078bf0b5eaeb3c39344a5657
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418576"
---
# <a name="termsandconditionsgroupassignment-resource-type"></a>termsAndConditionsGroupAssignment リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

TermsAndConditionsGroupAssignment エンティティの割り当てを表す、条項および条件 (T&C) を指定する特定のグループ ポリシー。 グループ内のユーザーは、デバイスを Intune に登録するためには使用条件に同意する必要があります。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト termsAndConditionsGroupAssignments](../api/intune-companyterms-termsandconditionsgroupassignment-list.md)|[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)コレクション|[TermsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)オブジェクトのプロパティと関係を一覧表示します。|
|[TermsAndConditionsGroupAssignment を取得します。](../api/intune-companyterms-termsandconditionsgroupassignment-get.md)|[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|[TermsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)オブジェクトのプロパティと関係を参照してください。|
|[TermsAndConditionsGroupAssignment を作成します。](../api/intune-companyterms-termsandconditionsgroupassignment-create.md)|[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|新しい[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)オブジェクトを作成します。|
|[TermsAndConditionsGroupAssignment を削除します。](../api/intune-companyterms-termsandconditionsgroupassignment-delete.md)|なし|の[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)を削除します。|
|[TermsAndConditionsGroupAssignment を更新します。](../api/intune-companyterms-termsandconditionsgroupassignment-update.md)|[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|[TermsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティの一意識別子。|
|targetGroupId|String|T&C ポリシーが割り当てられているグループの一意の識別子です。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|termsAndConditions|[termsAndConditions](../resources/intune-companyterms-termsandconditions.md)|割り当てられた使用条件へのナビゲーション リンク。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditionsGroupAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termsAndConditionsGroupAssignment",
  "id": "String (identifier)",
  "targetGroupId": "String"
}
```




