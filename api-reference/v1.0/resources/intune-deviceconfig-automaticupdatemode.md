---
title: 自動 updatemode 列挙型
description: 自動更新モードで可能な値。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7fd45ff85cbab934aa2549f13ee3e6671c65f9ae
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32575178"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="e81a4-103">自動 updatemode 列挙型</span><span class="sxs-lookup"><span data-stu-id="e81a4-103">automaticUpdateMode enum type</span></span>

> <span data-ttu-id="e81a4-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e81a4-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e81a4-105">自動更新モードで可能な値。</span><span class="sxs-lookup"><span data-stu-id="e81a4-105">Possible values for automatic update mode.</span></span>

## <a name="members"></a><span data-ttu-id="e81a4-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="e81a4-106">Members</span></span>
|<span data-ttu-id="e81a4-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="e81a4-107">Member</span></span>|<span data-ttu-id="e81a4-108">値</span><span class="sxs-lookup"><span data-stu-id="e81a4-108">Value</span></span>|<span data-ttu-id="e81a4-109">説明</span><span class="sxs-lookup"><span data-stu-id="e81a4-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e81a4-110">自分のもの</span><span class="sxs-lookup"><span data-stu-id="e81a4-110">userDefined</span></span>|<span data-ttu-id="e81a4-111">.0</span><span class="sxs-lookup"><span data-stu-id="e81a4-111">0</span></span>|<span data-ttu-id="e81a4-112">ユーザー定義、既定値、意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="e81a4-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="e81a4-113">notifydownload</span><span class="sxs-lookup"><span data-stu-id="e81a4-113">notifyDownload</span></span>|<span data-ttu-id="e81a4-114">1 </span><span class="sxs-lookup"><span data-stu-id="e81a4-114">1</span></span>|<span data-ttu-id="e81a4-115">ダウンロードを通知します。</span><span class="sxs-lookup"><span data-stu-id="e81a4-115">Notify on download.</span></span>|
|<span data-ttu-id="e81a4-116">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="e81a4-116">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="e81a4-117">2 </span><span class="sxs-lookup"><span data-stu-id="e81a4-117">2</span></span>|<span data-ttu-id="e81a4-118">メンテナンス時に自動インストールします。</span><span class="sxs-lookup"><span data-stu-id="e81a4-118">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="e81a4-119">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="e81a4-119">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="e81a4-120">3 </span><span class="sxs-lookup"><span data-stu-id="e81a4-120">3</span></span>|<span data-ttu-id="e81a4-121">メンテナンス時に自動的にインストールおよび再起動します。</span><span class="sxs-lookup"><span data-stu-id="e81a4-121">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="e81a4-122">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="e81a4-122">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="e81a4-123">4 </span><span class="sxs-lookup"><span data-stu-id="e81a4-123">4</span></span>|<span data-ttu-id="e81a4-124">スケジュールされた時刻に自動インストールおよび再起動します。</span><span class="sxs-lookup"><span data-stu-id="e81a4-124">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="e81a4-125">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="e81a4-125">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="e81a4-126">5 </span><span class="sxs-lookup"><span data-stu-id="e81a4-126">5</span></span>|<span data-ttu-id="e81a4-127">エンドユーザーコントロールを使用せずに自動インストールおよび再起動</span><span class="sxs-lookup"><span data-stu-id="e81a4-127">Auto-install and restart without end-user control</span></span>|



