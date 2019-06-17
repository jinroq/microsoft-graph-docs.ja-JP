---
title: iosVppAppAssignedDeviceLicense リソースの種類
description: iOS Volume Purchase Program デバイスライセンスの割り当て。 このクラスは、作成、削除、更新をサポートしていません。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6236b6f1d65a5b1d07a70407554f5af7b344258c
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34979327"
---
# <a name="iosvppappassigneddevicelicense-resource-type"></a>iosVppAppAssignedDeviceLicense リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

iOS Volume Purchase Program デバイスライセンスの割り当て。 このクラスは、作成、削除、更新をサポートしていません。


[IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト iosVppAppAssignedDeviceLicenses](../api/intune-apps-iosvppappassigneddevicelicense-list.md)|[iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)コレクション|[IosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[IosVppAppAssignedDeviceLicense を取得する](../api/intune-apps-iosvppappassigneddevicelicense-get.md)|[iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)|[IosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[IosVppAppAssignedDeviceLicense を作成する](../api/intune-apps-iosvppappassigneddevicelicense-create.md)|[iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)|新しい[iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)オブジェクトを作成します。|
|[IosVppAppAssignedDeviceLicense の削除](../api/intune-apps-iosvppappassigneddevicelicense-delete.md)|None|[IosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)を削除します。|
|[IosVppAppAssignedDeviceLicense の更新](../api/intune-apps-iosvppappassigneddevicelicense-update.md)|[iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)|[IosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|エンティティのキー。 [IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承します。|
|userEmailAddress|String|ユーザーの電子メールアドレス。 [IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承します。|
|userId|String|ユーザー ID。 [IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承します。|
|userName|String|ユーザー名。 [IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承します。|
|userPrincipalName|String|ユーザー プリンシパル名。 [IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承します。|
|managedDeviceId|String|管理されているデバイス ID。|
|deviceName|String|デバイス名。|

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





