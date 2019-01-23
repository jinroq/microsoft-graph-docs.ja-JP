---
title: outOfBoxExperienceSettings リソースの種類
description: ボックスの設定が発生します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5d2b48fef00c9c3a291a0a2fdfe680b9f4e21030
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404604"
---
# <a name="outofboxexperiencesettings-resource-type"></a>outOfBoxExperienceSettings リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

ボックスの設定が発生します。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|hidePrivacySettings|Boolean|ユーザーのプライバシー設定の表示と非表示を切り替える|
|hideEULA|Boolean|ユーザーに使用許諾契約書の表示と非表示を切り替える|
|userType|[windowsUserType](../resources/intune-enrollment-windowsusertype.md)|ユーザーの種類です。 使用可能な値は、`administrator`、`standard` です。|
|deviceUsageType|[windowsDeviceUsageType](../resources/intune-enrollment-windowsdeviceusagetype.md)|AAD の結合の認証の種類です。 使用可能な値は、`singleUser`、`shared` です。|
|skipKeyboardSelectionPage|Boolean|かどうか、セット、キーボードの選択をスキップするページの言語と地域が設定されている場合|
|hideEscapeLink|Boolean|ユーザーでは、true に設定を別のアカウントでのサインインの会社経由で起動できない場合|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.outOfBoxExperienceSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.outOfBoxExperienceSettings",
  "hidePrivacySettings": true,
  "hideEULA": true,
  "userType": "String",
  "deviceUsageType": "String",
  "skipKeyboardSelectionPage": true,
  "hideEscapeLink": true
}
```




