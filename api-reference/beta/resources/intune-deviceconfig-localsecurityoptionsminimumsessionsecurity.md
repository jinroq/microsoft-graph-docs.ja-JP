---
title: localSecurityOptionsMinimumSessionSecurity 列挙型
description: LocalSecurityOptionsMinimumSessionSecurity に指定できる値
author: tfitzmac
ms.openlocfilehash: 5feabd9c84ec42f55bb45b952be5af834fd84498
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350632"
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





