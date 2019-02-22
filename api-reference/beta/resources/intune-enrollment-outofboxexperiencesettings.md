---
title: outOfBoxExperienceSettings リソースの種類
description: 不在時の環境設定
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1148ba609a6533dcc6cedb9abd50e9191dceb5d2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145529"
---
# <a name="outofboxexperiencesettings-resource-type"></a>outOfBoxExperienceSettings リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

不在時の環境設定

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|hideprivacysettings|ブール値|ユーザーのプライバシー設定を表示または非表示にする|
|hideeula|ブール値|ユーザーに EULA を表示または非表示にする|
|userType|[windowsUserType](../resources/intune-enrollment-windowsusertype.md)|ユーザーの種類。 使用可能な値は、`administrator`、`standard` です。|
|deviceUsageType|[windowsDeviceUsageType](../resources/intune-enrollment-windowsdeviceusagetype.md)|AAD 参加認証の種類。 使用可能な値は、`singleUser`、`shared` です。|
|skipキーボードの selectionpage|ブール値|設定されている場合は、言語と地域が設定されている場合は、キーボードの選択ページをスキップします。|
|hideEscapeLink|ブール値|true に設定されている場合、ユーザーは別のアカウントを使用してサインインすることはできません (会社のサインイン時)。|

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




