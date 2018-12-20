---
title: 呼び出しでの IVR シナリオ
description: Graph で呼び出し元の Api をサポートする対話型音声応答 (IVR) のシナリオは、次のように。
author: VinodRavichandran
ms.openlocfilehash: cf7d6543c09b69050db9aedc270616cfea113c28
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380470"
---
# <a name="ivr-scenarios-in-calls"></a>呼び出しでの IVR シナリオ

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

Graph で呼び出し元の Api をサポートする対話型音声応答 (IVR) のシナリオは、次のように。

- オーディオ プロンプトを - たとえば、顧客サービス エージェントのキューに通話が開始するときに再生しています。
- 記録などのオプションを使用してメッセージを耳にした後に通常は、呼び出し元のオーディオを記録します。
- 購読トーン - たとえば、調、呼び出し元を選択すると、通常のオーディオ プロンプトを聞く後にどのような DTMF を知りたい場合。
- プロセスである PlayPrompt またはレコードの操作をキャンセルする場合たとえば、メディア処理をキャンセルします。
