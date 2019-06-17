---
title: deviceManagementDerivedCredentialSettings リソースの種類
description: 派生した資格情報のテナントレベルの設定を記述するエンティティ
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 06f87b7c2f94bcd95d27889bfb9ee0649c4aae92
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34990023"
---
# <a name="devicemanagementderivedcredentialsettings-resource-type"></a>deviceManagementDerivedCredentialSettings リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

派生した資格情報のテナントレベルの設定を記述するエンティティ

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[DeviceManagementDerivedCredentialSettings を取得する](../api/intune-deviceconfig-devicemanagementderivedcredentialsettings-get.md)|[deviceManagementDerivedCredentialSettings](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md)|[DeviceManagementDerivedCredentialSettings](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[DeviceManagementDerivedCredentialSettings の更新](../api/intune-deviceconfig-devicemanagementderivedcredentialsettings-update.md)|[deviceManagementDerivedCredentialSettings](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md)|[DeviceManagementDerivedCredentialSettings](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|派生した資格情報の一意識別子|
|helpUrl|String|エンドユーザーが会社のポータルを使用して派生した資格情報を取得するときに、エンドユーザーがアクセスできる URL。|
|displayName|String|プロファイルの表示名。|
|会社|[deviceManagementDerivedCredentialIssuer](../resources/intune-deviceconfig-devicemanagementderivedcredentialissuer.md)|使用する派生資格情報プロバイダー。 可能な値は、`intercede`、`entrustDatacard`、`purebred` です。|
|notificationType|[deviceManagementDerivedCredentialNotificationType](../resources/intune-deviceconfig-devicemanagementderivedcredentialnotificationtype.md)|デバイスに証明書を使用する、Wi-fi、VPN、または電子メールプロファイルを配信するために、会社のポータルを開くことをエンドユーザーに通知するために使用されるメソッド。 可能な値は、`none`、`companyPortal`、`email` です。|

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
  "id": "String (identifier)",
  "helpUrl": "String",
  "displayName": "String",
  "issuer": "String",
  "notificationType": "String"
}
```





