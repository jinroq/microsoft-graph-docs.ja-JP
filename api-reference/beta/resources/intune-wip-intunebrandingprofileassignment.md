---
title: intuneBrandingProfileAssignment リソースの種類
description: このエンティティには、ブランド化プロファイルをグループに割り当てるために使用されるプロパティが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 41e18a93b32d646501af1da62c07bb5764ea1f89
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36356586"
---
# <a name="intunebrandingprofileassignment-resource-type"></a>intuneBrandingProfileAssignment リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

このエンティティには、ブランド化プロファイルをグループに割り当てるために使用されるプロパティが含まれています。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト intuneBrandingProfileAssignments](../api/intune-wip-intunebrandingprofileassignment-list.md)|[intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)コレクション|[IntuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[IntuneBrandingProfileAssignment を取得する](../api/intune-wip-intunebrandingprofileassignment-get.md)|[intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)|[IntuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[IntuneBrandingProfileAssignment を作成する](../api/intune-wip-intunebrandingprofileassignment-create.md)|[intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)|新しい[intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)オブジェクトを作成します。|
|[IntuneBrandingProfileAssignment の削除](../api/intune-wip-intunebrandingprofileassignment-delete.md)|None|[IntuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)を削除します。|
|[IntuneBrandingProfileAssignment の更新](../api/intune-wip-intunebrandingprofileassignment-update.md)|[intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)|[IntuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティの一意識別子。|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|ブランド化プロファイルが割り当てられている割り当て先。|

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



