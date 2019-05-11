---
title: windowsUpdateStatus 列挙型
description: ビジネス構成デバイスの状態に関する Windows update
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c6eecee6626e4d47856071de3ebb53944e196478
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943642"
---
# <a name="windowsupdatestatus-enum-type"></a><span data-ttu-id="efdc6-103">windowsUpdateStatus 列挙型</span><span class="sxs-lookup"><span data-stu-id="efdc6-103">windowsUpdateStatus enum type</span></span>

> <span data-ttu-id="efdc6-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="efdc6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="efdc6-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="efdc6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="efdc6-106">ビジネス構成デバイスの状態に関する Windows update</span><span class="sxs-lookup"><span data-stu-id="efdc6-106">Windows update for business configuration device states</span></span>

## <a name="members"></a><span data-ttu-id="efdc6-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="efdc6-107">Members</span></span>
|<span data-ttu-id="efdc6-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="efdc6-108">Member</span></span>|<span data-ttu-id="efdc6-109">値</span><span class="sxs-lookup"><span data-stu-id="efdc6-109">Value</span></span>|<span data-ttu-id="efdc6-110">説明</span><span class="sxs-lookup"><span data-stu-id="efdc6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="efdc6-111">upToDate</span><span class="sxs-lookup"><span data-stu-id="efdc6-111">upToDate</span></span>|<span data-ttu-id="efdc6-112">.0</span><span class="sxs-lookup"><span data-stu-id="efdc6-112">0</span></span>|<span data-ttu-id="efdc6-113">保留中の更新はありません。保留中の再起動更新プログラムはありません。更新は失敗しています。</span><span class="sxs-lookup"><span data-stu-id="efdc6-113">There are no pending updates, no pending reboot updates and no failed updates.</span></span>|
|<span data-ttu-id="efdc6-114">pendingInstallation</span><span class="sxs-lookup"><span data-stu-id="efdc6-114">pendingInstallation</span></span>|<span data-ttu-id="efdc6-115">1-d</span><span class="sxs-lookup"><span data-stu-id="efdc6-115">1</span></span>|<span data-ttu-id="efdc6-116">承認されていない更新プログラムが含まれている保留中の更新プログラムがあります。</span><span class="sxs-lookup"><span data-stu-id="efdc6-116">There are updates that’s pending installation which includes updates that are not approved.</span></span> <span data-ttu-id="efdc6-117">保留中の再起動更新はありません。更新は失敗しません。</span><span class="sxs-lookup"><span data-stu-id="efdc6-117">There are no Pending reboot updates, no failed updates.</span></span>|
|<span data-ttu-id="efdc6-118">pendingReboot</span><span class="sxs-lookup"><span data-stu-id="efdc6-118">pendingReboot</span></span>|<span data-ttu-id="efdc6-119">pbm-2</span><span class="sxs-lookup"><span data-stu-id="efdc6-119">2</span></span>|<span data-ttu-id="efdc6-120">再起動が必要な更新プログラムがあります。</span><span class="sxs-lookup"><span data-stu-id="efdc6-120">There are updates that requires reboot.</span></span> <span data-ttu-id="efdc6-121">失敗した更新はありません。</span><span class="sxs-lookup"><span data-stu-id="efdc6-121">There are not failed updates.</span></span>|
|<span data-ttu-id="efdc6-122">フェール</span><span class="sxs-lookup"><span data-stu-id="efdc6-122">failed</span></span>|<span data-ttu-id="efdc6-123">1/3</span><span class="sxs-lookup"><span data-stu-id="efdc6-123">3</span></span>|<span data-ttu-id="efdc6-124">デバイスにインストールできなかった更新プログラムがあります。</span><span class="sxs-lookup"><span data-stu-id="efdc6-124">There are updates failed to install on the device.</span></span>|




