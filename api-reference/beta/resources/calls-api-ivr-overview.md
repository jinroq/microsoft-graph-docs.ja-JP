---
title: 通話における IVR シナリオ
description: 次に示す対話式音声応答 (IVR) シナリオでは、Microsoft Graph の呼び出し元 Api がサポートしています。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: conceptualPageType
ms.openlocfilehash: 25f9339f33a6a679a8c8829214526fc29bc88b04
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013040"
---
# <a name="ivr-scenarios-in-calls"></a>通話における IVR シナリオ

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

次に示す対話式音声応答 (IVR) シナリオでは、Microsoft Graph の呼び出し元 Api がサポートしています。

- 音声ガイダンスを再生する-たとえば、カスタマーサービスエージェントのキューに通話が配置された場合です。
- Record-たとえば、発信者の音声を録音する場合、通常は、オプションを含むプロンプトが表示された後に録音します。
- [トーン] (たとえば、発信者が選択した DTMF トーンを知る必要がある場合)、通常は音声プロンプトを聞きます。
- メディア処理をキャンセルします。たとえば、再生プロンプトや、処理中の可能性があるレコード操作を取り消す場合です。
