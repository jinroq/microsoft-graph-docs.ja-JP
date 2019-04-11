---
title: windowsEnrollmentStatusScreenSettings リソースの種類
description: 登録の状態画面の設定
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 18c947bbfc7e11ba4acef967171f77a7806b3509
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31772798"
---
# <a name="windowsenrollmentstatusscreensettings-resource-type"></a>windowsEnrollmentStatusScreenSettings リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

登録の状態画面の設定

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|hideinstallationprogress 進行状況|Boolean|ユーザーにインストールの進行状況を表示または非表示にする|
|allowdeviceusebeforeprofileandappinstallcomplete|Boolean|プロファイルとアプリのインストールが完了する前にユーザーがデバイスを使用することを許可またはブロックする|
|blockdevicesetupretrybyuser|Boolean|ユーザーがインストールエラー時にセットアップを再試行できるようにする|
|allowlogcollectiononinstallfailure|Boolean|インストール失敗時にログ収集を許可またはブロックする|
|customerrormessage|文字列|インストールエラーが発生したときに表示するカスタムエラーメッセージを設定する|
|installProgressTimeoutInMinutes|Int32|インストールの進行状況のタイムアウトを分単位で設定する|
|allowdeviceuseoninstallfailure|Boolean|インストールエラー時にユーザーがデバイスを引き続き使用できるようにする|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsEnrollmentStatusScreenSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsEnrollmentStatusScreenSettings",
  "hideInstallationProgress": true,
  "allowDeviceUseBeforeProfileAndAppInstallComplete": true,
  "blockDeviceSetupRetryByUser": true,
  "allowLogCollectionOnInstallFailure": true,
  "customErrorMessage": "String",
  "installProgressTimeoutInMinutes": 1024,
  "allowDeviceUseOnInstallFailure": true
}
```





