---
title: emailsyncschedule 列挙型
description: 電子メール同期スケジュールに指定できる値。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1da569d7050e88dd5eb41640bc2d8eaa602bb2b7
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31781282"
---
# <a name="emailsyncschedule-enum-type"></a>emailsyncschedule 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

電子メール同期スケジュールに指定できる値。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|自分のもの|.0|ユーザー定義、既定値、意図的ではありません。|
|asメッセージの受信|1-d|メッセージが到着したときに同期します。|
|手動|pbm-2|手動で同期します。|
|fifteenMinutes|1/3|15分ごとに同期します。|
|thirtyMinutes|2/4|30分ごとに同期します。|
|sixtyMinutes|5|60分ごとに同期します。|
|basedOnMyUsage|シックス|自分の使用状況に基づいて同期します。|





