---
title: defenderThreatAction 列挙型
description: Defender の既定のアクション実行するには、マルウェアの脅威が検出されました。
ms.openlocfilehash: d6a4ccbc9725c230f6abc7bd9ee1e38a30d5d133
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066491"
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





