---
title: iosVppAppAssignedDeviceLicense リソースの種類
description: iOS ボリューム購入プログラムのデバイス割り当てのライセンスを取得します。 このクラスは、作成、削除、更新をサポートしていません。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b18415b3a2d25990bc7202d96fc35f3289b56f4a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29393614"
---
# <a name="iosvppappassigneddevicelicense-resource-type"></a>iosVppAppAssignedDeviceLicense リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

iOS ボリューム購入プログラムのデバイス割り当てのライセンスを取得します。 このクラスは、作成、削除、更新をサポートしていません。


[IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト iosVppAppAssignedDeviceLicenses](../api/intune-apps-iosvppappassigneddevicelicense-list.md)|[iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)コレクション|[IosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)オブジェクトのプロパティと関係を一覧表示します。|
|[IosVppAppAssignedDeviceLicense を取得します。](../api/intune-apps-iosvppappassigneddevicelicense-get.md)|[iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)|[IosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)オブジェクトのプロパティと関係を参照してください。|
|[IosVppAppAssignedDeviceLicense を作成します。](../api/intune-apps-iosvppappassigneddevicelicense-create.md)|[iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)|新しい[iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)オブジェクトを作成します。|
|[IosVppAppAssignedDeviceLicense を削除します。](../api/intune-apps-iosvppappassigneddevicelicense-delete.md)|なし|の[iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)を削除します。|
|[IosVppAppAssignedDeviceLicense を更新します。](../api/intune-apps-iosvppappassigneddevicelicense-update.md)|[iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)|[IosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。 [IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承されました。|
|userEmailAddress|String|ユーザーの電子メール アドレスです。 [IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承されました。|
|userId|String|ユーザー id。 [IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承されました。|
|userName|String|ユーザー名。 [IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承されました。|
|userPrincipalName|String|ユーザー プリンシパル名。 [IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承されました。|
|managedDeviceId|String|管理対象デバイスの id。|
|deviceName|String|デバイスの名前。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosVppAppAssignedDeviceLicense"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppAppAssignedDeviceLicense",
  "id": "String (identifier)",
  "userEmailAddress": "String",
  "userId": "String",
  "userName": "String",
  "userPrincipalName": "String",
  "managedDeviceId": "String",
  "deviceName": "String"
}
```




