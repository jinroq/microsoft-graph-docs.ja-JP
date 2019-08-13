---
title: windowsUpdateNotificationDisplayOption 列挙型
description: Windows Update 通知の表示オプション
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 69c990e8cb2eefc71e1a0cae085e71da7e095383
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36337672"
---
# <a name="windowsupdatenotificationdisplayoption-enum-type"></a>windowsUpdateNotificationDisplayOption 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Windows Update 通知の表示オプション

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notConfigured|.0|未構成|
|defaultNotifications|1-d|既定の Windows Update 通知を使用します。|
|restartWarningsOnly|pbm-2|再起動警告を除く、すべての通知をオフにします。|
|disableAllNotifications|1/3|再起動の警告を含む、すべての通知をオフにします。|



