---
title: lanManagerAuthenticationLevel 列挙型
description: LanManagerAuthenticationLevel に指定できる値
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9a80aefec83c0c2a577af9b8dfed5dcea1ff7d79
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34989351"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a>lanManagerAuthenticationLevel 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

LanManagerAuthenticationLevel に指定できる値

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|lmAndNltm|.0|LM & NTLM 応答を送信する|
|lmNtlmAndNtlmV2|1-d|LM & NTLM を送信する-ネゴシエートされる場合は NTLMv2 セッションセキュリティを使用する|
|lmAndNtlmOnly|pbm-2|LM & NTLM 応答のみを送信する|
|lmAndNtlmV2|1/3|LM & NTLMv2 応答のみを送信する|
|lmNtlmV2AndNotLm|2/4|LM & NTLMv2 応答のみを送信します。 LM を拒否する|
|lmNtlmV2AndNotLmOrNtm|5|LM & NTLMv2 応答のみを送信します。 NTLM & の LM を拒否する|





