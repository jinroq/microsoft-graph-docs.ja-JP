---
title: edgeTelemetryMode 列挙型
description: Microsoft 365 分析機能に送信されるデータの参照の種類
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 81d429f7629a5d6a6f2593785605902065d9f1c7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430416"
---
# <a name="edgetelemetrymode-enum-type"></a>edgeTelemetryMode 列挙型

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Microsoft 365 分析機能に送信されるデータの参照の種類

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notConfigured|0|既定: 遠隔測定データを収集または送信|
|イントラネット|1|イントラネットの履歴のみを送信することを許可する: イントラネットのサイトの履歴データを参照するだけの送信|
|internet|2|インターネットの履歴のみを送信することを許可する: インターネット サイトの履歴データを参照するだけの送信|
|intranetAndInternet|3|イントラネットとインターネットの両方の履歴を送信することを許可する: イントラネットとインターネットのサイトの履歴データを参照する送信|




