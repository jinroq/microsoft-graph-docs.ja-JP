---
title: windowsUpdateNotificationDisplayOption 列挙型
description: Windows Update 通知の表示オプション
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7e792e3a866a0fadae5f866654e50ffe16cdc4c0
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31788269"
---
# <a name="windowsupdatenotificationdisplayoption-enum-type"></a>windowsUpdateNotificationDisplayOption 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Windows Update 通知の表示オプション

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notConfigured|.0|未構成|
|defaultnotifications|1-d|既定の Windows Update 通知を使用します。|
|restartWarningsOnly|pbm-2|再起動警告を除く、すべての通知をオフにします。|
|disableallnotifications|1/3|再起動の警告を含む、すべての通知をオフにします。|





