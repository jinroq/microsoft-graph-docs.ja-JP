---
title: emailsyncduration 列挙型
description: 電子メール同期の期間として指定できる値。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8f2408150ea590a5d154b71521ca46df7c0fcff9
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30142267"
---
# <a name="emailsyncduration-enum-type"></a>emailsyncduration 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

電子メール同期の期間として指定できる値。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|自分のもの|.0|ユーザー定義、既定値、意図的ではありません。|
|oneday|1-d|1日分のメールを同期します。|
|threeDays|pbm-2|3日間のメールを同期します。|
|oneWeek|1/3|電子メールの1週間を同期します。|
|2週間|2/4|2週間のメールを同期します。|
|オンライン|5|1か月分のメールを同期します。|
|無し|シックス|電子メールの期間を無制限に同期します。|




