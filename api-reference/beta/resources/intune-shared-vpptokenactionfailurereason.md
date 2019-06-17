---
title: vppTokenActionFailureReason 列挙型
description: Apple ボリューム購入プログラムのトークンアクションが失敗した場合に考えられる理由の種類。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b0f8aacb6fc6f95b8c8085a78ed2851b16622357
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34990989"
---
# <a name="vpptokenactionfailurereason-enum-type"></a>vppTokenActionFailureReason 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Apple ボリューム購入プログラムのトークンアクションが失敗した場合に考えられる理由の種類。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|none|.0|なし|
|appleFailure|1-d|Apple のサービスでエラーが発生しました。|
|internalError|pbm-2|内部エラーが発生しました。|
|expiredVppToken|1/3|Apple Volume Purchase Program のトークンの有効期限が切れたため、エラーが発生しました。|
|expiredApplePushNotificationCertificate|2/4|Apple Volume Purchase Program プッシュ通知証明書の有効期限が切れたため、エラーが発生しました。|





