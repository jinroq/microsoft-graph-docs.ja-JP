---
title: defenderPotentiallyUnwantedAppAction 列挙型
description: Defender の動作は、可能性のある不要なアプリケーション (PUA) を検出しました。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 96a3dd70ae0f56f2d0d5a9d6c4f87846e10bba45
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938560"
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





