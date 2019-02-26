---
title: 自動 updatemode 列挙型
description: 自動更新モードで可能な値。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7fd45ff85cbab934aa2549f13ee3e6671c65f9ae
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251378"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="c99c2-103">自動 updatemode 列挙型</span><span class="sxs-lookup"><span data-stu-id="c99c2-103">automaticUpdateMode enum type</span></span>

> <span data-ttu-id="c99c2-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c99c2-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c99c2-105">自動更新モードで可能な値。</span><span class="sxs-lookup"><span data-stu-id="c99c2-105">Possible values for automatic update mode.</span></span>

## <a name="members"></a><span data-ttu-id="c99c2-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="c99c2-106">Members</span></span>
|<span data-ttu-id="c99c2-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="c99c2-107">Member</span></span>|<span data-ttu-id="c99c2-108">値</span><span class="sxs-lookup"><span data-stu-id="c99c2-108">Value</span></span>|<span data-ttu-id="c99c2-109">説明</span><span class="sxs-lookup"><span data-stu-id="c99c2-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c99c2-110">自分のもの</span><span class="sxs-lookup"><span data-stu-id="c99c2-110">userDefined</span></span>|<span data-ttu-id="c99c2-111">.0</span><span class="sxs-lookup"><span data-stu-id="c99c2-111">0</span></span>|<span data-ttu-id="c99c2-112">ユーザー定義、既定値、意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="c99c2-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="c99c2-113">notifydownload</span><span class="sxs-lookup"><span data-stu-id="c99c2-113">notifyDownload</span></span>|<span data-ttu-id="c99c2-114">1-d</span><span class="sxs-lookup"><span data-stu-id="c99c2-114">1</span></span>|<span data-ttu-id="c99c2-115">ダウンロードを通知します。</span><span class="sxs-lookup"><span data-stu-id="c99c2-115">Notify on download.</span></span>|
|<span data-ttu-id="c99c2-116">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="c99c2-116">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="c99c2-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="c99c2-117">2</span></span>|<span data-ttu-id="c99c2-118">メンテナンス時に自動インストールします。</span><span class="sxs-lookup"><span data-stu-id="c99c2-118">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="c99c2-119">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="c99c2-119">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="c99c2-120">1/3</span><span class="sxs-lookup"><span data-stu-id="c99c2-120">3</span></span>|<span data-ttu-id="c99c2-121">メンテナンス時に自動的にインストールおよび再起動します。</span><span class="sxs-lookup"><span data-stu-id="c99c2-121">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="c99c2-122">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="c99c2-122">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="c99c2-123">2/4</span><span class="sxs-lookup"><span data-stu-id="c99c2-123">4</span></span>|<span data-ttu-id="c99c2-124">スケジュールされた時刻に自動インストールおよび再起動します。</span><span class="sxs-lookup"><span data-stu-id="c99c2-124">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="c99c2-125">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="c99c2-125">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="c99c2-126">5</span><span class="sxs-lookup"><span data-stu-id="c99c2-126">5</span></span>|<span data-ttu-id="c99c2-127">エンドユーザーコントロールを使用せずに自動インストールおよび再起動</span><span class="sxs-lookup"><span data-stu-id="c99c2-127">Auto-install and restart without end-user control</span></span>|



