---
title: 自動 updatemode 列挙型
description: 自動更新モードで可能な値。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9af00bda442c1a152820323fc0b7e1ddfcd8c384
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549341"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="6eed1-103">自動 updatemode 列挙型</span><span class="sxs-lookup"><span data-stu-id="6eed1-103">automaticUpdateMode enum type</span></span>

> <span data-ttu-id="6eed1-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6eed1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6eed1-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6eed1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6eed1-106">自動更新モードで可能な値。</span><span class="sxs-lookup"><span data-stu-id="6eed1-106">Possible values for automatic update mode.</span></span>

## <a name="members"></a><span data-ttu-id="6eed1-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="6eed1-107">Members</span></span>
|<span data-ttu-id="6eed1-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="6eed1-108">Member</span></span>|<span data-ttu-id="6eed1-109">値</span><span class="sxs-lookup"><span data-stu-id="6eed1-109">Value</span></span>|<span data-ttu-id="6eed1-110">説明</span><span class="sxs-lookup"><span data-stu-id="6eed1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6eed1-111">自分のもの</span><span class="sxs-lookup"><span data-stu-id="6eed1-111">userDefined</span></span>|<span data-ttu-id="6eed1-112">.0</span><span class="sxs-lookup"><span data-stu-id="6eed1-112">0</span></span>|<span data-ttu-id="6eed1-113">ユーザー定義、既定値、意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="6eed1-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="6eed1-114">notifydownload</span><span class="sxs-lookup"><span data-stu-id="6eed1-114">notifyDownload</span></span>|<span data-ttu-id="6eed1-115">1 </span><span class="sxs-lookup"><span data-stu-id="6eed1-115">1</span></span>|<span data-ttu-id="6eed1-116">ダウンロードを通知します。</span><span class="sxs-lookup"><span data-stu-id="6eed1-116">Notify on download.</span></span>|
|<span data-ttu-id="6eed1-117">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="6eed1-117">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="6eed1-118">2 </span><span class="sxs-lookup"><span data-stu-id="6eed1-118">2</span></span>|<span data-ttu-id="6eed1-119">メンテナンス時に自動インストールします。</span><span class="sxs-lookup"><span data-stu-id="6eed1-119">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="6eed1-120">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="6eed1-120">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="6eed1-121">3 </span><span class="sxs-lookup"><span data-stu-id="6eed1-121">3</span></span>|<span data-ttu-id="6eed1-122">メンテナンス時に自動的にインストールおよび再起動します。</span><span class="sxs-lookup"><span data-stu-id="6eed1-122">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="6eed1-123">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="6eed1-123">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="6eed1-124">4 </span><span class="sxs-lookup"><span data-stu-id="6eed1-124">4</span></span>|<span data-ttu-id="6eed1-125">スケジュールされた時刻に自動インストールおよび再起動します。</span><span class="sxs-lookup"><span data-stu-id="6eed1-125">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="6eed1-126">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="6eed1-126">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="6eed1-127">5 </span><span class="sxs-lookup"><span data-stu-id="6eed1-127">5</span></span>|<span data-ttu-id="6eed1-128">エンドユーザーコントロールを使用せずに自動インストールおよび再起動</span><span class="sxs-lookup"><span data-stu-id="6eed1-128">Auto-install and restart without end-user control</span></span>|
|<span data-ttu-id="6eed1-129">windowsdefault</span><span class="sxs-lookup"><span data-stu-id="6eed1-129">windowsDefault</span></span>|<span data-ttu-id="6eed1-130">6 </span><span class="sxs-lookup"><span data-stu-id="6eed1-130">6</span></span>|<span data-ttu-id="6eed1-131">Windows の既定値にリセットします。</span><span class="sxs-lookup"><span data-stu-id="6eed1-131">Reset to Windows default value.</span></span>|





