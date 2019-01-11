---
title: lanManagerAuthenticationLevel 列挙型
description: LanManagerAuthenticationLevel に指定できる値
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 68af209a005dc1d7e8d25672f5e97e1d929ba25b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866914"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a>lanManagerAuthenticationLevel 列挙型

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

LanManagerAuthenticationLevel に指定できる値
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|lmAndNltm|0|LM と NTLM 応答を送信します。|
|lmNtlmAndNtlmV2|1|ネゴシエートされた場合は、LM と NTLM を使用して NTLMv2 セッション セキュリティを送信します。|
|lmAndNtlmOnly|2|LM と NTLM 応答のみを送信します。|
|lmAndNtlmV2|3|LM と NTLMv2 応答のみを送信します。|
|lmNtlmV2AndNotLm|4|LM と NTLMv2 応答のみを送信します。 LM を拒否します。|
|lmNtlmV2AndNotLmOrNtm|5|LM と NTLMv2 応答のみを送信します。 LM と NTLM を拒否します。|





