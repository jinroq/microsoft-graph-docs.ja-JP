---
title: firewallPreSharedKeyEncodingMethodType 列挙型
description: FirewallPreSharedKeyEncodingMethod に指定できる値
author: tfitzmac
ms.openlocfilehash: 3ed2456f54bd27a3efa04d959edba48f7c100692
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27324935"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a>firewallPreSharedKeyEncodingMethodType 列挙型

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

FirewallPreSharedKeyEncodingMethod に指定できる値
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|deviceDefault|0|Intune で構成されている値は、デバイスのユーザーが設定した既定値をオーバーライドしない場合|
|none|1|事前共有キーはエンコードされません。 ワイド文字形式で保存される代わりに、|
|utF8|2|UTF-8 を使用して事前共有キーをエンコードします。|





