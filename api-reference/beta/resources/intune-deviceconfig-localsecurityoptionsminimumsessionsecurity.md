---
title: localSecurityOptionsMinimumSessionSecurity 列挙型
description: LocalSecurityOptionsMinimumSessionSecurity に指定できる値
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8dc6a96f5dda3cdba9ea3a57507bef4f32edc5a8
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36325527"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a>localSecurityOptionsMinimumSessionSecurity 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

LocalSecurityOptionsMinimumSessionSecurity に指定できる値

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|none|.0|LM & NTLM 応答を送信する|
|requireNtmlV2SessionSecurity|1-d|LM & NTLM を送信する-ネゴシエートされる場合は NTLMv2 セッションセキュリティを使用する|
|require128BitEncryption|pbm-2|LM & NTLM 応答のみを送信する|
|ntlmV2And128BitEncryption|1/3|LM & NTLMv2 応答のみを送信する|



