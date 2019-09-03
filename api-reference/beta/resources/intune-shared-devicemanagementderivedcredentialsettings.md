---
title: deviceManagementDerivedCredentialSettings リソースの種類
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8cbf9ae512659459035faf5938e3eae2dd2f09d3
ms.sourcegitcommit: 0f3e0bd7b57870a0f7b34cf52eaf4776ac82671e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/31/2019
ms.locfileid: "36699538"
---
# <a name="devicemanagementderivedcredentialsettings-resource-type"></a>deviceManagementDerivedCredentialSettings リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

DeviceManagementDerivedCredentialSettings リソースは、次のようなワークフローに従ってコンテンツが変化するコンテナーを表します。  

- デバイス構成の設定
- RA ポリシー

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[DeviceManagementDerivedCredentialSettings を取得する](../api/intune-shared-devicemanagementderivedcredentialsettings-get.md)|[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)|[DeviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[DeviceManagementDerivedCredentialSettings の更新](../api/intune-shared-devicemanagementderivedcredentialsettings-update.md)|[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)|[DeviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)オブジェクトのプロパティを更新します。|
|**リソースアクセスポリシー**|
|[リスト deviceManagementDerivedCredentialSettingses](../api/intune-shared-devicemanagementderivedcredentialsettings-list.md)|[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)コレクション|[DeviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[DeviceManagementDerivedCredentialSettings を作成する](../api/intune-shared-devicemanagementderivedcredentialsettings-create.md)|[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)|新しい[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)オブジェクトを作成します。|
|[DeviceManagementDerivedCredentialSettings の削除](../api/intune-shared-devicemanagementderivedcredentialsettings-delete.md)|None|[DeviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)を削除します。|


## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|派生した資格情報の一意識別子|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementDerivedCredentialSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementDerivedCredentialSettings",
  "id": "String (identifier)"
}
```



