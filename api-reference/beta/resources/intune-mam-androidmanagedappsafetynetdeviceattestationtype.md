---
title: androidManagedAppSafetyNetDeviceAttestationType 列挙型
description: 管理者が管理対象アプリに Android の saf etynet デバイスの構成証明の要件を適用している。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cef86d779a866174749a0916ab606f64374bfa1d
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31775472"
---
# <a name="androidmanagedappsafetynetdeviceattestationtype-enum-type"></a>androidManagedAppSafetyNetDeviceAttestationType 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

管理者が管理対象アプリに Android の saf etynet デバイスの構成証明の要件を適用している。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|none|.0|要件セットなし|
|basicintegrity|1-d|Android デバイスが安全であることを必要とするのは、安全な整合性検証|
|basicIntegrityAndDeviceCertification|pbm-2|Android デバイスが安全であることを必要とする、の基本的な整合性とデバイス証明の検証|





