---
title: windowsUpdateNotificationDisplayOption 列挙型
description: Windows Update 通知の表示オプション
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b11c793d2ef294bf9026de9f1869cdea28babfab
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943635"
---
# <a name="windowsupdatenotificationdisplayoption-enum-type"></a><span data-ttu-id="f0722-103">windowsUpdateNotificationDisplayOption 列挙型</span><span class="sxs-lookup"><span data-stu-id="f0722-103">windowsUpdateNotificationDisplayOption enum type</span></span>

> <span data-ttu-id="f0722-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f0722-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f0722-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f0722-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0722-106">Windows Update 通知の表示オプション</span><span class="sxs-lookup"><span data-stu-id="f0722-106">Windows Update Notification Display Options</span></span>

## <a name="members"></a><span data-ttu-id="f0722-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="f0722-107">Members</span></span>
|<span data-ttu-id="f0722-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="f0722-108">Member</span></span>|<span data-ttu-id="f0722-109">値</span><span class="sxs-lookup"><span data-stu-id="f0722-109">Value</span></span>|<span data-ttu-id="f0722-110">説明</span><span class="sxs-lookup"><span data-stu-id="f0722-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0722-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="f0722-111">notConfigured</span></span>|<span data-ttu-id="f0722-112">.0</span><span class="sxs-lookup"><span data-stu-id="f0722-112">0</span></span>|<span data-ttu-id="f0722-113">未構成</span><span class="sxs-lookup"><span data-stu-id="f0722-113">Not configured</span></span>|
|<span data-ttu-id="f0722-114">defaultNotifications</span><span class="sxs-lookup"><span data-stu-id="f0722-114">defaultNotifications</span></span>|<span data-ttu-id="f0722-115">1-d</span><span class="sxs-lookup"><span data-stu-id="f0722-115">1</span></span>|<span data-ttu-id="f0722-116">既定の Windows Update 通知を使用します。</span><span class="sxs-lookup"><span data-stu-id="f0722-116">Use the default Windows Update notifications.</span></span>|
|<span data-ttu-id="f0722-117">restartWarningsOnly</span><span class="sxs-lookup"><span data-stu-id="f0722-117">restartWarningsOnly</span></span>|<span data-ttu-id="f0722-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="f0722-118">2</span></span>|<span data-ttu-id="f0722-119">再起動警告を除く、すべての通知をオフにします。</span><span class="sxs-lookup"><span data-stu-id="f0722-119">Turn off all notifications, excluding restart warnings.</span></span>|
|<span data-ttu-id="f0722-120">disableAllNotifications</span><span class="sxs-lookup"><span data-stu-id="f0722-120">disableAllNotifications</span></span>|<span data-ttu-id="f0722-121">1/3</span><span class="sxs-lookup"><span data-stu-id="f0722-121">3</span></span>|<span data-ttu-id="f0722-122">再起動の警告を含む、すべての通知をオフにします。</span><span class="sxs-lookup"><span data-stu-id="f0722-122">Turn off all notifications, including restart warnings.</span></span>|




