---
title: windowsSModeConfiguration 列挙型
description: S モードのロック解除を構成するために使用可能なオプション
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 841c95fa1b02f0923c9659ab9c1858b4c2b9560c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32554185"
---
# <a name="windowssmodeconfiguration-enum-type"></a>windowsSModeConfiguration 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

S モードのロック解除を構成するために使用可能なオプション

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|noRestriction|.0|このオプションを選択すると、ロックを解除するためのすべての制限が削除されます-既定値|
|拒否|1 |このオプションは、ユーザーが S モードからデバイスのロックを解除するのをブロックします。|
|外す|2 |このオプションでは、デバイスを S モードからロック解除します。|





