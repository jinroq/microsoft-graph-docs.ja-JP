---
title: outOfBoxExperienceSettings リソースの種類
description: 不在時の環境設定
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0f465297f437f3710f8c789d8683794b7c9d5fa5
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31773512"
---
# <a name="outofboxexperiencesettings-resource-type"></a>outOfBoxExperienceSettings リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

不在時の環境設定

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|hideprivacysettings|Boolean|ユーザーのプライバシー設定を表示または非表示にする|
|hideeula|Boolean|ユーザーに EULA を表示または非表示にする|
|userType|[windowsUserType](../resources/intune-enrollment-windowsusertype.md)|ユーザーの種類。 可能な値は、`administrator`、`standard` です。|
|deviceUsageType|[windowsDeviceUsageType](../resources/intune-enrollment-windowsdeviceusagetype.md)|AAD 参加認証の種類。 可能な値は、`singleUser`、`shared` です。|
|skipキーボードの selectionpage|Boolean|設定されている場合は、言語と地域が設定されている場合は、キーボードの選択ページをスキップします。|
|hideEscapeLink|Boolean|true に設定されている場合、ユーザーは別のアカウントを使用してサインインすることはできません (会社のサインイン時)。|

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





