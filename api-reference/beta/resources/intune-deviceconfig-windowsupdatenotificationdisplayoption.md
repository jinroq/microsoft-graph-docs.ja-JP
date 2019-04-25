---
title: windowsUpdateNotificationDisplayOption 列挙型
description: Windows Update 通知の表示オプション
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7e792e3a866a0fadae5f866654e50ffe16cdc4c0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523644"
---
# <a name="windowsupdatenotificationdisplayoption-enum-type"></a><span data-ttu-id="eff55-103">windowsUpdateNotificationDisplayOption 列挙型</span><span class="sxs-lookup"><span data-stu-id="eff55-103">windowsUpdateNotificationDisplayOption enum type</span></span>

> <span data-ttu-id="eff55-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eff55-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eff55-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="eff55-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eff55-106">Windows Update 通知の表示オプション</span><span class="sxs-lookup"><span data-stu-id="eff55-106">Windows Update Notification Display Options</span></span>

## <a name="members"></a><span data-ttu-id="eff55-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="eff55-107">Members</span></span>
|<span data-ttu-id="eff55-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="eff55-108">Member</span></span>|<span data-ttu-id="eff55-109">値</span><span class="sxs-lookup"><span data-stu-id="eff55-109">Value</span></span>|<span data-ttu-id="eff55-110">説明</span><span class="sxs-lookup"><span data-stu-id="eff55-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eff55-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="eff55-111">notConfigured</span></span>|<span data-ttu-id="eff55-112">.0</span><span class="sxs-lookup"><span data-stu-id="eff55-112">0</span></span>|<span data-ttu-id="eff55-113">未構成</span><span class="sxs-lookup"><span data-stu-id="eff55-113">Not configured</span></span>|
|<span data-ttu-id="eff55-114">defaultnotifications</span><span class="sxs-lookup"><span data-stu-id="eff55-114">defaultNotifications</span></span>|<span data-ttu-id="eff55-115">1 </span><span class="sxs-lookup"><span data-stu-id="eff55-115">1</span></span>|<span data-ttu-id="eff55-116">既定の Windows Update 通知を使用します。</span><span class="sxs-lookup"><span data-stu-id="eff55-116">Use the default Windows Update notifications.</span></span>|
|<span data-ttu-id="eff55-117">restartWarningsOnly</span><span class="sxs-lookup"><span data-stu-id="eff55-117">restartWarningsOnly</span></span>|<span data-ttu-id="eff55-118">2 </span><span class="sxs-lookup"><span data-stu-id="eff55-118">2</span></span>|<span data-ttu-id="eff55-119">再起動警告を除く、すべての通知をオフにします。</span><span class="sxs-lookup"><span data-stu-id="eff55-119">Turn off all notifications, excluding restart warnings.</span></span>|
|<span data-ttu-id="eff55-120">disableallnotifications</span><span class="sxs-lookup"><span data-stu-id="eff55-120">disableAllNotifications</span></span>|<span data-ttu-id="eff55-121">3 </span><span class="sxs-lookup"><span data-stu-id="eff55-121">3</span></span>|<span data-ttu-id="eff55-122">再起動の警告を含む、すべての通知をオフにします。</span><span class="sxs-lookup"><span data-stu-id="eff55-122">Turn off all notifications, including restart warnings.</span></span>|





