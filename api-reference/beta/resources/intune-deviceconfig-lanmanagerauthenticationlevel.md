---
title: lanmanagerauthenticationlevel 列挙型
description: lanmanagerauthenticationlevel に指定できる値
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e3b93f229661de3e2fbb28f764288983b2fd83bb
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31801247"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a>lanmanagerauthenticationlevel 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

lanmanagerauthenticationlevel に指定できる値

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|lmandnltm|.0|LM & NTLM 応答の送信|
|lmNtlmAndNtlmV2|1-d|LM & NTLM を送信する-ネゴシエートされる場合は NTLMv2 セッションセキュリティを使用する|
|lmAndNtlmOnly|pbm-2|LM & NTLM 応答のみを送信する|
|lmAndNtlmV2|1/3|LM & NTLMv2 応答のみを送信する|
|lmNtlmV2AndNotLm|2/4|LM & NTLMv2 応答のみを送信します。 lm を拒否する|
|lmNtlmV2AndNotLmOrNtm|5|LM & NTLMv2 応答のみを送信します。 lm & NTLM を拒否する|





