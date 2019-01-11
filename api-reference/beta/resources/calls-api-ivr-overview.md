---
title: 呼び出しでの IVR シナリオ
description: Graph で呼び出し元の Api をサポートする対話型音声応答 (IVR) のシナリオは、次のように。
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 014fd2169678617043a5a540f625479e68302b34
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855812"
---
# <a name="ivr-scenarios-in-calls"></a><span data-ttu-id="e93bc-103">呼び出しでの IVR シナリオ</span><span class="sxs-lookup"><span data-stu-id="e93bc-103">IVR scenarios in calls</span></span>

> <span data-ttu-id="e93bc-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e93bc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e93bc-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e93bc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e93bc-106">Graph で呼び出し元の Api をサポートする対話型音声応答 (IVR) のシナリオは、次のように。</span><span class="sxs-lookup"><span data-stu-id="e93bc-106">The following are the Interactive Voice Response (IVR) scenarios that the calling APIs in Microsoft Graph support:</span></span>

- <span data-ttu-id="e93bc-107">オーディオ プロンプトを - たとえば、顧客サービス エージェントのキューに通話が開始するときに再生しています。</span><span class="sxs-lookup"><span data-stu-id="e93bc-107">Playing an audio prompt - for example, when a call is placed in a customer service agent's queue.</span></span>
- <span data-ttu-id="e93bc-108">記録などのオプションを使用してメッセージを耳にした後に通常は、呼び出し元のオーディオを記録します。</span><span class="sxs-lookup"><span data-stu-id="e93bc-108">Record - for example, to record the caller's audio, usually after they heard a prompt with options.</span></span>
- <span data-ttu-id="e93bc-109">購読トーン - たとえば、調、呼び出し元を選択すると、通常のオーディオ プロンプトを聞く後にどのような DTMF を知りたい場合。</span><span class="sxs-lookup"><span data-stu-id="e93bc-109">Subscribe to tone - for example, when you want to know what DTMF tones the caller selected, usually after hearing the audio prompt.</span></span>
- <span data-ttu-id="e93bc-110">プロセスである PlayPrompt またはレコードの操作をキャンセルする場合たとえば、メディア処理をキャンセルします。</span><span class="sxs-lookup"><span data-stu-id="e93bc-110">Cancel Media Processing - for example, when you want to cancel any PlayPrompt or Record operations that might be in process.</span></span>
