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
# <a name="ivr-scenarios-in-calls"></a><span data-ttu-id="f940a-103">呼び出しでの IVR シナリオ</span><span class="sxs-lookup"><span data-stu-id="f940a-103">IVR scenarios in calls</span></span>

> <span data-ttu-id="f940a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f940a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f940a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f940a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f940a-106">Graph で呼び出し元の Api をサポートする対話型音声応答 (IVR) のシナリオは、次のように。</span><span class="sxs-lookup"><span data-stu-id="f940a-106">The following are the Interactive Voice Response (IVR) scenarios that the calling APIs in Microsoft Graph support:</span></span>

- <span data-ttu-id="f940a-107">オーディオ プロンプトを - たとえば、顧客サービス エージェントのキューに通話が開始するときに再生しています。</span><span class="sxs-lookup"><span data-stu-id="f940a-107">Playing an audio prompt - for example, when a call is placed in a customer service agent's queue.</span></span>
- <span data-ttu-id="f940a-108">記録などのオプションを使用してメッセージを耳にした後に通常は、呼び出し元のオーディオを記録します。</span><span class="sxs-lookup"><span data-stu-id="f940a-108">Record - for example, to record the caller's audio, usually after they heard a prompt with options.</span></span>
- <span data-ttu-id="f940a-109">購読トーン - たとえば、調、呼び出し元を選択すると、通常のオーディオ プロンプトを聞く後にどのような DTMF を知りたい場合。</span><span class="sxs-lookup"><span data-stu-id="f940a-109">Subscribe to tone - for example, when you want to know what DTMF tones the caller selected, usually after hearing the audio prompt.</span></span>
- <span data-ttu-id="f940a-110">プロセスである PlayPrompt またはレコードの操作をキャンセルする場合たとえば、メディア処理をキャンセルします。</span><span class="sxs-lookup"><span data-stu-id="f940a-110">Cancel Media Processing - for example, when you want to cancel any PlayPrompt or Record operations that might be in process.</span></span>
