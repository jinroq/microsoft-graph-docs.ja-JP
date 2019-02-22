---
title: windowsSModeConfiguration 列挙型
description: S モードのロック解除を構成するために使用可能なオプション
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6a451108c6e55f8587317dfc43caf8bc84cca673
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144717"
---
# <a name="windowssmodeconfiguration-enum-type"></a>windowsSModeConfiguration 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

S モードのロック解除を構成するために使用可能なオプション

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|noRestriction|.0|このオプションを選択すると、ロックを解除するためのすべての制限が削除されます-既定値|
|拒否|1-d|このオプションは、ユーザーが S モードからデバイスのロックを解除するのをブロックします。|
|外す|pbm-2|このオプションでは、デバイスを S モードからロック解除します。|




