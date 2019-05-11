---
title: deviceRegistrationState 列挙型
description: デバイス登録の状態。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 94ff2a645b9ea3862cee50ca086284deea02da09
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33942018"
---
# <a name="deviceregistrationstate-enum-type"></a>deviceRegistrationState 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

デバイス登録の状態。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notRegistered 済み|.0|デバイスが登録されていません。|
|い|pbm-2|デバイスは登録されています。|
|破棄|1/3|デバイスがブロックされているか、ワイプされているか、破棄されています。|
|keyConflict|2/4|デバイスにキーの競合があります。|
|approvalPending|5|デバイスの承認が保留中です。|
|certificateReset|シックス|デバイス証明書がリセットされました。|
|notRegisteredPendingEnrollment|7|デバイスは登録されておらず、登録が保留されていません。|
|不明|8 |デバイス登録の状態が不明です。|




