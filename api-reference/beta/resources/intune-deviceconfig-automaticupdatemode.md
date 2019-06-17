---
title: 自動 Updatemode 列挙型
description: 自動更新モードで可能な値。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d2fffa3e1b1a5e7efa43d7ce653792247e3ad790
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34983632"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="747c0-103">自動 Updatemode 列挙型</span><span class="sxs-lookup"><span data-stu-id="747c0-103">automaticUpdateMode enum type</span></span>

> <span data-ttu-id="747c0-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="747c0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="747c0-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="747c0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="747c0-106">自動更新モードで可能な値。</span><span class="sxs-lookup"><span data-stu-id="747c0-106">Possible values for automatic update mode.</span></span>

## <a name="members"></a><span data-ttu-id="747c0-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="747c0-107">Members</span></span>
|<span data-ttu-id="747c0-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="747c0-108">Member</span></span>|<span data-ttu-id="747c0-109">値</span><span class="sxs-lookup"><span data-stu-id="747c0-109">Value</span></span>|<span data-ttu-id="747c0-110">説明</span><span class="sxs-lookup"><span data-stu-id="747c0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="747c0-111">自分のもの</span><span class="sxs-lookup"><span data-stu-id="747c0-111">userDefined</span></span>|<span data-ttu-id="747c0-112">.0</span><span class="sxs-lookup"><span data-stu-id="747c0-112">0</span></span>|<span data-ttu-id="747c0-113">ユーザー定義、既定値、意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="747c0-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="747c0-114">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="747c0-114">notifyDownload</span></span>|<span data-ttu-id="747c0-115">1-d</span><span class="sxs-lookup"><span data-stu-id="747c0-115">1</span></span>|<span data-ttu-id="747c0-116">ダウンロードを通知します。</span><span class="sxs-lookup"><span data-stu-id="747c0-116">Notify on download.</span></span>|
|<span data-ttu-id="747c0-117">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="747c0-117">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="747c0-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="747c0-118">2</span></span>|<span data-ttu-id="747c0-119">メンテナンス時に自動インストールします。</span><span class="sxs-lookup"><span data-stu-id="747c0-119">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="747c0-120">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="747c0-120">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="747c0-121">1/3</span><span class="sxs-lookup"><span data-stu-id="747c0-121">3</span></span>|<span data-ttu-id="747c0-122">メンテナンス時に自動的にインストールおよび再起動します。</span><span class="sxs-lookup"><span data-stu-id="747c0-122">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="747c0-123">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="747c0-123">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="747c0-124">2/4</span><span class="sxs-lookup"><span data-stu-id="747c0-124">4</span></span>|<span data-ttu-id="747c0-125">スケジュールされた時刻に自動インストールおよび再起動します。</span><span class="sxs-lookup"><span data-stu-id="747c0-125">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="747c0-126">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="747c0-126">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="747c0-127">5</span><span class="sxs-lookup"><span data-stu-id="747c0-127">5</span></span>|<span data-ttu-id="747c0-128">エンドユーザーコントロールを使用せずに自動インストールおよび再起動</span><span class="sxs-lookup"><span data-stu-id="747c0-128">Auto-install and restart without end-user control</span></span>|
|<span data-ttu-id="747c0-129">windowsDefault</span><span class="sxs-lookup"><span data-stu-id="747c0-129">windowsDefault</span></span>|<span data-ttu-id="747c0-130">シックス</span><span class="sxs-lookup"><span data-stu-id="747c0-130">6</span></span>|<span data-ttu-id="747c0-131">Windows の既定値にリセットします。</span><span class="sxs-lookup"><span data-stu-id="747c0-131">Reset to Windows default value.</span></span>|





