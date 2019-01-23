---
title: localSecurityOptionsMinimumSessionSecurity 列挙型
description: LocalSecurityOptionsMinimumSessionSecurity に指定できる値
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c39f2bb6d0bab2aff09fc05bb0492e81102e1b7c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396085"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a>localSecurityOptionsMinimumSessionSecurity 列挙型

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

LocalSecurityOptionsMinimumSessionSecurity に指定できる値

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|none|0|NTLM 応答を送信するには、LM &|
|requireNtmlV2SessionSecurity|1|LM NTLM の使用を & の NTLMv2 セッション セキュリティをネゴシエートされた場合に送信します。|
|require128BitEncryption|2|NTLM 応答のみを送信するには、LM &|
|ntlmV2And128BitEncryption|3|NTLMv2 応答のみを送信するには、LM &|




