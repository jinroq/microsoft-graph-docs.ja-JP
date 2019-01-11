---
title: defenderThreatAction 列挙型
description: Defender の既定のアクション実行するには、マルウェアの脅威が検出されました。
localization_priority: Normal
ms.openlocfilehash: 7e448e6fae0ebbb0f14a3b7932e6f306a70588b9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837871"
---
# <a name="defenderthreataction-enum-type"></a>defenderThreatAction 列挙型

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Defender の既定のアクション実行するには、マルウェアの脅威が検出されました。
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|deviceDefault|0|更新プログラム定義に基づいたアクションを適用します。|
|クリーン|1|検出された脅威をクリーニングします。|
|検査|2|検出された脅威を隔離します。|
|remove|3|検出された脅威を削除します。|
|許可します。|4|脅威の検出を許可します。|
|ユーザー定義|5|検出された脅威に対して実行するアクションを決定するユーザーを許可します。|
|ブロック|6|検出された脅威をブロックします。|





