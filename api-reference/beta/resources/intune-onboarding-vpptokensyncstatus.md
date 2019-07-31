---
title: vppTokenSyncStatus 列挙型
description: Apple Volume Purchase Program のトークンに関連付けられている同期状態。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: fca1a785ca16ba3b153e18381d869e598199ed16
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967722"
---
# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="dddea-103">vppTokenSyncStatus 列挙型</span><span class="sxs-lookup"><span data-stu-id="dddea-103">vppTokenSyncStatus enum type</span></span>

> <span data-ttu-id="dddea-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dddea-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dddea-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="dddea-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dddea-106">Apple Volume Purchase Program のトークンに関連付けられている同期状態。</span><span class="sxs-lookup"><span data-stu-id="dddea-106">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="dddea-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="dddea-107">Members</span></span>
|<span data-ttu-id="dddea-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="dddea-108">Member</span></span>|<span data-ttu-id="dddea-109">値</span><span class="sxs-lookup"><span data-stu-id="dddea-109">Value</span></span>|<span data-ttu-id="dddea-110">説明</span><span class="sxs-lookup"><span data-stu-id="dddea-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dddea-111">none</span><span class="sxs-lookup"><span data-stu-id="dddea-111">none</span></span>|<span data-ttu-id="dddea-112">.0</span><span class="sxs-lookup"><span data-stu-id="dddea-112">0</span></span>|<span data-ttu-id="dddea-113">既定の状態です。</span><span class="sxs-lookup"><span data-stu-id="dddea-113">Default status.</span></span>|
|<span data-ttu-id="dddea-114">inProgress</span><span class="sxs-lookup"><span data-stu-id="dddea-114">inProgress</span></span>|<span data-ttu-id="dddea-115">1-d</span><span class="sxs-lookup"><span data-stu-id="dddea-115">1</span></span>|<span data-ttu-id="dddea-116">前回の同期が進行中です。</span><span class="sxs-lookup"><span data-stu-id="dddea-116">Last Sync in progress.</span></span>|
|<span data-ttu-id="dddea-117">せ</span><span class="sxs-lookup"><span data-stu-id="dddea-117">completed</span></span>|<span data-ttu-id="dddea-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="dddea-118">2</span></span>|<span data-ttu-id="dddea-119">前回の同期が正常に完了しました。</span><span class="sxs-lookup"><span data-stu-id="dddea-119">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="dddea-120">フェール</span><span class="sxs-lookup"><span data-stu-id="dddea-120">failed</span></span>|<span data-ttu-id="dddea-121">1/3</span><span class="sxs-lookup"><span data-stu-id="dddea-121">3</span></span>|<span data-ttu-id="dddea-122">前回の同期に失敗しました。</span><span class="sxs-lookup"><span data-stu-id="dddea-122">Last Sync failed.</span></span>|





