---
title: enrollmentTroubleshootingEvent リソースの種類
description: 登録エラーを表すイベント。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b17cb948e67fa178c9839b95eebebe50d4a5b486
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036712"
---
# <a name="enrollmenttroubleshootingevent-resource-type"></a>enrollmentTroubleshootingEvent リソースの種類

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

登録エラーを表すイベント。


[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) からの継承

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[List enrollmentTroubleshootingEvents](../api/intune-troubleshooting-enrollmenttroubleshootingevent-list.md)|[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) コレクション|[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[Get enrollmentTroubleshootingEvent](../api/intune-troubleshooting-enrollmenttroubleshootingevent-get.md)|[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)|[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Create enrollmentTroubleshootingEvent](../api/intune-troubleshooting-enrollmenttroubleshootingevent-create.md)|[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)|新しい [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) オブジェクトを作成します。|
|[Delete enrollmentTroubleshootingEvent](../api/intune-troubleshooting-enrollmenttroubleshootingevent-delete.md)|なし|[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) を削除します。|
|[Update enrollmentTroubleshootingEvent](../api/intune-troubleshooting-enrollmenttroubleshootingevent-update.md)|[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)|[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|オブジェクトの UUID。[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承|
|eventDateTime|DateTimeOffset|インシデントが発生した時間。 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承します|
|correlationId|String|サービスのエラーをトレースするための ID。 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承します|
|managedDeviceIdentifier|String|Intune によって作成または収集されるデバイス識別子。|
|operatingSystem|文字列|オペレーティング システム。|
|osVersion|String|OS バージョン。|
|userId|String|デバイスを登録しようとするユーザーの識別子。|
|deviceId|String|Azure AD デバイス識別子。|
|enrollmentType|[deviceEnrollmentType](../resources/intune-shared-deviceenrollmenttype.md)|登録の種類。 可能な値は、`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement` です。|
|failureCategory|[deviceEnrollmentFailureReason](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|高レベルのエラー カテゴリ。 可能な値は、`unknown`、`authentication`、`authorization`、`accountValidation`、`userValidation`、`deviceNotSupported`、`inMaintenance`、`badRequest`、`featureNotSupported`、`enrollmentRestrictionsEnforced`、`clientDisconnected`、`userAbandonment` です。|
|failureReason|String|詳細なエラーの理由:|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.enrollmentTroubleshootingEvent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.enrollmentTroubleshootingEvent",
  "id": "String (identifier)",
  "eventDateTime": "String (timestamp)",
  "correlationId": "String",
  "managedDeviceIdentifier": "String",
  "operatingSystem": "String",
  "osVersion": "String",
  "userId": "String",
  "deviceId": "String",
  "enrollmentType": "String",
  "failureCategory": "String",
  "failureReason": "String"
}
```



