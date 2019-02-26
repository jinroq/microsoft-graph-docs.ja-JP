---
title: windowsInformationProtectionEnforcementLevel 列挙型
description: WIP 保護適用レベルに指定できる値
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 184f5b6d296a37f9356c2cfeefe7c3ecdbdb6973
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30150149"
---
# <a name="windowsinformationprotectionenforcementlevel-enum-type"></a>windowsInformationProtectionEnforcementLevel 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

WIP 保護適用レベルに指定できる値

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|noprotection|.0|保護の適用なし|
|encryptAndAuditOnly|1-d|暗号化と監査のみ|
|encryptAuditAndPrompt|pbm-2|暗号化、監査、および確認|
|encryptAuditAndBlock|1/3|暗号化、監査、ブロック|




