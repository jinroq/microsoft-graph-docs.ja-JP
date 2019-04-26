---
title: deviceEnrollmentFailureReason 列挙型
description: 登録の最上位レベルのエラーカテゴリ。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 623030bccfac9e023a0d1df2dff7ea317b503485
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32571836"
---
# <a name="deviceenrollmentfailurereason-enum-type"></a>deviceEnrollmentFailureReason 列挙型

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

登録の最上位レベルのエラーカテゴリ。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|不明|.0|既定値、エラーの理由は不明です。|
|認証|1 |認証に失敗した|
|手続き|2 |呼び出しは認証されましたが、登録が承認されていません。|
|accountvalidation|3 |登録のためにアカウントを検証できませんでした。 (アカウントがブロックされ、登録が有効になっていません)|
|uservalidation|4 |ユーザーを検証できませんでした。 (ユーザーが存在しません。ライセンスがありません)|
|devicenotsupported|5 |デバイスは、モバイルデバイス管理ではサポートされていません。|
|inmaintenance|6 |アカウントはメンテナンス中です。|
|badrequest|7 |クライアントがサービスで認識/サポートされていない要求を送信しました。|
|featureNotSupported|8 |この登録で使用されている機能は、このアカウントではサポートされていません。|
|enrollmentRestrictionsEnforced|9 |管理者によって構成された登録の制限は、この登録をブロックしました。|
|clientdisconnected|10  |クライアントがタイムアウトしたか、登録が enduser によって中止されました。|
|userAbandonment|11 |登録は enduser によって中止されました。 (Enduser が開始されましたが、適切なタイミングで完了できませんでした)|


<!-- {
  "type": "#page.annotation",
  "suppressions": [
     "Warning: Enum deviceEnrollmentFailureReason has some values specified and others unspecified."
  ],
}
-->

