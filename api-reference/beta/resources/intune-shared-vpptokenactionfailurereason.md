---
title: vppTokenActionFailureReason 列挙型
description: Apple ボリューム購入プログラム トークンの操作エラーが発生する理由の種類です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: baf33c29a822cc725c66ff6a3a7d796e57e63693
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961163"
---
# <a name="vpptokenactionfailurereason-enum-type"></a>vppTokenActionFailureReason 列挙型

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Apple ボリューム購入プログラム トークンの操作エラーが発生する理由の種類です。
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|none|0|なし|
|appleFailure|1|Apple のサービスでエラーが発生しました。|
|internalError|2|内部エラーが発生しました。|
|expiredVppToken|3|Apple ボリューム購入プログラムのトークンの有効期限が切れていたためにエラーが発生しました。|
|expiredApplePushNotificationCertificate|4|Apple ボリューム購入プログラムをプッシュ通知証明書の有効期限が切れているためにエラーが発生しました。|





