---
title: sideLoadingKey リソースの種類
description: SideLoadingKey エンティティは、テナントの基幹業務アプリを intall するために Windows 8 および8.1 デバイスに必要です。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 036944ea41ee9b180247577c7c56c2055b33fc2a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010715"
---
# <a name="sideloadingkey-resource-type"></a>sideLoadingKey リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

SideLoadingKey エンティティは、テナントの基幹業務アプリを intall するために Windows 8 および8.1 デバイスに必要です。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト sideLoadingKeies](../api/intune-onboarding-sideloadingkey-list.md)|[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)コレクション|[SideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[SideLoadingKey を取得する](../api/intune-onboarding-sideloadingkey-get.md)|[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)|[SideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[SideLoadingKey を作成する](../api/intune-onboarding-sideloadingkey-create.md)|[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)|新しい[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)オブジェクトを作成します。|
|[SideLoadingKey の削除](../api/intune-onboarding-sideloadingkey-delete.md)|None|[SideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)を削除します。|
|[SideLoadingKey の更新](../api/intune-onboarding-sideloadingkey-update.md)|[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)|[SideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|サイドローディングキーの一意 Id。|
|value|文字列|サイドローディングキー値は、5 x 5 の値で、hiphens で区切られています。|
|displayName|String|ITPro 管理者に表示されるサイドローディングキー名。|
|description|String|ITPro 管理者に表示されるサイドローディングキーの説明。|
|totalActivation|Int32|ITPro 管理者に表示されるサイドローディングキーの合計です。|
|lastUpdatedDateTime|String|サイドローディングキー最終更新日が ITPro の管理者に表示されます。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.sideLoadingKey"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sideLoadingKey",
  "id": "String (identifier)",
  "value": "String",
  "displayName": "String",
  "description": "String",
  "totalActivation": 1024,
  "lastUpdatedDateTime": "String"
}
```





