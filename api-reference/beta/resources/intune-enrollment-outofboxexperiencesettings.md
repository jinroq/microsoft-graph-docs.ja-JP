---
title: outOfBoxExperienceSettings リソースの種類
description: 不在時の環境設定
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fb8a3c0358343a3d1051258188028ffa5c1f0293
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941500"
---
# <a name="outofboxexperiencesettings-resource-type"></a>outOfBoxExperienceSettings リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

不在時の環境設定

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|hidePrivacySettings|Boolean|ユーザーのプライバシー設定を表示または非表示にする|
|hideEULA|Boolean|ユーザーに EULA を表示または非表示にする|
|userType|[windowsUserType](../resources/intune-enrollment-windowsusertype.md)|ユーザーの種類。 可能な値は、`administrator`、`standard` です。|
|deviceUsageType|[windowsDeviceUsageType](../resources/intune-enrollment-windowsdeviceusagetype.md)|AAD 参加認証の種類。 可能な値は、`singleUser`、`shared` です。|
|Skipキーボードの Selectionpage|Boolean|設定されている場合は、言語と地域が設定されている場合は、キーボードの選択ページをスキップします。|
|hideEscapeLink|Boolean|True に設定されている場合、ユーザーは別のアカウントを使用してサインインすることはできません (会社のサインイン時)。|

## <a name="relationships"></a>関係
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




