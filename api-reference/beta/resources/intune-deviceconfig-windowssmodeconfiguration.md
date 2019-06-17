---
title: windowsSModeConfiguration 列挙型
description: S モードのロック解除を構成するために使用可能なオプション
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: db32cab4fa405d9783415710bb5412e08c56239b
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34996457"
---
# <a name="windowssmodeconfiguration-enum-type"></a>windowsSModeConfiguration 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

S モードのロック解除を構成するために使用可能なオプション

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|noRestriction|.0|このオプションを選択すると、ロックを解除するためのすべての制限が削除されます-既定値|
|拒否|1-d|このオプションは、ユーザーが S モードからデバイスのロックを解除するのをブロックします。|
|外す|pbm-2|このオプションでは、デバイスを S モードからロック解除します。|





