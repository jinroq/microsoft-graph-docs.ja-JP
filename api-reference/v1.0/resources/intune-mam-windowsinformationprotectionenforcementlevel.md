---
title: windowsInformationProtectionEnforcementLevel 列挙型
description: WIP 保護適用レベルに指定できる値
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b1901059ef45141b0dc40d91dcbf4d9237cd6fc5
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254815"
---
# <a name="windowsinformationprotectionenforcementlevel-enum-type"></a>windowsInformationProtectionEnforcementLevel 列挙型

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

WIP 保護適用レベルに指定できる値

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|noprotection|.0|保護の適用なし|
|encryptAndAuditOnly|1-d|暗号化と監査のみ|
|encryptAuditAndPrompt|pbm-2|暗号化、監査、および確認|
|encryptAuditAndBlock|1/3|暗号化、監査、ブロック|



