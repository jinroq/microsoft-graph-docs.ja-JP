---
title: emailSyncDuration 列挙型
description: 電子メール同期の期間として指定できる値。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: fc05be47c2adc0764a2cdb1e69f7ec11413320cc
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36357195"
---
# <a name="emailsyncduration-enum-type"></a>emailSyncDuration 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

電子メール同期の期間として指定できる値。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|自分のもの|.0|ユーザー定義、既定値、意図的ではありません。|
|oneDay|1-d|1日分のメールを同期します。|
|threeDays|pbm-2|3日間のメールを同期します。|
|oneWeek|1/3|電子メールの1週間を同期します。|
|2週間|2/4|2週間のメールを同期します。|
|オンライン|5|1か月分のメールを同期します。|
|無制限|シックス|電子メールの期間を無制限に同期します。|



