---
title: androidDeviceOwnerAppAutoUpdatePolicyType 列挙型
description: Android デバイスの所有者に指定できる値のデバイスのアプリケーションの自動状態では、ポリシーを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 68dec6bb21cf27a7b5b54f9fc8a839fba3dc6f00
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419073"
---
# <a name="androiddeviceownerappautoupdatepolicytype-enum-type"></a>androidDeviceOwnerAppAutoUpdatePolicyType 列挙型

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Android デバイスの所有者に指定できる値のデバイスのアプリケーションの自動状態では、ポリシーを更新します。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notConfigured|0|次のように構成されません。この値は無視されます。|
|userChoice|1|ユーザーは、自動更新を制御できます。|
|ぜんぜん|2|アプリは自動で更新しません。|
|wiFiOnly|3|アプリケーションは自動的に更新 Wi-fi 経由のみです。|
|いつも|4|アプリケーションは、いつでも自動的に更新します。 データ料がかかる場合があります。|




