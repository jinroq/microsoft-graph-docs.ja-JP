---
title: edgeTelemetryMode 列挙型
description: Microsoft 365 analytics に送信された参照データの種類
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b48840debffcc7aedf1454d9cee11b6c0ab9edc1
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172472"
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
|internet|pbm-2|インターネットの送信履歴のみを許可する: インターネットサイトの閲覧履歴データのみを送信する|
|intranetandinternet|1/3|イントラネットとインターネットの両方の履歴を送信できるようにする: イントラネットおよびインターネットサイトの閲覧履歴データを送信する|




