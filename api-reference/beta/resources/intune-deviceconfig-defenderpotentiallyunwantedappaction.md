---
title: defenderPotentiallyUnwantedAppAction 列挙型
description: Defender の動作は、可能性のある不要なアプリケーション (PUA) を検出しました。
localization_priority: Normal
ms.openlocfilehash: 9b04cd6daeae303910519d0735165171575d8c44
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858647"
---
# <a name="defenderpotentiallyunwantedappaction-enum-type"></a>defenderPotentiallyUnwantedAppAction 列挙型

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Defender の動作は、可能性のある不要なアプリケーション (PUA) を検出しました。
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|deviceDefault|0|私用領域の保護では、無効です。 Defender は、望ましくない可能性のあるアプリケーションに対して保護されなくなります。|
|ブロック|1|私用領域の保護を有効にします。 検出された項目がブロックされます。 履歴とその他の脅威に表示されます。|
|監査|2|監査モードにします。 Defender は、可能性のある不要なアプリケーションを検出が、アクションを実行しません。 Defender はアクションを実行したと、イベント ビューアーの Defender によって作成されたイベントを検索して、アプリケーションに関する情報を確認することができます。|





