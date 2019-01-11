---
title: managedAppDataEncryptionType 列挙型
description: マネージ アプリケーションのアプリケーション データを暗号化するレベルを表します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f57904d45b24f6aaae9d67394facb07692add67e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834147"
---
# <a name="managedappdataencryptiontype-enum-type"></a>managedAppDataEncryptionType 列挙型

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

マネージ アプリケーションのアプリケーション データを暗号化するレベルを表します。
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|useDeviceSettings|0|デバイスの既定の設定に基づいて、アプリケーション データが暗号化されます。|
|afterDeviceRestart|1|デバイスが再起動されると、アプリケーション データが暗号化されます。|
|whenDeviceLockedExceptOpenFiles|2|開かれているファイル内のデータを除いて、デバイスがロックされている場合、このポリシーに関連付けられているアプリケーションのデータは暗号化されて|
|whenDeviceLocked|3|デバイスがロックされている場合、このポリシーに関連付けられているアプリケーション データが暗号化されて|



