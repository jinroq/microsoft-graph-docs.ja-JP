---
title: windowsEnrollmentStatusScreenSettings リソースの種類
description: 登録の状態画面の設定
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d22f7497fb79921bbbf34c6f3334ccc2ae4d7d53
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34994903"
---
# <a name="windowsenrollmentstatusscreensettings-resource-type"></a>windowsEnrollmentStatusScreenSettings リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

登録の状態画面の設定

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|hideInstallationProgress 進行状況|Boolean|ユーザーにインストールの進行状況を表示または非表示にする|
|allowDeviceUseBeforeProfileAndAppInstallComplete|Boolean|プロファイルとアプリのインストールが完了する前にユーザーがデバイスを使用することを許可またはブロックする|
|blockDeviceSetupRetryByUser|Boolean|ユーザーがインストールエラー時にセットアップを再試行できるようにする|
|allowLogCollectionOnInstallFailure|Boolean|インストール失敗時にログ収集を許可またはブロックする|
|customErrorMessage|String|インストールエラーが発生したときに表示するカスタムエラーメッセージを設定する|
|installProgressTimeoutInMinutes|Int32|インストールの進行状況のタイムアウトを分単位で設定する|
|allowDeviceUseOnInstallFailure|Boolean|インストールエラー時にユーザーがデバイスを引き続き使用できるようにする|

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





