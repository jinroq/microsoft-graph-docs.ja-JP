---
title: 自動 Updatemode 列挙型
description: 自動更新モードで可能な値。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: e8d64f3af656a03bd02ecba5db2fbdab288f3693
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36333885"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="781f4-103">自動 Updatemode 列挙型</span><span class="sxs-lookup"><span data-stu-id="781f4-103">automaticUpdateMode enum type</span></span>

> <span data-ttu-id="781f4-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="781f4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="781f4-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="781f4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="781f4-106">自動更新モードで可能な値。</span><span class="sxs-lookup"><span data-stu-id="781f4-106">Possible values for automatic update mode.</span></span>

## <a name="members"></a><span data-ttu-id="781f4-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="781f4-107">Members</span></span>
|<span data-ttu-id="781f4-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="781f4-108">Member</span></span>|<span data-ttu-id="781f4-109">値</span><span class="sxs-lookup"><span data-stu-id="781f4-109">Value</span></span>|<span data-ttu-id="781f4-110">説明</span><span class="sxs-lookup"><span data-stu-id="781f4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="781f4-111">自分のもの</span><span class="sxs-lookup"><span data-stu-id="781f4-111">userDefined</span></span>|<span data-ttu-id="781f4-112">.0</span><span class="sxs-lookup"><span data-stu-id="781f4-112">0</span></span>|<span data-ttu-id="781f4-113">ユーザー定義、既定値、意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="781f4-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="781f4-114">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="781f4-114">notifyDownload</span></span>|<span data-ttu-id="781f4-115">1-d</span><span class="sxs-lookup"><span data-stu-id="781f4-115">1</span></span>|<span data-ttu-id="781f4-116">ダウンロードを通知します。</span><span class="sxs-lookup"><span data-stu-id="781f4-116">Notify on download.</span></span>|
|<span data-ttu-id="781f4-117">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="781f4-117">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="781f4-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="781f4-118">2</span></span>|<span data-ttu-id="781f4-119">メンテナンス時に自動インストールします。</span><span class="sxs-lookup"><span data-stu-id="781f4-119">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="781f4-120">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="781f4-120">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="781f4-121">1/3</span><span class="sxs-lookup"><span data-stu-id="781f4-121">3</span></span>|<span data-ttu-id="781f4-122">メンテナンス時に自動的にインストールおよび再起動します。</span><span class="sxs-lookup"><span data-stu-id="781f4-122">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="781f4-123">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="781f4-123">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="781f4-124">2/4</span><span class="sxs-lookup"><span data-stu-id="781f4-124">4</span></span>|<span data-ttu-id="781f4-125">スケジュールされた時刻に自動インストールおよび再起動します。</span><span class="sxs-lookup"><span data-stu-id="781f4-125">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="781f4-126">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="781f4-126">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="781f4-127">5</span><span class="sxs-lookup"><span data-stu-id="781f4-127">5</span></span>|<span data-ttu-id="781f4-128">エンドユーザーコントロールを使用せずに自動インストールおよび再起動</span><span class="sxs-lookup"><span data-stu-id="781f4-128">Auto-install and restart without end-user control</span></span>|
|<span data-ttu-id="781f4-129">windowsDefault</span><span class="sxs-lookup"><span data-stu-id="781f4-129">windowsDefault</span></span>|<span data-ttu-id="781f4-130">シックス</span><span class="sxs-lookup"><span data-stu-id="781f4-130">6</span></span>|<span data-ttu-id="781f4-131">Windows の既定値にリセットします。</span><span class="sxs-lookup"><span data-stu-id="781f4-131">Reset to Windows default value.</span></span>|



