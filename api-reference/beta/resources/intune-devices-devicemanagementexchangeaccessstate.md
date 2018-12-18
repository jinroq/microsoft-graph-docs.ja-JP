---
title: deviceManagementExchangeAccessState 列挙型
description: デバイスの Exchange のアクセスの状態です。
author: tfitzmac
ms.openlocfilehash: cb72a3e07f0f14fdd509bb0274605cb9592db241
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328743"
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





