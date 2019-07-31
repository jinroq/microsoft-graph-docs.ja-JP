---
title: androidDeviceOwnerAppAutoUpdatePolicyType 列挙型
description: Android デバイス所有者デバイスのアプリ自動更新ポリシーの状態の値を指定できます。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: bdc8c5f9064ab68017d9857f384fb17388d0cce7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971551"
---
# <a name="androiddeviceownerappautoupdatepolicytype-enum-type"></a>androidDeviceOwnerAppAutoUpdatePolicyType 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Android デバイス所有者デバイスのアプリ自動更新ポリシーの状態の値を指定できます。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notConfigured|.0|未構成。この値は無視されます。|
|userChoice|1-d|ユーザーは自動更新を制御できます。|
|ぜんぜん|pbm-2|アプリが自動更新されることはありません。|
|wiFiOnly|1/3|アプリは Wi-fi 経由で自動更新されます。|
|いつも|2/4|アプリはいつでも自動更新されます。 データ料金が適用される場合があります。|





