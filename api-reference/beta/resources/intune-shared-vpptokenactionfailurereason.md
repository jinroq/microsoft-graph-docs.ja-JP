---
title: vppTokenActionFailureReason 列挙型
description: Apple ボリューム購入プログラムのトークンアクションが失敗した場合に考えられる理由の種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 05d3137bb5aac2aef3024825df5e7e0b84ffde51
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169693"
---
# <a name="vpptokenactionfailurereason-enum-type"></a>vppTokenActionFailureReason 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Apple ボリューム購入プログラムのトークンアクションが失敗した場合に考えられる理由の種類。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|none|.0|なし|
|appleFailure|1-d|Apple のサービスでエラーが発生しました。|
|internalError|pbm-2|内部エラーが発生しました。|
|expiredVppToken|1/3|Apple volume purchase program のトークンの有効期限が切れたため、エラーが発生しました。|
|expiredApplePushNotificationCertificate|2/4|Apple volume purchase program プッシュ通知証明書の有効期限が切れたため、エラーが発生しました。|




