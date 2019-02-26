---
title: vpptokensyncstatus 列挙型
description: Apple volume purchase program のトークンに関連付けられている同期状態。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6938fd41b6cd7c089b08edb629bc1197ec47c2d7
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254052"
---
# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="1d100-103">vpptokensyncstatus 列挙型</span><span class="sxs-lookup"><span data-stu-id="1d100-103">vppTokenSyncStatus enum type</span></span>

> <span data-ttu-id="1d100-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1d100-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d100-105">Apple volume purchase program のトークンに関連付けられている同期状態。</span><span class="sxs-lookup"><span data-stu-id="1d100-105">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="1d100-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="1d100-106">Members</span></span>
|<span data-ttu-id="1d100-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="1d100-107">Member</span></span>|<span data-ttu-id="1d100-108">値</span><span class="sxs-lookup"><span data-stu-id="1d100-108">Value</span></span>|<span data-ttu-id="1d100-109">説明</span><span class="sxs-lookup"><span data-stu-id="1d100-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d100-110">none</span><span class="sxs-lookup"><span data-stu-id="1d100-110">none</span></span>|<span data-ttu-id="1d100-111">.0</span><span class="sxs-lookup"><span data-stu-id="1d100-111">0</span></span>|<span data-ttu-id="1d100-112">既定の状態です。</span><span class="sxs-lookup"><span data-stu-id="1d100-112">Default status.</span></span>|
|<span data-ttu-id="1d100-113">inProgress</span><span class="sxs-lookup"><span data-stu-id="1d100-113">inProgress</span></span>|<span data-ttu-id="1d100-114">1-d</span><span class="sxs-lookup"><span data-stu-id="1d100-114">1</span></span>|<span data-ttu-id="1d100-115">前回の同期が進行中です。</span><span class="sxs-lookup"><span data-stu-id="1d100-115">Last Sync in progress.</span></span>|
|<span data-ttu-id="1d100-116">せ</span><span class="sxs-lookup"><span data-stu-id="1d100-116">completed</span></span>|<span data-ttu-id="1d100-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="1d100-117">2</span></span>|<span data-ttu-id="1d100-118">前回の同期が正常に完了しました。</span><span class="sxs-lookup"><span data-stu-id="1d100-118">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="1d100-119">フェール</span><span class="sxs-lookup"><span data-stu-id="1d100-119">failed</span></span>|<span data-ttu-id="1d100-120">1/3</span><span class="sxs-lookup"><span data-stu-id="1d100-120">3</span></span>|<span data-ttu-id="1d100-121">前回の同期に失敗しました。</span><span class="sxs-lookup"><span data-stu-id="1d100-121">Last Sync failed.</span></span>|



