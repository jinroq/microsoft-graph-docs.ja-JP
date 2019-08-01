---
title: vppTokenSyncStatus 列挙型
description: Apple Volume Purchase Program のトークンに関連付けられている同期状態。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 7af4ed87234dc588a9d0969d2ed347adaa4d29da
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037231"
---
# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="127ba-103">vppTokenSyncStatus 列挙型</span><span class="sxs-lookup"><span data-stu-id="127ba-103">vppTokenSyncStatus enum type</span></span>

> <span data-ttu-id="127ba-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="127ba-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="127ba-105">Apple Volume Purchase Program のトークンに関連付けられている同期状態。</span><span class="sxs-lookup"><span data-stu-id="127ba-105">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="127ba-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="127ba-106">Members</span></span>
|<span data-ttu-id="127ba-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="127ba-107">Member</span></span>|<span data-ttu-id="127ba-108">値</span><span class="sxs-lookup"><span data-stu-id="127ba-108">Value</span></span>|<span data-ttu-id="127ba-109">説明</span><span class="sxs-lookup"><span data-stu-id="127ba-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="127ba-110">none</span><span class="sxs-lookup"><span data-stu-id="127ba-110">none</span></span>|<span data-ttu-id="127ba-111">.0</span><span class="sxs-lookup"><span data-stu-id="127ba-111">0</span></span>|<span data-ttu-id="127ba-112">既定の状態です。</span><span class="sxs-lookup"><span data-stu-id="127ba-112">Default status.</span></span>|
|<span data-ttu-id="127ba-113">inProgress</span><span class="sxs-lookup"><span data-stu-id="127ba-113">inProgress</span></span>|<span data-ttu-id="127ba-114">1-d</span><span class="sxs-lookup"><span data-stu-id="127ba-114">1</span></span>|<span data-ttu-id="127ba-115">前回の同期が進行中です。</span><span class="sxs-lookup"><span data-stu-id="127ba-115">Last Sync in progress.</span></span>|
|<span data-ttu-id="127ba-116">せ</span><span class="sxs-lookup"><span data-stu-id="127ba-116">completed</span></span>|<span data-ttu-id="127ba-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="127ba-117">2</span></span>|<span data-ttu-id="127ba-118">前回の同期が正常に完了しました。</span><span class="sxs-lookup"><span data-stu-id="127ba-118">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="127ba-119">フェール</span><span class="sxs-lookup"><span data-stu-id="127ba-119">failed</span></span>|<span data-ttu-id="127ba-120">1/3</span><span class="sxs-lookup"><span data-stu-id="127ba-120">3</span></span>|<span data-ttu-id="127ba-121">前回の同期に失敗しました。</span><span class="sxs-lookup"><span data-stu-id="127ba-121">Last Sync failed.</span></span>|



