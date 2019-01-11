---
title: windowsEnrollmentStatusScreenSettings リソースの種類
description: 登録ステータス画面の設定
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7263fdd8ab3d9a39d5081322c62cfcf76a4c7aa0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27877449"
---
# <a name="windowsenrollmentstatusscreensettings-resource-type"></a>windowsEnrollmentStatusScreenSettings リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

登録ステータス画面の設定
## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|hideInstallationProgress|ブール型|ユーザーにインストールの進行状況の表示と非表示を切り替える|
|allowDeviceUseBeforeProfileAndAppInstallComplete|ブール型|許可またはブロックのユーザー プロファイル、およびアプリケーション インストールが完了する前にデバイスを使用するには|
|blockDeviceSetupRetryByUser|ブール型|インストールの失敗時にセットアップを再実行するユーザーを許可します。|
|allowLogCollectionOnInstallFailure|ブール型|許可またはブロックのインストールの失敗時にログの収集|
|customErrorMessage|String|インストールの失敗時に表示するカスタム エラー メッセージを設定します。|
|installProgressTimeoutInMinutes|Int32|インストールの進行状況のタイムアウトを分単位で設定します。|
|allowDeviceUseOnInstallFailure|ブール型|インストールの失敗時にデバイスを使用するユーザーを許可します。|

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





