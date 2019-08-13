---
title: deviceEnrollmentFailureReason 列挙型
description: 登録の最上位レベルのエラーカテゴリ。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 912c32c737ba289168493cbfddd064e76ca91053
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36347786"
---
# <a name="deviceenrollmentfailurereason-enum-type"></a>deviceEnrollmentFailureReason 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

登録の最上位レベルのエラーカテゴリ。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|不明|.0|既定値、エラーの理由は不明です。|
|認証|1-d|認証に失敗した|
|手続き|pbm-2|呼び出しは認証されましたが、登録が承認されていません。|
|accountValidation|1/3|登録のためにアカウントを検証できませんでした。 (アカウントがブロックされ、登録が有効になっていません)|
|userValidation|2/4|ユーザーを検証できませんでした。 (ユーザーが存在しません。ライセンスがありません)|
|deviceNotSupported|5|デバイスは、モバイルデバイス管理ではサポートされていません。|
|inMaintenance|シックス|アカウントはメンテナンス中です。|
|badRequest|7|クライアントがサービスで認識/サポートされていない要求を送信しました。|
|featureNotSupported|8 |この登録で使用されている機能は、このアカウントではサポートされていません。|
|enrollmentRestrictionsEnforced|9 |管理者によって構成された登録の制限は、この登録をブロックしました。|
|clientDisconnected|10 |クライアントがタイムアウトしたか、登録が enduser によって中止されました。|
|userAbandonment|#|登録は enduser によって中止されました。 (Enduser が開始されましたが、適切なタイミングで完了できませんでした)|



