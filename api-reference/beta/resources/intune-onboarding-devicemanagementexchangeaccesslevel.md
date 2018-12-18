---
title: deviceManagementExchangeAccessLevel 列挙型
description: Exchange のアクセス レベルです。
author: tfitzmac
ms.openlocfilehash: 8f163c5186c1fc8dac13a22d730870c52df66a06
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320798"
---
# <a name="devicemanagementexchangeaccesslevel-enum-type"></a>deviceManagementExchangeAccessLevel 列挙型

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Exchange のアクセス レベルです。
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|none|0|Exchange では、デバイス アクセス ルールが構成されていません。|
|許可します。|1|デバイスの Exchange へのアクセスを許可します。|
|ブロック|2|デバイスから Exchange へのアクセスをブロックします。|
|検査|3|デバイスを Exchange で隔離します。|





