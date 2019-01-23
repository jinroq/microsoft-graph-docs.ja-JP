---
title: intuneBrandingProfileAssignment リソースの種類
description: このエンティティには、ブランドのプロファイルをグループに割り当てるためのプロパティが含まれています。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: fcc0b625bc3918206a1d75ae7ef123484ae0357c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431613"
---
# <a name="intunebrandingprofileassignment-resource-type"></a>intuneBrandingProfileAssignment リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

このエンティティには、ブランドのプロファイルをグループに割り当てるためのプロパティが含まれています。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト intuneBrandingProfileAssignments](../api/intune-wip-intunebrandingprofileassignment-list.md)|[intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)コレクション|[IntuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)オブジェクトのプロパティと関係を一覧表示します。|
|[IntuneBrandingProfileAssignment を取得します。](../api/intune-wip-intunebrandingprofileassignment-get.md)|[intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)|[IntuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)オブジェクトのプロパティと関係を参照してください。|
|[IntuneBrandingProfileAssignment を作成します。](../api/intune-wip-intunebrandingprofileassignment-create.md)|[intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)|新しい[intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)オブジェクトを作成します。|
|[IntuneBrandingProfileAssignment を削除します。](../api/intune-wip-intunebrandingprofileassignment-delete.md)|なし|の[intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)を削除します。|
|[IntuneBrandingProfileAssignment を更新します。](../api/intune-wip-intunebrandingprofileassignment-update.md)|[intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)|[IntuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティの一意識別子。|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|割り当てのターゲットにブランドのプロファイルが割り当てられています。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.intuneBrandingProfileAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.intuneBrandingProfileAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




