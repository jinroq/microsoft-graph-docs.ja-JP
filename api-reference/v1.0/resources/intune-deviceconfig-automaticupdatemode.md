---
title: 自動 Updatemode 列挙型
description: 自動更新モードで可能な値。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 3a0cc2d3918573fca6480c6eecd07889534cda4b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028575"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="b7ab6-103">自動 Updatemode 列挙型</span><span class="sxs-lookup"><span data-stu-id="b7ab6-103">automaticUpdateMode enum type</span></span>

> <span data-ttu-id="b7ab6-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b7ab6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7ab6-105">自動更新モードで可能な値。</span><span class="sxs-lookup"><span data-stu-id="b7ab6-105">Possible values for automatic update mode.</span></span>

## <a name="members"></a><span data-ttu-id="b7ab6-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="b7ab6-106">Members</span></span>
|<span data-ttu-id="b7ab6-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="b7ab6-107">Member</span></span>|<span data-ttu-id="b7ab6-108">値</span><span class="sxs-lookup"><span data-stu-id="b7ab6-108">Value</span></span>|<span data-ttu-id="b7ab6-109">説明</span><span class="sxs-lookup"><span data-stu-id="b7ab6-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7ab6-110">自分のもの</span><span class="sxs-lookup"><span data-stu-id="b7ab6-110">userDefined</span></span>|<span data-ttu-id="b7ab6-111">.0</span><span class="sxs-lookup"><span data-stu-id="b7ab6-111">0</span></span>|<span data-ttu-id="b7ab6-112">ユーザー定義、既定値、意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="b7ab6-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="b7ab6-113">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="b7ab6-113">notifyDownload</span></span>|<span data-ttu-id="b7ab6-114">1-d</span><span class="sxs-lookup"><span data-stu-id="b7ab6-114">1</span></span>|<span data-ttu-id="b7ab6-115">ダウンロードを通知します。</span><span class="sxs-lookup"><span data-stu-id="b7ab6-115">Notify on download.</span></span>|
|<span data-ttu-id="b7ab6-116">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="b7ab6-116">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="b7ab6-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="b7ab6-117">2</span></span>|<span data-ttu-id="b7ab6-118">メンテナンス時に自動インストールします。</span><span class="sxs-lookup"><span data-stu-id="b7ab6-118">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="b7ab6-119">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="b7ab6-119">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="b7ab6-120">1/3</span><span class="sxs-lookup"><span data-stu-id="b7ab6-120">3</span></span>|<span data-ttu-id="b7ab6-121">メンテナンス時に自動的にインストールおよび再起動します。</span><span class="sxs-lookup"><span data-stu-id="b7ab6-121">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="b7ab6-122">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="b7ab6-122">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="b7ab6-123">2/4</span><span class="sxs-lookup"><span data-stu-id="b7ab6-123">4</span></span>|<span data-ttu-id="b7ab6-124">スケジュールされた時刻に自動インストールおよび再起動します。</span><span class="sxs-lookup"><span data-stu-id="b7ab6-124">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="b7ab6-125">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="b7ab6-125">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="b7ab6-126">5</span><span class="sxs-lookup"><span data-stu-id="b7ab6-126">5</span></span>|<span data-ttu-id="b7ab6-127">エンドユーザーコントロールを使用せずに自動インストールおよび再起動</span><span class="sxs-lookup"><span data-stu-id="b7ab6-127">Auto-install and restart without end-user control</span></span>|



