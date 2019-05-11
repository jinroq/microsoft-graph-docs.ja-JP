---
title: managedAppDataEncryptionType 列挙型
description: 管理対象アプリについてアプリケーションデータを暗号化するレベルを表します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fde2db55cb9af109e2de82f87ef96044f8da36aa
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940786"
---
# <a name="managedappdataencryptiontype-enum-type"></a>managedAppDataEncryptionType 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

管理対象アプリについてアプリケーションデータを暗号化するレベルを表します。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|useDeviceSettings|.0|アプリデータは、デバイスの既定の設定に基づいて暗号化されます。|
|afterDeviceRestart|1-d|アプリのデータは、デバイスの再起動時に暗号化されます。|
|whenDeviceLockedExceptOpenFiles|pbm-2|このポリシーに関連付けられたアプリデータは、開いているファイル内のデータを除き、デバイスがロックされたときに暗号化されます。|
|whenDeviceLocked|1/3|デバイスがロックされている場合、このポリシーに関連付けられているアプリデータは暗号化されます。|




