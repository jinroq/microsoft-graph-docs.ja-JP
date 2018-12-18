---
title: iosVppEBookAssignment リソースの種類
description: グループへの iOS VPP 電子ブックの割り当てに使用されるプロパティが含まれています。
author: tfitzmac
ms.openlocfilehash: 1383c3370c7074e615d9b95300bbd57d940fc81f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314274"
---
# <a name="iosvppebookassignment-resource-type"></a>iosVppEBookAssignment リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

グループへの iOS VPP 電子ブックの割り当てに使用されるプロパティが含まれています。

[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[iosVppEBookAssignments のリスト](../api/intune-books-iosvppebookassignment-list.md)|[iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) コレクション|[iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[iosVppEBookAssignment の取得](../api/intune-books-iosvppebookassignment-get.md)|[iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md)|[iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[iosVppEBookAssignment の作成](../api/intune-books-iosvppebookassignment-create.md)|[iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md)|新しい [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) オブジェクトを作成します。|
|[iosVppEBookAssignment の削除](../api/intune-books-iosvppebookassignment-delete.md)|なし|[iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) を削除します。|
|[iosVppEBookAssignment の更新](../api/intune-books-iosvppebookassignment-update.md)|[iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md)|[iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) のプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|ID|String|エンティティのキー。 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) から継承します|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|電子ブックの割り当て先。 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) から継承します|
|installIntent|[installIntent](../resources/intune-shared-installintent.md)|電子ブックのインストールの目的。 [ManagedEBookAssignment](../resources/intune-books-managedebookassignment.md)から継承されます。 可能な値は、`available`、`required`、`uninstall`、`availableWithoutEnrollment` です。|

## <a name="relationships"></a>関係
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosVppEBookAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppEBookAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "String"
}
```





