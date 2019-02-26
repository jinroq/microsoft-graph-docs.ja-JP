---
title: lanmanagerauthenticationlevel 列挙型
description: lanmanagerauthenticationlevel に指定できる値
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 63f04f1ef2fc12fa0352aeec803c46fb4ebab3d2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166571"
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




