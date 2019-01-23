---
title: lanManagerAuthenticationLevel 列挙型
description: LanManagerAuthenticationLevel に指定できる値
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6e8c7b3df6f515d3dad0d7619b6c0b755ad799d7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29397457"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a>lanManagerAuthenticationLevel 列挙型

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

LanManagerAuthenticationLevel に指定できる値

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|lmAndNltm|0|NTLM 応答を送信するには、LM &|
|lmNtlmAndNtlmV2|1|LM NTLM の使用を & の NTLMv2 セッション セキュリティをネゴシエートされた場合に送信します。|
|lmAndNtlmOnly|2|NTLM 応答のみを送信するには、LM &|
|lmAndNtlmV2|3|NTLMv2 応答のみを送信するには、LM &|
|lmNtlmV2AndNotLm|4|LM & NTLMv2 応答のみを送信します。 LM を拒否します。|
|lmNtlmV2AndNotLmOrNtm|5|LM & NTLMv2 応答のみを送信します。 LM & NTLM を拒否します。|




