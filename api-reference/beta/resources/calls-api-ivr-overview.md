---
title: 呼び出しでの IVR シナリオ
description: Graph で呼び出し元の Api をサポートする対話型音声応答 (IVR) のシナリオは、次のように。
ms.openlocfilehash: 22318b2bc755b161a55fc42fd924017545d38e3b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066559"
---
# <a name="ivr-scenarios-in-calls"></a>呼び出しでの IVR シナリオ

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

Graph で呼び出し元の Api をサポートする対話型音声応答 (IVR) のシナリオは、次のように。

- オーディオ プロンプトを - たとえば、顧客サービス エージェントのキューに通話が開始するときに再生しています。
- 記録などのオプションを使用してメッセージを耳にした後に通常は、呼び出し元のオーディオを記録します。
- 購読トーン - たとえば、調、呼び出し元を選択すると、通常のオーディオ プロンプトを聞く後にどのような DTMF を知りたい場合。
- プロセスである PlayPrompt またはレコードの操作をキャンセルする場合たとえば、メディア処理をキャンセルします。
