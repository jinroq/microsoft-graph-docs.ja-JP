---
title: emailSyncDuration 列挙型
description: 電子メールに使用できる値は、時間を同期します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8bf62aea1904c0fd25867aef308ca5a269e3ea20
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399410"
---
# <a name="emailsyncduration-enum-type"></a>emailSyncDuration 列挙型

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

電子メールに使用できる値は、時間を同期します。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|ユーザー定義|0|ユーザー定義、既定値、ない目的。|
|直後|1|1 日分の電子メールを同期します。|
|3 日|2|3 日間の電子メールを同期します。|
|1 週間|3|1 週間分のメールを同期します。|
|2 週間|4|2 週間分のメールを同期します。|
|oneMonth|5|電子メールの 1 か月を同期します。|
|無制限|6|電子メールの無制限の時間を同期します。|




