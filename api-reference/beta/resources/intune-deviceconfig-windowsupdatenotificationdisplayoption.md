---
title: windowsUpdateNotificationDisplayOption 列挙型
description: Windows Update 通知の表示オプション
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 69c990e8cb2eefc71e1a0cae085e71da7e095383
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36337672"
---
# <a name="windowsupdatenotificationdisplayoption-enum-type"></a><span data-ttu-id="efa3f-103">windowsUpdateNotificationDisplayOption 列挙型</span><span class="sxs-lookup"><span data-stu-id="efa3f-103">windowsUpdateNotificationDisplayOption enum type</span></span>

> <span data-ttu-id="efa3f-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="efa3f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="efa3f-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="efa3f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="efa3f-106">Windows Update 通知の表示オプション</span><span class="sxs-lookup"><span data-stu-id="efa3f-106">Windows Update Notification Display Options</span></span>

## <a name="members"></a><span data-ttu-id="efa3f-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="efa3f-107">Members</span></span>
|<span data-ttu-id="efa3f-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="efa3f-108">Member</span></span>|<span data-ttu-id="efa3f-109">値</span><span class="sxs-lookup"><span data-stu-id="efa3f-109">Value</span></span>|<span data-ttu-id="efa3f-110">説明</span><span class="sxs-lookup"><span data-stu-id="efa3f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="efa3f-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="efa3f-111">notConfigured</span></span>|<span data-ttu-id="efa3f-112">.0</span><span class="sxs-lookup"><span data-stu-id="efa3f-112">0</span></span>|<span data-ttu-id="efa3f-113">未構成</span><span class="sxs-lookup"><span data-stu-id="efa3f-113">Not configured</span></span>|
|<span data-ttu-id="efa3f-114">defaultNotifications</span><span class="sxs-lookup"><span data-stu-id="efa3f-114">defaultNotifications</span></span>|<span data-ttu-id="efa3f-115">1-d</span><span class="sxs-lookup"><span data-stu-id="efa3f-115">1</span></span>|<span data-ttu-id="efa3f-116">既定の Windows Update 通知を使用します。</span><span class="sxs-lookup"><span data-stu-id="efa3f-116">Use the default Windows Update notifications.</span></span>|
|<span data-ttu-id="efa3f-117">restartWarningsOnly</span><span class="sxs-lookup"><span data-stu-id="efa3f-117">restartWarningsOnly</span></span>|<span data-ttu-id="efa3f-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="efa3f-118">2</span></span>|<span data-ttu-id="efa3f-119">再起動警告を除く、すべての通知をオフにします。</span><span class="sxs-lookup"><span data-stu-id="efa3f-119">Turn off all notifications, excluding restart warnings.</span></span>|
|<span data-ttu-id="efa3f-120">disableAllNotifications</span><span class="sxs-lookup"><span data-stu-id="efa3f-120">disableAllNotifications</span></span>|<span data-ttu-id="efa3f-121">1/3</span><span class="sxs-lookup"><span data-stu-id="efa3f-121">3</span></span>|<span data-ttu-id="efa3f-122">再起動の警告を含む、すべての通知をオフにします。</span><span class="sxs-lookup"><span data-stu-id="efa3f-122">Turn off all notifications, including restart warnings.</span></span>|



