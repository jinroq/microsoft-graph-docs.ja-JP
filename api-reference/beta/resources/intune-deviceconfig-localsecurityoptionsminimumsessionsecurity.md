---
title: localSecurityOptionsMinimumSessionSecurity 列挙型
description: LocalSecurityOptionsMinimumSessionSecurity に指定できる値
ms.openlocfilehash: 969c7d6576c613f5214bfc3b8a5a1ad36722f0df
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072332"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a>localSecurityOptionsMinimumSessionSecurity 列挙型

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

LocalSecurityOptionsMinimumSessionSecurity に指定できる値
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|none|0|LM と NTLM 応答を送信します。|
|requireNtmlV2SessionSecurity|1|ネゴシエートされた場合は、LM と NTLM を使用して NTLMv2 セッション セキュリティを送信します。|
|require128BitEncryption|2|LM と NTLM 応答のみを送信します。|
|ntlmV2And128BitEncryption|3|LM と NTLMv2 応答のみを送信します。|





