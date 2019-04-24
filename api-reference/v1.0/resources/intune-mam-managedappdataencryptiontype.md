---
title: managedAppDataEncryptionType 列挙型
description: 管理対象アプリについてアプリケーションデータを暗号化するレベルを表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 774312d5f19b223fd33e2c156610f516ae7f48a3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32465256"
---
# <a name="managedappdataencryptiontype-enum-type"></a>managedAppDataEncryptionType 列挙型

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

管理対象アプリについてアプリケーションデータを暗号化するレベルを表します。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|usedevicesettings|.0|アプリデータは、デバイスの既定の設定に基づいて暗号化されます。|
|afterdevicerestart|1-d|アプリのデータは、デバイスの再起動時に暗号化されます。|
|whenDeviceLockedExceptOpenFiles|pbm-2|このポリシーに関連付けられたアプリデータは、開いているファイル内のデータを除き、デバイスがロックされたときに暗号化されます。|
|whendevicelocked|1/3|デバイスがロックされている場合、このポリシーに関連付けられているアプリデータは暗号化されます。|



