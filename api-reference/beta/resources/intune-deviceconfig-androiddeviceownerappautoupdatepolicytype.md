---
title: androidDeviceOwnerAppAutoUpdatePolicyType 列挙型
description: Android デバイスの所有者に指定できる値のデバイスのアプリケーションの自動状態では、ポリシーを更新します。
localization_priority: Normal
ms.openlocfilehash: 721d08220553bf6acfaac0f84bf0d71725c39ba6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834119"
---
# <a name="androiddeviceownerappautoupdatepolicytype-enum-type"></a>androidDeviceOwnerAppAutoUpdatePolicyType 列挙型

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Android デバイスの所有者に指定できる値のデバイスのアプリケーションの自動状態では、ポリシーを更新します。
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notConfigured|0|次のように構成されません。この値は無視されます。|
|userChoice|1|ユーザーは、自動更新を制御できます。|
|ぜんぜん|2|アプリは自動で更新しません。|
|wiFiOnly|3|アプリケーションは自動的に更新 Wi-fi 経由のみです。|
|いつも|4|アプリケーションは、いつでも自動的に更新します。 データ料がかかる場合があります。|





