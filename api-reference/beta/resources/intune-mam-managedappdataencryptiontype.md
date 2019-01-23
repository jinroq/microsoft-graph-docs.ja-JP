---
title: managedAppDataEncryptionType 列挙型
description: マネージ アプリケーションのアプリケーション データを暗号化するレベルを表します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 00174e7fba8a8da7490d04815b07a794a966179c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413690"
---
# <a name="managedappdataencryptiontype-enum-type"></a>managedAppDataEncryptionType 列挙型

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

マネージ アプリケーションのアプリケーション データを暗号化するレベルを表します。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|useDeviceSettings|0|デバイスの既定の設定に基づいて、アプリケーション データが暗号化されます。|
|afterDeviceRestart|1|デバイスが再起動されると、アプリケーション データが暗号化されます。|
|whenDeviceLockedExceptOpenFiles|2|開かれているファイル内のデータを除いて、デバイスがロックされている場合、このポリシーに関連付けられているアプリケーションのデータは暗号化されて|
|whenDeviceLocked|3|デバイスがロックされている場合、このポリシーに関連付けられているアプリケーション データが暗号化されて|




