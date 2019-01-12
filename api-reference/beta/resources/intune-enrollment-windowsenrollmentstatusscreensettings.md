---
title: windowsEnrollmentStatusScreenSettings リソースの種類
description: 登録ステータス画面の設定
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: abc48a1d63cc514d2ec887a7758e69a0ea8112a7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978572"
---
# <a name="windowsenrollmentstatusscreensettings-resource-type"></a>windowsEnrollmentStatusScreenSettings リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

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





