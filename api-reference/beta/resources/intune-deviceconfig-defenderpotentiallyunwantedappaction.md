---
title: defenderPotentiallyUnwantedAppAction 列挙型
description: Defender の動作は、可能性のある不要なアプリケーション (PUA) を検出しました。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2ace0cc29ad284cde63b7e4934fb8cb395f27bbe
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422755"
---
# <a name="defenderpotentiallyunwantedappaction-enum-type"></a><span data-ttu-id="70ae1-103">defenderPotentiallyUnwantedAppAction 列挙型</span><span class="sxs-lookup"><span data-stu-id="70ae1-103">defenderPotentiallyUnwantedAppAction enum type</span></span>

> <span data-ttu-id="70ae1-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="70ae1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="70ae1-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="70ae1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="70ae1-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="70ae1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="70ae1-107">Defender の動作は、可能性のある不要なアプリケーション (PUA) を検出しました。</span><span class="sxs-lookup"><span data-stu-id="70ae1-107">Defender’s action to take on detected Potentially Unwanted Application (PUA).</span></span>

## <a name="members"></a><span data-ttu-id="70ae1-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="70ae1-108">Members</span></span>
|<span data-ttu-id="70ae1-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="70ae1-109">Member</span></span>|<span data-ttu-id="70ae1-110">値</span><span class="sxs-lookup"><span data-stu-id="70ae1-110">Value</span></span>|<span data-ttu-id="70ae1-111">説明</span><span class="sxs-lookup"><span data-stu-id="70ae1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70ae1-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="70ae1-112">deviceDefault</span></span>|<span data-ttu-id="70ae1-113">0</span><span class="sxs-lookup"><span data-stu-id="70ae1-113">0</span></span>|<span data-ttu-id="70ae1-114">私用領域の保護では、無効です。</span><span class="sxs-lookup"><span data-stu-id="70ae1-114">PUA Protection is off.</span></span> <span data-ttu-id="70ae1-115">Defender は、望ましくない可能性のあるアプリケーションに対して保護されなくなります。</span><span class="sxs-lookup"><span data-stu-id="70ae1-115">Defender will not protect against potentially unwanted applications.</span></span>|
|<span data-ttu-id="70ae1-116">ブロック</span><span class="sxs-lookup"><span data-stu-id="70ae1-116">block</span></span>|<span data-ttu-id="70ae1-117">1</span><span class="sxs-lookup"><span data-stu-id="70ae1-117">1</span></span>|<span data-ttu-id="70ae1-118">私用領域の保護を有効にします。</span><span class="sxs-lookup"><span data-stu-id="70ae1-118">PUA Protection is on.</span></span> <span data-ttu-id="70ae1-119">検出された項目がブロックされます。</span><span class="sxs-lookup"><span data-stu-id="70ae1-119">Detected items are blocked.</span></span> <span data-ttu-id="70ae1-120">履歴とその他の脅威に表示されます。</span><span class="sxs-lookup"><span data-stu-id="70ae1-120">They will show in history along with other threats.</span></span>|
|<span data-ttu-id="70ae1-121">監査</span><span class="sxs-lookup"><span data-stu-id="70ae1-121">audit</span></span>|<span data-ttu-id="70ae1-122">2</span><span class="sxs-lookup"><span data-stu-id="70ae1-122">2</span></span>|<span data-ttu-id="70ae1-123">監査モードにします。</span><span class="sxs-lookup"><span data-stu-id="70ae1-123">Audit mode.</span></span> <span data-ttu-id="70ae1-124">Defender は、可能性のある不要なアプリケーションを検出が、アクションを実行しません。</span><span class="sxs-lookup"><span data-stu-id="70ae1-124">Defender will detect potentially unwanted applications, but take no actions.</span></span> <span data-ttu-id="70ae1-125">Defender はアクションを実行したと、イベント ビューアーの Defender によって作成されたイベントを検索して、アプリケーションに関する情報を確認することができます。</span><span class="sxs-lookup"><span data-stu-id="70ae1-125">You can review information about applications Defender would have taken action against by searching for events created by Defender in the Event Viewer.</span></span>|




