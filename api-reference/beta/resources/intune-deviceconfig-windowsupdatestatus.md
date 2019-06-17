---
title: windowsUpdateStatus 列挙型
description: ビジネス構成デバイスの状態に関する Windows update
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8ace0b42b09093ce2e9d485271ec607ffd618c9e
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34978690"
---
# <a name="windowsupdatestatus-enum-type"></a><span data-ttu-id="f0a0a-103">windowsUpdateStatus 列挙型</span><span class="sxs-lookup"><span data-stu-id="f0a0a-103">windowsUpdateStatus enum type</span></span>

> <span data-ttu-id="f0a0a-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f0a0a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f0a0a-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f0a0a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0a0a-106">ビジネス構成デバイスの状態に関する Windows update</span><span class="sxs-lookup"><span data-stu-id="f0a0a-106">Windows update for business configuration device states</span></span>

## <a name="members"></a><span data-ttu-id="f0a0a-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="f0a0a-107">Members</span></span>
|<span data-ttu-id="f0a0a-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="f0a0a-108">Member</span></span>|<span data-ttu-id="f0a0a-109">値</span><span class="sxs-lookup"><span data-stu-id="f0a0a-109">Value</span></span>|<span data-ttu-id="f0a0a-110">説明</span><span class="sxs-lookup"><span data-stu-id="f0a0a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0a0a-111">upToDate</span><span class="sxs-lookup"><span data-stu-id="f0a0a-111">upToDate</span></span>|<span data-ttu-id="f0a0a-112">.0</span><span class="sxs-lookup"><span data-stu-id="f0a0a-112">0</span></span>|<span data-ttu-id="f0a0a-113">保留中の更新はありません。保留中の再起動更新プログラムはありません。更新は失敗しています。</span><span class="sxs-lookup"><span data-stu-id="f0a0a-113">There are no pending updates, no pending reboot updates and no failed updates.</span></span>|
|<span data-ttu-id="f0a0a-114">pendingInstallation</span><span class="sxs-lookup"><span data-stu-id="f0a0a-114">pendingInstallation</span></span>|<span data-ttu-id="f0a0a-115">1-d</span><span class="sxs-lookup"><span data-stu-id="f0a0a-115">1</span></span>|<span data-ttu-id="f0a0a-116">承認されていない更新プログラムが含まれている保留中の更新プログラムがあります。</span><span class="sxs-lookup"><span data-stu-id="f0a0a-116">There are updates that’s pending installation which includes updates that are not approved.</span></span> <span data-ttu-id="f0a0a-117">保留中の再起動更新はありません。更新は失敗しません。</span><span class="sxs-lookup"><span data-stu-id="f0a0a-117">There are no Pending reboot updates, no failed updates.</span></span>|
|<span data-ttu-id="f0a0a-118">pendingReboot</span><span class="sxs-lookup"><span data-stu-id="f0a0a-118">pendingReboot</span></span>|<span data-ttu-id="f0a0a-119">pbm-2</span><span class="sxs-lookup"><span data-stu-id="f0a0a-119">2</span></span>|<span data-ttu-id="f0a0a-120">再起動が必要な更新プログラムがあります。</span><span class="sxs-lookup"><span data-stu-id="f0a0a-120">There are updates that requires reboot.</span></span> <span data-ttu-id="f0a0a-121">失敗した更新はありません。</span><span class="sxs-lookup"><span data-stu-id="f0a0a-121">There are not failed updates.</span></span>|
|<span data-ttu-id="f0a0a-122">フェール</span><span class="sxs-lookup"><span data-stu-id="f0a0a-122">failed</span></span>|<span data-ttu-id="f0a0a-123">1/3</span><span class="sxs-lookup"><span data-stu-id="f0a0a-123">3</span></span>|<span data-ttu-id="f0a0a-124">デバイスにインストールできなかった更新プログラムがあります。</span><span class="sxs-lookup"><span data-stu-id="f0a0a-124">There are updates failed to install on the device.</span></span>|





