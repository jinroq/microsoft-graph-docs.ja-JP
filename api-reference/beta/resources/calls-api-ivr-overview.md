---
title: 通話における IVR シナリオ
description: 次に示す対話式音声応答 (IVR) シナリオでは、Microsoft Graph の呼び出し元 api がサポートしています。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 69023de179714797156f8ed039e2086e060fe9b1
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33338783"
---
# <a name="ivr-scenarios-in-calls"></a>通話における IVR シナリオ

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

次に示す対話式音声応答 (IVR) シナリオでは、Microsoft Graph の呼び出し元 api がサポートしています。

- 音声ガイダンスを再生する-たとえば、カスタマーサービスエージェントのキューに通話が配置された場合です。
- record-たとえば、発信者の音声を録音する場合、通常は、オプションを含むプロンプトが表示された後に録音します。
- [トーン] (たとえば、発信者が選択した DTMF トーンを知る必要がある場合)、通常は音声プロンプトを聞きます。
- メディア処理をキャンセルします。たとえば、再生プロンプトや、処理中の可能性があるレコード操作を取り消す場合です。
