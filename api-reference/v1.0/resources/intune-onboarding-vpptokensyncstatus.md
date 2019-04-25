---
title: vpptokensyncstatus 列挙型
description: Apple volume purchase program のトークンに関連付けられている同期状態。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6938fd41b6cd7c089b08edb629bc1197ec47c2d7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32548090"
---
# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="ca068-103">vpptokensyncstatus 列挙型</span><span class="sxs-lookup"><span data-stu-id="ca068-103">vppTokenSyncStatus enum type</span></span>

> <span data-ttu-id="ca068-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ca068-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca068-105">Apple volume purchase program のトークンに関連付けられている同期状態。</span><span class="sxs-lookup"><span data-stu-id="ca068-105">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="ca068-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="ca068-106">Members</span></span>
|<span data-ttu-id="ca068-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="ca068-107">Member</span></span>|<span data-ttu-id="ca068-108">値</span><span class="sxs-lookup"><span data-stu-id="ca068-108">Value</span></span>|<span data-ttu-id="ca068-109">説明</span><span class="sxs-lookup"><span data-stu-id="ca068-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca068-110">なし</span><span class="sxs-lookup"><span data-stu-id="ca068-110">none</span></span>|<span data-ttu-id="ca068-111">.0</span><span class="sxs-lookup"><span data-stu-id="ca068-111">0</span></span>|<span data-ttu-id="ca068-112">既定の状態です。</span><span class="sxs-lookup"><span data-stu-id="ca068-112">Default status.</span></span>|
|<span data-ttu-id="ca068-113">inProgress</span><span class="sxs-lookup"><span data-stu-id="ca068-113">inProgress</span></span>|<span data-ttu-id="ca068-114">1 </span><span class="sxs-lookup"><span data-stu-id="ca068-114">1</span></span>|<span data-ttu-id="ca068-115">前回の同期が進行中です。</span><span class="sxs-lookup"><span data-stu-id="ca068-115">Last Sync in progress.</span></span>|
|<span data-ttu-id="ca068-116">せ</span><span class="sxs-lookup"><span data-stu-id="ca068-116">completed</span></span>|<span data-ttu-id="ca068-117">2 </span><span class="sxs-lookup"><span data-stu-id="ca068-117">2</span></span>|<span data-ttu-id="ca068-118">前回の同期が正常に完了しました。</span><span class="sxs-lookup"><span data-stu-id="ca068-118">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="ca068-119">フェール</span><span class="sxs-lookup"><span data-stu-id="ca068-119">failed</span></span>|<span data-ttu-id="ca068-120">3 </span><span class="sxs-lookup"><span data-stu-id="ca068-120">3</span></span>|<span data-ttu-id="ca068-121">前回の同期に失敗しました。</span><span class="sxs-lookup"><span data-stu-id="ca068-121">Last Sync failed.</span></span>|



