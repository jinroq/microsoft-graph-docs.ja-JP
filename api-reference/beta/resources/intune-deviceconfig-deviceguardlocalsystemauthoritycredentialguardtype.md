---
title: deviceGuardLocalSystemAuthorityCredentialGuardType 列挙型
description: Credential Guard 設定の可能な値。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0f22336a37c3d10d4e86b3db2af41e8103dcfe33
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32567229"
---
# <a name="deviceguardlocalsystemauthoritycredentialguardtype-enum-type"></a>deviceGuardLocalSystemAuthorityCredentialGuardType 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Credential Guard 設定の可能な値。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notConfigured|.0|以前に UEFI ロックを設定していない場合に、Credential Guard をリモートで無効にします。|
|enableWithUEFILock|1 |UEFI ロックを使用して Credential Guard を有効にします。|
|enableWithoutUEFILock|2 |UEFI ロックなしで Credential Guard を有効にします。|





