---
title: automaticUpdateMode 列挙型
description: 自動更新モードを使用可能な値です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d982c4c9ee524712c212eba1b8b44349d0a70377
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402637"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="ec63a-103">automaticUpdateMode 列挙型</span><span class="sxs-lookup"><span data-stu-id="ec63a-103">automaticUpdateMode enum type</span></span>

> <span data-ttu-id="ec63a-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ec63a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ec63a-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ec63a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ec63a-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ec63a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ec63a-107">自動更新モードを使用可能な値です。</span><span class="sxs-lookup"><span data-stu-id="ec63a-107">Possible values for automatic update mode.</span></span>

## <a name="members"></a><span data-ttu-id="ec63a-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="ec63a-108">Members</span></span>
|<span data-ttu-id="ec63a-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="ec63a-109">Member</span></span>|<span data-ttu-id="ec63a-110">値</span><span class="sxs-lookup"><span data-stu-id="ec63a-110">Value</span></span>|<span data-ttu-id="ec63a-111">説明</span><span class="sxs-lookup"><span data-stu-id="ec63a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec63a-112">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="ec63a-112">userDefined</span></span>|<span data-ttu-id="ec63a-113">0</span><span class="sxs-lookup"><span data-stu-id="ec63a-113">0</span></span>|<span data-ttu-id="ec63a-114">ユーザー定義、既定値、ない目的。</span><span class="sxs-lookup"><span data-stu-id="ec63a-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="ec63a-115">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="ec63a-115">notifyDownload</span></span>|<span data-ttu-id="ec63a-116">1</span><span class="sxs-lookup"><span data-stu-id="ec63a-116">1</span></span>|<span data-ttu-id="ec63a-117">ダウンロード時に通知します。</span><span class="sxs-lookup"><span data-stu-id="ec63a-117">Notify on download.</span></span>|
|<span data-ttu-id="ec63a-118">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="ec63a-118">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="ec63a-119">2</span><span class="sxs-lookup"><span data-stu-id="ec63a-119">2</span></span>|<span data-ttu-id="ec63a-120">メンテナンス時に自動インストールします。</span><span class="sxs-lookup"><span data-stu-id="ec63a-120">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="ec63a-121">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="ec63a-121">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="ec63a-122">3</span><span class="sxs-lookup"><span data-stu-id="ec63a-122">3</span></span>|<span data-ttu-id="ec63a-123">自動インストールおよびメンテナンス時に再起動します。</span><span class="sxs-lookup"><span data-stu-id="ec63a-123">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="ec63a-124">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="ec63a-124">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="ec63a-125">4</span><span class="sxs-lookup"><span data-stu-id="ec63a-125">4</span></span>|<span data-ttu-id="ec63a-126">自動インストールし、スケジュールされた時刻に再起動します。</span><span class="sxs-lookup"><span data-stu-id="ec63a-126">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="ec63a-127">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="ec63a-127">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="ec63a-128">5</span><span class="sxs-lookup"><span data-stu-id="ec63a-128">5</span></span>|<span data-ttu-id="ec63a-129">自動インストールし、エンドユーザーの制御に再起動します</span><span class="sxs-lookup"><span data-stu-id="ec63a-129">Auto-install and restart without end-user control</span></span>|
|<span data-ttu-id="ec63a-130">windowsDefault</span><span class="sxs-lookup"><span data-stu-id="ec63a-130">windowsDefault</span></span>|<span data-ttu-id="ec63a-131">6</span><span class="sxs-lookup"><span data-stu-id="ec63a-131">6</span></span>|<span data-ttu-id="ec63a-132">Windows の既定値にリセットされます。</span><span class="sxs-lookup"><span data-stu-id="ec63a-132">Reset to Windows default value.</span></span>|




