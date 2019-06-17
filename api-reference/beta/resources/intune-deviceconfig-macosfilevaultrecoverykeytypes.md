---
title: macOSFileVaultRecoveryKeyTypes 列挙型
description: MacOS FileVault の回復キーの種類
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 193bfc5769da2919f93df9beef38524a57bfece0
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "35002547"
---
# <a name="macosfilevaultrecoverykeytypes-enum-type"></a>macOSFileVaultRecoveryKeyTypes 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

MacOS FileVault の回復キーの種類

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notConfigured|.0|デバイスの既定値。意図的ではありません。|
|institutionalRecoveryKey|1-d|"マスター" 回復キーは、パスワードが失われたデバイスのロックを解除するために使用できる "マスター" 回復キーに似ています。|
|パーソナル Recoverykey|pbm-2|個人回復キーは、デバイスに対するパスワードが失われた場合でも、ユーザーのデバイスのロックを解除するために使用できる一意のコードです。|





