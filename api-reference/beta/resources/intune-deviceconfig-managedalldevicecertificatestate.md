---
title: managedAllDeviceCertificateState リソースの種類
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: aaf13c6c29668b2cf21bd4ce282c71773de69133
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36368878"
---
# <a name="managedalldevicecertificatestate-resource-type"></a>managedAllDeviceCertificateState リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

まだ文書化されていません

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト managedAllDeviceCertificateStates](../api/intune-deviceconfig-managedalldevicecertificatestate-list.md)|[managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)コレクション|[ManagedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[ManagedAllDeviceCertificateState を取得する](../api/intune-deviceconfig-managedalldevicecertificatestate-get.md)|[managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)|[ManagedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[ManagedAllDeviceCertificateState を作成する](../api/intune-deviceconfig-managedalldevicecertificatestate-create.md)|[managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)|新しい[managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)オブジェクトを作成します。|
|[ManagedAllDeviceCertificateState の削除](../api/intune-deviceconfig-managedalldevicecertificatestate-delete.md)|None|[ManagedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)を削除します。|
|[ManagedAllDeviceCertificateState の更新](../api/intune-deviceconfig-managedalldevicecertificatestate-update.md)|[managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)|[ManagedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|エンティティのキー。|
|certificateRevokeStatus|[certificateRevocationStatus](../resources/intune-deviceconfig-certificaterevocationstatus.md)|状態を取り消します。 可能な値は、`none`、`pending`、`issued`、`failed`、`revoked` です。|
|managedDeviceDisplayName|String|デバイスの表示名|
|userPrincipalName|String|ユーザー プリンシパル名|
|certificateExpirationDateTime|DateTimeOffset|証明書の有効期限|
|Certificate/Ername|String|発行者|
|certificateThumbprint|String|拇印|
|certificateSerialNumber|String|シリアル番号|
|certificateSubjectName|String|証明書のサブジェクト名|
|certificateKeyUsages|Int32|キー使用法|
|certificateExtendedKeyUsages|String|拡張キー使用法|
|certificateIssuanceDateTime|DateTimeOffset|発行日|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAllDeviceCertificateState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAllDeviceCertificateState",
  "id": "String (identifier)",
  "certificateRevokeStatus": "String",
  "managedDeviceDisplayName": "String",
  "userPrincipalName": "String",
  "certificateExpirationDateTime": "String (timestamp)",
  "certificateIssuerName": "String",
  "certificateThumbprint": "String",
  "certificateSerialNumber": "String",
  "certificateSubjectName": "String",
  "certificateKeyUsages": 1024,
  "certificateExtendedKeyUsages": "String",
  "certificateIssuanceDateTime": "String (timestamp)"
}
```



