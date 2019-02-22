---
title: androidDeviceOwnerAppAutoUpdatePolicyType 列挙型
description: Android デバイス所有者デバイスのアプリ自動更新ポリシーの状態の値を指定できます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6242bc9470661d75b3174198761cfcab8284381d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159256"
---
# <a name="androiddeviceownerappautoupdatepolicytype-enum-type"></a>androidDeviceOwnerAppAutoUpdatePolicyType 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Android デバイス所有者デバイスのアプリ自動更新ポリシーの状態の値を指定できます。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notConfigured|.0|未構成。この値は無視されます。|
|userchoice|1-d|ユーザーは自動更新を制御できます。|
|ぜんぜん|pbm-2|アプリが自動更新されることはありません。|
|wiFiOnly|1/3|アプリは wi-fi 経由で自動更新されます。|
|いつも|2/4|アプリはいつでも自動更新されます。 データ料金が適用される場合があります。|




