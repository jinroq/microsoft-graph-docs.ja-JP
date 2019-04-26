---
title: emailsyncduration 列挙型
description: 電子メール同期の期間として指定できる値。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0f66f3abc888205c66745906da0a8803c18b4522
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32556215"
---
# <a name="emailsyncduration-enum-type"></a>emailsyncduration 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

電子メール同期の期間として指定できる値。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|自分のもの|.0|ユーザー定義、既定値、意図的ではありません。|
|oneday|1 |1日分のメールを同期します。|
|threeDays|2 |3日間のメールを同期します。|
|oneWeek|3 |電子メールの1週間を同期します。|
|2週間|4 |2週間のメールを同期します。|
|オンライン|5 |1か月分のメールを同期します。|
|無制限|6 |電子メールの期間を無制限に同期します。|





