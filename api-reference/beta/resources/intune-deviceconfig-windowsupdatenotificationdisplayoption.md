---
title: windowsUpdateNotificationDisplayOption 列挙型
description: Windows Update 通知の表示オプション
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4dadeaa0b02083cea589c798304b4f02bf6af17b
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/14/2019
ms.locfileid: "30631598"
---
# <a name="windowsupdatenotificationdisplayoption-enum-type"></a>windowsUpdateNotificationDisplayOption 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Windows Update 通知の表示オプション

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notConfigured|.0|未構成|
|defaultnotifications|1|既定の Windows Update 通知を使用します。|
|restartWarningsOnly|2|再起動警告を除く、すべての通知をオフにします。|
|disableallnotifications|1/3|再起動の警告を含む、すべての通知をオフにします。|




