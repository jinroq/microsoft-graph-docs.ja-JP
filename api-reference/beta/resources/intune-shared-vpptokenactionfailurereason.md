---
title: vppTokenActionFailureReason 列挙型
description: Apple ボリューム購入プログラム トークンの操作エラーが発生する理由の種類です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bba4c339b774fd32a852925729e2e158dc13e52d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29393145"
---
# <a name="vpptokenactionfailurereason-enum-type"></a>vppTokenActionFailureReason 列挙型

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Apple ボリューム購入プログラム トークンの操作エラーが発生する理由の種類です。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|none|0|なし|
|appleFailure|1|Apple のサービスでエラーが発生しました。|
|internalError|2|内部エラーが発生しました。|
|expiredVppToken|3|Apple ボリューム購入プログラムのトークンの有効期限が切れていたためにエラーが発生しました。|
|expiredApplePushNotificationCertificate|4|Apple ボリューム購入プログラムをプッシュ通知証明書の有効期限が切れているためにエラーが発生しました。|




