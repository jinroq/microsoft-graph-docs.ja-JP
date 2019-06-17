---
title: defenderPotentiallyUnwantedAppAction 列挙型
description: 検出された望ましくない可能性があるアプリケーション (PUA) に対して実行する、Defender のアクション。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3816fe9e4366d21ddab43558ea6ab703a2d4d660
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34979859"
---
# <a name="defenderpotentiallyunwantedappaction-enum-type"></a><span data-ttu-id="ffec3-103">defenderPotentiallyUnwantedAppAction 列挙型</span><span class="sxs-lookup"><span data-stu-id="ffec3-103">defenderPotentiallyUnwantedAppAction enum type</span></span>

> <span data-ttu-id="ffec3-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ffec3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ffec3-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ffec3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ffec3-106">検出された望ましくない可能性があるアプリケーション (PUA) に対して実行する、Defender のアクション。</span><span class="sxs-lookup"><span data-stu-id="ffec3-106">Defender’s action to take on detected Potentially Unwanted Application (PUA).</span></span>

## <a name="members"></a><span data-ttu-id="ffec3-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="ffec3-107">Members</span></span>
|<span data-ttu-id="ffec3-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="ffec3-108">Member</span></span>|<span data-ttu-id="ffec3-109">値</span><span class="sxs-lookup"><span data-stu-id="ffec3-109">Value</span></span>|<span data-ttu-id="ffec3-110">説明</span><span class="sxs-lookup"><span data-stu-id="ffec3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ffec3-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="ffec3-111">deviceDefault</span></span>|<span data-ttu-id="ffec3-112">.0</span><span class="sxs-lookup"><span data-stu-id="ffec3-112">0</span></span>|<span data-ttu-id="ffec3-113">PUA の保護がオフになっています。</span><span class="sxs-lookup"><span data-stu-id="ffec3-113">PUA Protection is off.</span></span> <span data-ttu-id="ffec3-114">Defender は望ましくない可能性があるアプリケーションに対する保護を行いません。</span><span class="sxs-lookup"><span data-stu-id="ffec3-114">Defender will not protect against potentially unwanted applications.</span></span>|
|<span data-ttu-id="ffec3-115">拒否</span><span class="sxs-lookup"><span data-stu-id="ffec3-115">block</span></span>|<span data-ttu-id="ffec3-116">1-d</span><span class="sxs-lookup"><span data-stu-id="ffec3-116">1</span></span>|<span data-ttu-id="ffec3-117">PUA の保護がオンになっています。</span><span class="sxs-lookup"><span data-stu-id="ffec3-117">PUA Protection is on.</span></span> <span data-ttu-id="ffec3-118">検出されたアイテムはブロックされます。</span><span class="sxs-lookup"><span data-stu-id="ffec3-118">Detected items are blocked.</span></span> <span data-ttu-id="ffec3-119">これらのメンバーは、他の脅威と共に履歴に表示されます。</span><span class="sxs-lookup"><span data-stu-id="ffec3-119">They will show in history along with other threats.</span></span>|
|<span data-ttu-id="ffec3-120">監査</span><span class="sxs-lookup"><span data-stu-id="ffec3-120">audit</span></span>|<span data-ttu-id="ffec3-121">pbm-2</span><span class="sxs-lookup"><span data-stu-id="ffec3-121">2</span></span>|<span data-ttu-id="ffec3-122">監査モード。</span><span class="sxs-lookup"><span data-stu-id="ffec3-122">Audit mode.</span></span> <span data-ttu-id="ffec3-123">Defender は望ましくない可能性があるアプリケーションを検出しますが、アクションは実行しません。</span><span class="sxs-lookup"><span data-stu-id="ffec3-123">Defender will detect potentially unwanted applications, but take no actions.</span></span> <span data-ttu-id="ffec3-124">イベントビューアーで、Defender によって作成されたイベントを検索することによって、アプリケーション Defender が操作を実行したことについての情報を確認できます。</span><span class="sxs-lookup"><span data-stu-id="ffec3-124">You can review information about applications Defender would have taken action against by searching for events created by Defender in the Event Viewer.</span></span>|





