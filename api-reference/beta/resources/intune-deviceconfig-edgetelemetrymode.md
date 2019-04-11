---
title: edgeTelemetryMode 列挙型
description: Microsoft 365 analytics に送信された参照データの種類
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1d671849e34d27403450ae6324b824a92ae9d9b4
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31774590"
---
# <a name="edgetelemetrymode-enum-type"></a>edgeTelemetryMode 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Microsoft 365 analytics に送信された参照データの種類

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notConfigured|.0|既定–収集または送信されたテレメトリデータはありません。|
|イントラネット|1-d|イントラネットの履歴のみを送信できるようにする: イントラネットサイトの閲覧履歴データのみを送信する|
|経由|pbm-2|インターネットの送信履歴のみを許可する: インターネットサイトの閲覧履歴データのみを送信する|
|intranetandinternet|1/3|イントラネットとインターネットの両方の履歴を送信できるようにする: イントラネットおよびインターネットサイトの閲覧履歴データを送信する|





