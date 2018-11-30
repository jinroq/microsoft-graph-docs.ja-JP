---
title: deviceEnrollmentFailureReason 列挙型
description: 登録の最上位レベルの障害のカテゴリ。
ms.openlocfilehash: c0062a829811d9fb25453adb260d4d2be0295dd7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072801"
---
# <a name="deviceenrollmentfailurereason-enum-type"></a>deviceEnrollmentFailureReason 列挙型

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

登録の最上位レベルの障害のカテゴリ。
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|不明|0|既定値、失敗の理由は不明です。|
|認証|1|認証に失敗しました|
|承認|2|呼び出しが認証されると、ですが、登録する権限がありませんでした。|
|accountValidation|3|登録用のアカウントを検証できませんでした。 (アカウントがブロックされている登録が有効になっていません)|
|userValidation|4|ユーザーを検証できませんでした。 (ユーザーが存在しない場合は、不足しているライセンス)|
|deviceNotSupported|5|モバイル デバイスの管理には、デバイスはサポートされていません。|
|inMaintenance|6|アカウントがメンテナンスします。|
|badRequest|7|サービスで認識されるサポートではない要求をクライアントに送信されます。|
|featureNotSupported|8|このアカウントには、この登録で使用される機能はサポートされていません。|
|enrollmentRestrictionsEnforced|9|管理者によって構成されている登録の制限には、この登録がブロックされています。|
|clientDisconnected|10|クライアントがタイムアウトするか、登録は、エンド ・ ユーザーによって中止されました。|
|userAbandonment|11|登録は、エンド ・ ユーザーによって中断されました。 (エンド ・ ユーザーは、契約時の開始が、時間内に完了できませんでした)|





