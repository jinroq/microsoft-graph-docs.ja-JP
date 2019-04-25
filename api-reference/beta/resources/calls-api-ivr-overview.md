---
title: 通話における IVR シナリオ
description: 次に示す対話式音声応答 (IVR) シナリオでは、Microsoft Graph の呼び出し元 api がサポートしています。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: aed30bc5ad109dc3f21d381f4d6b04e087a779a3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535569"
---
# <a name="ivr-scenarios-in-calls"></a><span data-ttu-id="f1f12-103">通話における IVR シナリオ</span><span class="sxs-lookup"><span data-stu-id="f1f12-103">IVR scenarios in calls</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1f12-104">次に示す対話式音声応答 (IVR) シナリオでは、Microsoft Graph の呼び出し元 api がサポートしています。</span><span class="sxs-lookup"><span data-stu-id="f1f12-104">The following are the Interactive Voice Response (IVR) scenarios that the calling APIs in Microsoft Graph support:</span></span>

- <span data-ttu-id="f1f12-105">音声ガイダンスを再生する-たとえば、カスタマーサービスエージェントのキューに通話が配置された場合です。</span><span class="sxs-lookup"><span data-stu-id="f1f12-105">Playing an audio prompt - for example, when a call is placed in a customer service agent's queue.</span></span>
- <span data-ttu-id="f1f12-106">record-たとえば、発信者の音声を録音する場合、通常は、オプションを含むプロンプトが表示された後に録音します。</span><span class="sxs-lookup"><span data-stu-id="f1f12-106">Record - for example, to record the caller's audio, usually after they heard a prompt with options.</span></span>
- <span data-ttu-id="f1f12-107">[トーン] (たとえば、発信者が選択した DTMF トーンを知る必要がある場合)、通常は音声プロンプトを聞きます。</span><span class="sxs-lookup"><span data-stu-id="f1f12-107">Subscribe to tone - for example, when you want to know what DTMF tones the caller selected, usually after hearing the audio prompt.</span></span>
- <span data-ttu-id="f1f12-108">メディア処理をキャンセルします。たとえば、再生プロンプトや、処理中の可能性があるレコード操作を取り消す場合です。</span><span class="sxs-lookup"><span data-stu-id="f1f12-108">Cancel Media Processing - for example, when you want to cancel any PlayPrompt or Record operations that might be in process.</span></span>
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/calls-api-ivr-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
