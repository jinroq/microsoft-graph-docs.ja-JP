---
title: managedAppDataEncryptionType 列挙型
description: 管理対象アプリについてアプリケーションデータを暗号化するレベルを表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 47396f32ed23234c5fe758a29b6e97ee3602234f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159081"
---
# <a name="managedappdataencryptiontype-enum-type"></a>managedAppDataEncryptionType 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

管理対象アプリについてアプリケーションデータを暗号化するレベルを表します。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|usedevicesettings|.0|アプリデータは、デバイスの既定の設定に基づいて暗号化されます。|
|afterdevicerestart|1-d|アプリのデータは、デバイスの再起動時に暗号化されます。|
|whenDeviceLockedExceptOpenFiles|pbm-2|このポリシーに関連付けられたアプリデータは、開いているファイル内のデータを除き、デバイスがロックされたときに暗号化されます。|
|whendevicelocked|1/3|デバイスがロックされている場合、このポリシーに関連付けられているアプリデータは暗号化されます。|




