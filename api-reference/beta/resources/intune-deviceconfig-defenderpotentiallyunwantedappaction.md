---
title: defenderPotentiallyUnwantedAppAction 列挙型
description: Defender の動作は、可能性のある不要なアプリケーション (PUA) を検出しました。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 96a3dd70ae0f56f2d0d5a9d6c4f87846e10bba45
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938560"
---
# <a name="defenderpotentiallyunwantedappaction-enum-type"></a><span data-ttu-id="b89ed-103">defenderPotentiallyUnwantedAppAction 列挙型</span><span class="sxs-lookup"><span data-stu-id="b89ed-103">defenderPotentiallyUnwantedAppAction enum type</span></span>

> <span data-ttu-id="b89ed-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b89ed-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b89ed-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b89ed-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b89ed-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b89ed-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b89ed-107">Defender の動作は、可能性のある不要なアプリケーション (PUA) を検出しました。</span><span class="sxs-lookup"><span data-stu-id="b89ed-107">Defender’s action to take on detected Potentially Unwanted Application (PUA).</span></span>
## <a name="members"></a><span data-ttu-id="b89ed-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="b89ed-108">Members</span></span>
|<span data-ttu-id="b89ed-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="b89ed-109">Member</span></span>|<span data-ttu-id="b89ed-110">値</span><span class="sxs-lookup"><span data-stu-id="b89ed-110">Value</span></span>|<span data-ttu-id="b89ed-111">説明</span><span class="sxs-lookup"><span data-stu-id="b89ed-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b89ed-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="b89ed-112">deviceDefault</span></span>|<span data-ttu-id="b89ed-113">0</span><span class="sxs-lookup"><span data-stu-id="b89ed-113">0</span></span>|<span data-ttu-id="b89ed-114">私用領域の保護では、無効です。</span><span class="sxs-lookup"><span data-stu-id="b89ed-114">PUA Protection is off.</span></span> <span data-ttu-id="b89ed-115">Defender は、望ましくない可能性のあるアプリケーションに対して保護されなくなります。</span><span class="sxs-lookup"><span data-stu-id="b89ed-115">Defender will not protect against potentially unwanted applications.</span></span>|
|<span data-ttu-id="b89ed-116">ブロック</span><span class="sxs-lookup"><span data-stu-id="b89ed-116">block</span></span>|<span data-ttu-id="b89ed-117">1</span><span class="sxs-lookup"><span data-stu-id="b89ed-117">1</span></span>|<span data-ttu-id="b89ed-118">私用領域の保護を有効にします。</span><span class="sxs-lookup"><span data-stu-id="b89ed-118">PUA Protection is on.</span></span> <span data-ttu-id="b89ed-119">検出された項目がブロックされます。</span><span class="sxs-lookup"><span data-stu-id="b89ed-119">Detected items are blocked.</span></span> <span data-ttu-id="b89ed-120">履歴とその他の脅威に表示されます。</span><span class="sxs-lookup"><span data-stu-id="b89ed-120">They will show in history along with other threats.</span></span>|
|<span data-ttu-id="b89ed-121">監査</span><span class="sxs-lookup"><span data-stu-id="b89ed-121">audit</span></span>|<span data-ttu-id="b89ed-122">2</span><span class="sxs-lookup"><span data-stu-id="b89ed-122">2</span></span>|<span data-ttu-id="b89ed-123">監査モードにします。</span><span class="sxs-lookup"><span data-stu-id="b89ed-123">Audit mode.</span></span> <span data-ttu-id="b89ed-124">Defender は、可能性のある不要なアプリケーションを検出が、アクションを実行しません。</span><span class="sxs-lookup"><span data-stu-id="b89ed-124">Defender will detect potentially unwanted applications, but take no actions.</span></span> <span data-ttu-id="b89ed-125">Defender はアクションを実行したと、イベント ビューアーの Defender によって作成されたイベントを検索して、アプリケーションに関する情報を確認することができます。</span><span class="sxs-lookup"><span data-stu-id="b89ed-125">You can review information about applications Defender would have taken action against by searching for events created by Defender in the Event Viewer.</span></span>|





