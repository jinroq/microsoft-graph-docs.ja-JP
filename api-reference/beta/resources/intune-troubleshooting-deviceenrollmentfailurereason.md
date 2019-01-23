---
title: deviceEnrollmentFailureReason 列挙型
description: 登録の最上位レベルの障害のカテゴリ。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: fbfe7193c72f1ff1a03a7e7bb4da57d0a032e530
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396211"
---
# <a name="deviceenrollmentfailurereason-enum-type"></a>deviceEnrollmentFailureReason 列挙型

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

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




