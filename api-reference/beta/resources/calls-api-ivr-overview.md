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
# <a name="ivr-scenarios-in-calls"></a><span data-ttu-id="8c2e1-103">通話における IVR シナリオ</span><span class="sxs-lookup"><span data-stu-id="8c2e1-103">IVR scenarios in calls</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c2e1-104">次に示す対話式音声応答 (IVR) シナリオでは、Microsoft Graph の呼び出し元 api がサポートしています。</span><span class="sxs-lookup"><span data-stu-id="8c2e1-104">The following are the Interactive Voice Response (IVR) scenarios that the calling APIs in Microsoft Graph support:</span></span>

- <span data-ttu-id="8c2e1-105">音声ガイダンスを再生する-たとえば、カスタマーサービスエージェントのキューに通話が配置された場合です。</span><span class="sxs-lookup"><span data-stu-id="8c2e1-105">Playing an audio prompt - for example, when a call is placed in a customer service agent's queue.</span></span>
- <span data-ttu-id="8c2e1-106">record-たとえば、発信者の音声を録音する場合、通常は、オプションを含むプロンプトが表示された後に録音します。</span><span class="sxs-lookup"><span data-stu-id="8c2e1-106">Record - for example, to record the caller's audio, usually after they heard a prompt with options.</span></span>
- <span data-ttu-id="8c2e1-107">[トーン] (たとえば、発信者が選択した DTMF トーンを知る必要がある場合)、通常は音声プロンプトを聞きます。</span><span class="sxs-lookup"><span data-stu-id="8c2e1-107">Subscribe to tone - for example, when you want to know what DTMF tones the caller selected, usually after hearing the audio prompt.</span></span>
- <span data-ttu-id="8c2e1-108">メディア処理をキャンセルします。たとえば、再生プロンプトや、処理中の可能性があるレコード操作を取り消す場合です。</span><span class="sxs-lookup"><span data-stu-id="8c2e1-108">Cancel Media Processing - for example, when you want to cancel any PlayPrompt or Record operations that might be in process.</span></span>
