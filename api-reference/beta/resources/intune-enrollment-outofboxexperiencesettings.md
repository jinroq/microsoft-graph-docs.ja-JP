---
title: outOfBoxExperienceSettings リソースの種類
description: ボックスの設定が発生します。
author: tfitzmac
ms.openlocfilehash: 545fbe5c27063397a4d08c40729227804ebfc56d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308408"
---
# <a name="outofboxexperiencesettings-resource-type"></a>outOfBoxExperienceSettings リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

ボックスの設定が発生します。
## <a name="properties"></a>Properties
|プロパティ|種類|説明|
|:---|:---|:---|
|hidePrivacySettings|ブール型|ユーザーのプライバシー設定の表示と非表示を切り替える|
|hideEULA|ブール型|ユーザーに使用許諾契約書の表示と非表示を切り替える|
|userType|[windowsUserType](../resources/intune-enrollment-windowsusertype.md)|ユーザーの種類です。 使用可能な値は、`administrator`、`standard` です。|
|deviceUsageType|[windowsDeviceUsageType](../resources/intune-enrollment-windowsdeviceusagetype.md)|AAD の結合の認証の種類です。 使用可能な値は、`singleUser`、`shared` です。|
|skipKeyboardSelectionPage|ブール型|かどうか、セット、キーボードの選択をスキップするページの言語と地域が設定されている場合|
|hideEscapeLink|ブール型|ユーザーでは、true に設定を別のアカウントでのサインインの会社経由で起動できない場合|

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





