---
title: vpptokensyncstatus 列挙型
description: Apple volume purchase program のトークンに関連付けられている同期状態。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 59653a8df6c0fd08ffd0d8aa3081d58e56447a95
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566375"
---
# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="86543-103">vpptokensyncstatus 列挙型</span><span class="sxs-lookup"><span data-stu-id="86543-103">vppTokenSyncStatus enum type</span></span>

> <span data-ttu-id="86543-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="86543-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="86543-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="86543-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86543-106">Apple volume purchase program のトークンに関連付けられている同期状態。</span><span class="sxs-lookup"><span data-stu-id="86543-106">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="86543-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="86543-107">Members</span></span>
|<span data-ttu-id="86543-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="86543-108">Member</span></span>|<span data-ttu-id="86543-109">値</span><span class="sxs-lookup"><span data-stu-id="86543-109">Value</span></span>|<span data-ttu-id="86543-110">説明</span><span class="sxs-lookup"><span data-stu-id="86543-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86543-111">なし</span><span class="sxs-lookup"><span data-stu-id="86543-111">none</span></span>|<span data-ttu-id="86543-112">.0</span><span class="sxs-lookup"><span data-stu-id="86543-112">0</span></span>|<span data-ttu-id="86543-113">既定の状態です。</span><span class="sxs-lookup"><span data-stu-id="86543-113">Default status.</span></span>|
|<span data-ttu-id="86543-114">inProgress</span><span class="sxs-lookup"><span data-stu-id="86543-114">inProgress</span></span>|<span data-ttu-id="86543-115">1 </span><span class="sxs-lookup"><span data-stu-id="86543-115">1</span></span>|<span data-ttu-id="86543-116">前回の同期が進行中です。</span><span class="sxs-lookup"><span data-stu-id="86543-116">Last Sync in progress.</span></span>|
|<span data-ttu-id="86543-117">せ</span><span class="sxs-lookup"><span data-stu-id="86543-117">completed</span></span>|<span data-ttu-id="86543-118">2 </span><span class="sxs-lookup"><span data-stu-id="86543-118">2</span></span>|<span data-ttu-id="86543-119">前回の同期が正常に完了しました。</span><span class="sxs-lookup"><span data-stu-id="86543-119">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="86543-120">フェール</span><span class="sxs-lookup"><span data-stu-id="86543-120">failed</span></span>|<span data-ttu-id="86543-121">3 </span><span class="sxs-lookup"><span data-stu-id="86543-121">3</span></span>|<span data-ttu-id="86543-122">前回の同期に失敗しました。</span><span class="sxs-lookup"><span data-stu-id="86543-122">Last Sync failed.</span></span>|





