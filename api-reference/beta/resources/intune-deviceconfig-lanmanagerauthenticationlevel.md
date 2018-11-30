---
title: lanManagerAuthenticationLevel 列挙型
description: LanManagerAuthenticationLevel に指定できる値
ms.openlocfilehash: 9fb8113c4953a0cabcecfbc5303b9f62f685d5ca
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066945"
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





