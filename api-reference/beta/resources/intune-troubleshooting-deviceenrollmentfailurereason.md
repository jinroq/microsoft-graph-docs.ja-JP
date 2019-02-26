---
title: deviceEnrollmentFailureReason 列挙型
description: 登録の最上位レベルのエラーカテゴリ。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f03ce73f1d6f8b5edc6b3e3b661f9a7ba79407bb
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163855"
---
# <a name="deviceenrollmentfailurereason-enum-type"></a>deviceEnrollmentFailureReason 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

登録の最上位レベルのエラーカテゴリ。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|不明|.0|既定値、エラーの理由は不明です。|
|認証|1-d|認証に失敗した|
|承認|pbm-2|呼び出しは認証されましたが、登録が承認されていません。|
|accountvalidation|1/3|登録のためにアカウントを検証できませんでした。 (アカウントがブロックされ、登録が有効になっていません)|
|uservalidation|2/4|ユーザーを検証できませんでした。 (ユーザーが存在しません。ライセンスがありません)|
|devicenotsupported|5|デバイスは、モバイルデバイス管理ではサポートされていません。|
|inmaintenance|シックス|アカウントはメンテナンス中です。|
|badrequest|7|クライアントがサービスで認識/サポートされていない要求を送信しました。|
|featureNotSupported|~|この登録で使用されている機能は、このアカウントではサポートされていません。|
|enrollmentRestrictionsEnforced|i-9|管理者によって構成された登録の制限は、この登録をブロックしました。|
|clientdisconnected|個|クライアントがタイムアウトしたか、登録が enduser によって中止されました。|
|userAbandonment|#|登録は enduser によって中止されました。 (Enduser が開始されましたが、適切なタイミングで完了できませんでした)|




