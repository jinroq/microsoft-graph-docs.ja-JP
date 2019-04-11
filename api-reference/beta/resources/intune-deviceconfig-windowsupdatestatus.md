---
title: windowsUpdateStatus 列挙型
description: ビジネス構成デバイスの状態に関する Windows update
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 73cd3208b7729544d6fbd620a13ce295b39aff26
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31780183"
---
# <a name="windowsupdatestatus-enum-type"></a><span data-ttu-id="db9f7-103">windowsUpdateStatus 列挙型</span><span class="sxs-lookup"><span data-stu-id="db9f7-103">windowsUpdateStatus enum type</span></span>

> <span data-ttu-id="db9f7-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="db9f7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="db9f7-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="db9f7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db9f7-106">ビジネス構成デバイスの状態に関する Windows update</span><span class="sxs-lookup"><span data-stu-id="db9f7-106">Windows update for business configuration device states</span></span>

## <a name="members"></a><span data-ttu-id="db9f7-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="db9f7-107">Members</span></span>
|<span data-ttu-id="db9f7-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="db9f7-108">Member</span></span>|<span data-ttu-id="db9f7-109">値</span><span class="sxs-lookup"><span data-stu-id="db9f7-109">Value</span></span>|<span data-ttu-id="db9f7-110">説明</span><span class="sxs-lookup"><span data-stu-id="db9f7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db9f7-111">upToDate</span><span class="sxs-lookup"><span data-stu-id="db9f7-111">upToDate</span></span>|<span data-ttu-id="db9f7-112">.0</span><span class="sxs-lookup"><span data-stu-id="db9f7-112">0</span></span>|<span data-ttu-id="db9f7-113">保留中の更新はありません。保留中の再起動更新プログラムはありません。更新は失敗しています。</span><span class="sxs-lookup"><span data-stu-id="db9f7-113">There are no pending updates, no pending reboot updates and no failed updates.</span></span>|
|<span data-ttu-id="db9f7-114">pendinginstallation</span><span class="sxs-lookup"><span data-stu-id="db9f7-114">pendingInstallation</span></span>|<span data-ttu-id="db9f7-115">1-d</span><span class="sxs-lookup"><span data-stu-id="db9f7-115">1</span></span>|<span data-ttu-id="db9f7-116">承認されていない更新プログラムが含まれている保留中の更新プログラムがあります。</span><span class="sxs-lookup"><span data-stu-id="db9f7-116">There are updates that’s pending installation which includes updates that are not approved.</span></span> <span data-ttu-id="db9f7-117">保留中の再起動更新はありません。更新は失敗しません。</span><span class="sxs-lookup"><span data-stu-id="db9f7-117">There are no Pending reboot updates, no failed updates.</span></span>|
|<span data-ttu-id="db9f7-118">pendingreboot</span><span class="sxs-lookup"><span data-stu-id="db9f7-118">pendingReboot</span></span>|<span data-ttu-id="db9f7-119">pbm-2</span><span class="sxs-lookup"><span data-stu-id="db9f7-119">2</span></span>|<span data-ttu-id="db9f7-120">再起動が必要な更新プログラムがあります。</span><span class="sxs-lookup"><span data-stu-id="db9f7-120">There are updates that requires reboot.</span></span> <span data-ttu-id="db9f7-121">失敗した更新はありません。</span><span class="sxs-lookup"><span data-stu-id="db9f7-121">There are not failed updates.</span></span>|
|<span data-ttu-id="db9f7-122">フェール</span><span class="sxs-lookup"><span data-stu-id="db9f7-122">failed</span></span>|<span data-ttu-id="db9f7-123">1/3</span><span class="sxs-lookup"><span data-stu-id="db9f7-123">3</span></span>|<span data-ttu-id="db9f7-124">デバイスにインストールできなかった更新プログラムがあります。</span><span class="sxs-lookup"><span data-stu-id="db9f7-124">There are updates failed to install on the device.</span></span>|





