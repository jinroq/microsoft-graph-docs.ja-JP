---
title: windows10EnrollmentCompletionPageConfiguration リソースの種類
description: Windows 10 の登録ステータスページの構成
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7d8b60a1c2afcaccef95caef77f0bda6d3cd65a9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566382"
---
# <a name="windows10enrollmentcompletionpageconfiguration-resource-type"></a>windows10EnrollmentCompletionPageConfiguration リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Windows 10 の登録ステータスページの構成


[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) からの継承

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト windows10EnrollmentCompletionPageConfigurations](../api/intune-onboarding-windows10enrollmentcompletionpageconfiguration-list.md)|[windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)コレクション|[windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[windows10EnrollmentCompletionPageConfiguration を取得する](../api/intune-onboarding-windows10enrollmentcompletionpageconfiguration-get.md)|[windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)|[windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[windows10EnrollmentCompletionPageConfiguration を作成する](../api/intune-onboarding-windows10enrollmentcompletionpageconfiguration-create.md)|[windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)|新しい[windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)オブジェクトを作成します。|
|[windows10EnrollmentCompletionPageConfiguration の削除](../api/intune-onboarding-windows10enrollmentcompletionpageconfiguration-delete.md)|なし|[windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)を削除します。|
|[windows10EnrollmentCompletionPageConfiguration の更新](../api/intune-onboarding-windows10enrollmentcompletionpageconfiguration-update.md)|[windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)|[windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承された登録ステータスページの構成の Id|
|displayName|String|まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します|
|説明|String|まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します|
|priority|Int32|まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します|
|createdDateTime|DateTimeOffset|まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します|
|version|Int32|まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) から継承します|
|showinstallationprogress|Boolean|ユーザーにインストールの進行状況を表示または非表示にする|
|blockdevicesetupretrybyuser|Boolean|ユーザーがインストールエラー時にセットアップを再試行できるようにする|
|allowdeviceresetoninstallfailure|Boolean|インストール失敗時にデバイスのリセットを許可またはブロックする|
|allowlogcollectiononinstallfailure|Boolean|インストール失敗時にログ収集を許可またはブロックする|
|customerrormessage|String|インストールエラーが発生したときに表示するカスタムエラーメッセージを設定する|
|installProgressTimeoutInMinutes|Int32|インストールの進行状況のタイムアウトを分単位で設定する|
|allowdeviceuseoninstallfailure|Boolean|インストールエラー時にユーザーがデバイスを引き続き使用できるようにする|
|selectedMobileAppIds|String collection|インストールの状態を追跡するために選択されたアプリケーション|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|assignments|[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) コレクション|デバイスの構成プロファイルのグループ割り当てのリストです。 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) からの継承|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows10EnrollmentCompletionPageConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10EnrollmentCompletionPageConfiguration",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "priority": 1024,
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "version": 1024,
  "showInstallationProgress": true,
  "blockDeviceSetupRetryByUser": true,
  "allowDeviceResetOnInstallFailure": true,
  "allowLogCollectionOnInstallFailure": true,
  "customErrorMessage": "String",
  "installProgressTimeoutInMinutes": 1024,
  "allowDeviceUseOnInstallFailure": true,
  "selectedMobileAppIds": [
    "String"
  ]
}
```





