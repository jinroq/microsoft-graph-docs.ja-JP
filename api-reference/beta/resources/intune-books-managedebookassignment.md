---
title: managedEBookAssignment リソースの種類
description: グループへの電子ブックの割り当てに使用されるプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 325e094698bb2ccbfaf4c41dd46f71c461c8681f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32541382"
---
# <a name="managedebookassignment-resource-type"></a>managedEBookAssignment リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

グループへの電子ブックの割り当てに使用されるプロパティが含まれています。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[managedEBookAssignments のリスト](../api/intune-books-managedebookassignment-list.md)|[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) コレクション|[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[managedEBookAssignment の取得](../api/intune-books-managedebookassignment-get.md)|[managedEBookAssignment](../resources/intune-books-managedebookassignment.md)|[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[managedEBookAssignment の作成](../api/intune-books-managedebookassignment-create.md)|[managedEBookAssignment](../resources/intune-books-managedebookassignment.md)|新しい [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) オブジェクトを作成します。|
|[managedEBookAssignment の削除](../api/intune-books-managedebookassignment-delete.md)|なし|[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) を削除します。|
|[managedEBookAssignment の更新](../api/intune-books-managedebookassignment-update.md)|[managedEBookAssignment](../resources/intune-books-managedebookassignment.md)|[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|電子ブックの割り当て先。|
|installIntent|[installIntent](../resources/intune-shared-installintent.md)|電子ブックのインストールの目的。 可能な値は、`available`、`required`、`uninstall`、`availableWithoutEnrollment` です。|

## <a name="relationships"></a>関係
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedEBookAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedEBookAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "String"
}
```





