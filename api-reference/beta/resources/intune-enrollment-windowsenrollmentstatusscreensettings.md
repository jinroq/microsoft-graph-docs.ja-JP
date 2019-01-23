---
title: windowsEnrollmentStatusScreenSettings リソースの種類
description: 登録ステータス画面の設定
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e5ffb2827988b80b4d6563d8a92c9ccea7ac9828
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399935"
---
# <a name="windowsenrollmentstatusscreensettings-resource-type"></a>windowsEnrollmentStatusScreenSettings リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

登録ステータス画面の設定

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|hideInstallationProgress|Boolean|ユーザーにインストールの進行状況の表示と非表示を切り替える|
|allowDeviceUseBeforeProfileAndAppInstallComplete|Boolean|許可またはブロックのユーザー プロファイル、およびアプリケーション インストールが完了する前にデバイスを使用するには|
|blockDeviceSetupRetryByUser|Boolean|インストールの失敗時にセットアップを再実行するユーザーを許可します。|
|allowLogCollectionOnInstallFailure|Boolean|許可またはブロックのインストールの失敗時にログの収集|
|customErrorMessage|String|インストールの失敗時に表示するカスタム エラー メッセージを設定します。|
|installProgressTimeoutInMinutes|Int32|インストールの進行状況のタイムアウトを分単位で設定します。|
|allowDeviceUseOnInstallFailure|Boolean|インストールの失敗時にデバイスを使用するユーザーを許可します。|

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




