---
title: deviceManagementExchangeAccessState 列挙型
description: デバイスの Exchange のアクセスの状態です。
ms.openlocfilehash: e075f3c52dc09d2c762552d3c6580d419f0616f8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069655"
---
# <a name="devicemanagementexchangeaccessstate-enum-type"></a>deviceManagementExchangeAccessState 列挙型

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

デバイスの Exchange のアクセスの状態です。
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|none|0|Exchange から検出アクセス状態がないです。|
|不明|1|Exchange へのデバイスのアクセス状態は不明です。|
|許可|2|デバイスが Exchange へのアクセス権を持つ|
|ブロック|3|デバイスが Exchange でブロックされています。|
|検疫|4|デバイスが Exchange の検疫します。|





