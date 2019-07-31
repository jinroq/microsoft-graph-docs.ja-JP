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
# <a name="ivr-scenarios-in-calls"></a><span data-ttu-id="8c9ec-103">通話における IVR シナリオ</span><span class="sxs-lookup"><span data-stu-id="8c9ec-103">IVR scenarios in calls</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c9ec-104">次に示す対話式音声応答 (IVR) シナリオでは、Microsoft Graph の呼び出し元 Api がサポートしています。</span><span class="sxs-lookup"><span data-stu-id="8c9ec-104">The following are the Interactive Voice Response (IVR) scenarios that the calling APIs in Microsoft Graph support:</span></span>

- <span data-ttu-id="8c9ec-105">音声ガイダンスを再生する-たとえば、カスタマーサービスエージェントのキューに通話が配置された場合です。</span><span class="sxs-lookup"><span data-stu-id="8c9ec-105">Playing an audio prompt - for example, when a call is placed in a customer service agent's queue.</span></span>
- <span data-ttu-id="8c9ec-106">Record-たとえば、発信者の音声を録音する場合、通常は、オプションを含むプロンプトが表示された後に録音します。</span><span class="sxs-lookup"><span data-stu-id="8c9ec-106">Record - for example, to record the caller's audio, usually after they heard a prompt with options.</span></span>
- <span data-ttu-id="8c9ec-107">[トーン] (たとえば、発信者が選択した DTMF トーンを知る必要がある場合)、通常は音声プロンプトを聞きます。</span><span class="sxs-lookup"><span data-stu-id="8c9ec-107">Subscribe to tone - for example, when you want to know what DTMF tones the caller selected, usually after hearing the audio prompt.</span></span>
- <span data-ttu-id="8c9ec-108">メディア処理をキャンセルします。たとえば、再生プロンプトや、処理中の可能性があるレコード操作を取り消す場合です。</span><span class="sxs-lookup"><span data-stu-id="8c9ec-108">Cancel Media Processing - for example, when you want to cancel any PlayPrompt or Record operations that might be in process.</span></span>
