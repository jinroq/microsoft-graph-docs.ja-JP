---
title: edgeTelemetryMode 列挙型
description: Microsoft 365 analytics に送信された参照データの種類
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 105c0fe71aa851d8f8002920cdc9a91993f39c9f
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34996415"
---
# <a name="edgetelemetrymode-enum-type"></a>edgeTelemetryMode 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Microsoft 365 analytics に送信された参照データの種類

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notConfigured|.0|既定–収集または送信されたテレメトリデータはありません。|
|イントラネット|1-d|イントラネットの履歴のみを送信できるようにする: イントラネットサイトの閲覧履歴データのみを送信する|
|経由|pbm-2|インターネットの送信履歴のみを許可する: インターネットサイトの閲覧履歴データのみを送信する|
|intranetAndInternet|1/3|イントラネットとインターネットの両方の履歴を送信できるようにする: イントラネットおよびインターネットサイトの閲覧履歴データを送信する|





