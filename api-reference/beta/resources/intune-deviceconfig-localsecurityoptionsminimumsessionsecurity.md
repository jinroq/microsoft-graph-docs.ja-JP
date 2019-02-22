---
title: localsecurityoptionsminimumsessionsecurity 列挙型
description: localsecurityoptionsminimumsessionsecurity に指定できる値
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fe6007747aed1037a4dc3d5264bb432182a28c00
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145347"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a>localsecurityoptionsminimumsessionsecurity 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

localsecurityoptionsminimumsessionsecurity に指定できる値

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|none|.0|LM & NTLM 応答の送信|
|requireNtmlV2SessionSecurity|1-d|LM & NTLM を送信する-ネゴシエートされる場合は NTLMv2 セッションセキュリティを使用する|
|require128BitEncryption|pbm-2|LM & NTLM 応答のみを送信する|
|ntlmV2And128BitEncryption|1/3|LM & NTLMv2 応答のみを送信する|




