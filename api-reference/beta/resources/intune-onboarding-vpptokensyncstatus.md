---
title: vpptokensyncstatus 列挙型
description: Apple volume purchase program のトークンに関連付けられている同期状態。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 46de00423a08e7edc6f5ac9c62d1caf0165e1d94
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30170428"
---
# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="d1a52-103">vpptokensyncstatus 列挙型</span><span class="sxs-lookup"><span data-stu-id="d1a52-103">vppTokenSyncStatus enum type</span></span>

> <span data-ttu-id="d1a52-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d1a52-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d1a52-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d1a52-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1a52-106">Apple volume purchase program のトークンに関連付けられている同期状態。</span><span class="sxs-lookup"><span data-stu-id="d1a52-106">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="d1a52-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="d1a52-107">Members</span></span>
|<span data-ttu-id="d1a52-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="d1a52-108">Member</span></span>|<span data-ttu-id="d1a52-109">値</span><span class="sxs-lookup"><span data-stu-id="d1a52-109">Value</span></span>|<span data-ttu-id="d1a52-110">説明</span><span class="sxs-lookup"><span data-stu-id="d1a52-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1a52-111">none</span><span class="sxs-lookup"><span data-stu-id="d1a52-111">none</span></span>|<span data-ttu-id="d1a52-112">.0</span><span class="sxs-lookup"><span data-stu-id="d1a52-112">0</span></span>|<span data-ttu-id="d1a52-113">既定の状態です。</span><span class="sxs-lookup"><span data-stu-id="d1a52-113">Default status.</span></span>|
|<span data-ttu-id="d1a52-114">inProgress</span><span class="sxs-lookup"><span data-stu-id="d1a52-114">inProgress</span></span>|<span data-ttu-id="d1a52-115">1-d</span><span class="sxs-lookup"><span data-stu-id="d1a52-115">1</span></span>|<span data-ttu-id="d1a52-116">前回の同期が進行中です。</span><span class="sxs-lookup"><span data-stu-id="d1a52-116">Last Sync in progress.</span></span>|
|<span data-ttu-id="d1a52-117">せ</span><span class="sxs-lookup"><span data-stu-id="d1a52-117">completed</span></span>|<span data-ttu-id="d1a52-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="d1a52-118">2</span></span>|<span data-ttu-id="d1a52-119">前回の同期が正常に完了しました。</span><span class="sxs-lookup"><span data-stu-id="d1a52-119">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="d1a52-120">フェール</span><span class="sxs-lookup"><span data-stu-id="d1a52-120">failed</span></span>|<span data-ttu-id="d1a52-121">1/3</span><span class="sxs-lookup"><span data-stu-id="d1a52-121">3</span></span>|<span data-ttu-id="d1a52-122">前回の同期に失敗しました。</span><span class="sxs-lookup"><span data-stu-id="d1a52-122">Last Sync failed.</span></span>|




