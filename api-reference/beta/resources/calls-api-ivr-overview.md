---
title: 呼び出しでの IVR シナリオ
description: Graph で呼び出し元の Api をサポートする対話型音声応答 (IVR) のシナリオは、次のように。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: a3657d60344941de931e4f77bddde922d7d01f21
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27936362"
---
# <a name="ivr-scenarios-in-calls"></a>呼び出しでの IVR シナリオ

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

Graph で呼び出し元の Api をサポートする対話型音声応答 (IVR) のシナリオは、次のように。

- オーディオ プロンプトを - たとえば、顧客サービス エージェントのキューに通話が開始するときに再生しています。
- 記録などのオプションを使用してメッセージを耳にした後に通常は、呼び出し元のオーディオを記録します。
- 購読トーン - たとえば、調、呼び出し元を選択すると、通常のオーディオ プロンプトを聞く後にどのような DTMF を知りたい場合。
- プロセスである PlayPrompt またはレコードの操作をキャンセルする場合たとえば、メディア処理をキャンセルします。
