---
title: windowsSModeConfiguration 列挙型
description: S モードのロック解除を構成するために使用可能なオプション
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 467879cf7992a60203164d5db6f7e657a77f87d4
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943817"
---
# <a name="windowssmodeconfiguration-enum-type"></a><span data-ttu-id="659db-103">windowsSModeConfiguration 列挙型</span><span class="sxs-lookup"><span data-stu-id="659db-103">windowsSModeConfiguration enum type</span></span>

> <span data-ttu-id="659db-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="659db-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="659db-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="659db-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="659db-106">S モードのロック解除を構成するために使用可能なオプション</span><span class="sxs-lookup"><span data-stu-id="659db-106">The possible options to configure S mode unlock</span></span>

## <a name="members"></a><span data-ttu-id="659db-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="659db-107">Members</span></span>
|<span data-ttu-id="659db-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="659db-108">Member</span></span>|<span data-ttu-id="659db-109">値</span><span class="sxs-lookup"><span data-stu-id="659db-109">Value</span></span>|<span data-ttu-id="659db-110">説明</span><span class="sxs-lookup"><span data-stu-id="659db-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="659db-111">noRestriction</span><span class="sxs-lookup"><span data-stu-id="659db-111">noRestriction</span></span>|<span data-ttu-id="659db-112">.0</span><span class="sxs-lookup"><span data-stu-id="659db-112">0</span></span>|<span data-ttu-id="659db-113">このオプションを選択すると、ロックを解除するためのすべての制限が削除されます-既定値</span><span class="sxs-lookup"><span data-stu-id="659db-113">This option will remove all restrictions to unlock S mode - default</span></span>|
|<span data-ttu-id="659db-114">拒否</span><span class="sxs-lookup"><span data-stu-id="659db-114">block</span></span>|<span data-ttu-id="659db-115">1-d</span><span class="sxs-lookup"><span data-stu-id="659db-115">1</span></span>|<span data-ttu-id="659db-116">このオプションは、ユーザーが S モードからデバイスのロックを解除するのをブロックします。</span><span class="sxs-lookup"><span data-stu-id="659db-116">This option will block the user to unlock the device from S mode</span></span>|
|<span data-ttu-id="659db-117">外す</span><span class="sxs-lookup"><span data-stu-id="659db-117">unlock</span></span>|<span data-ttu-id="659db-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="659db-118">2</span></span>|<span data-ttu-id="659db-119">このオプションでは、デバイスを S モードからロック解除します。</span><span class="sxs-lookup"><span data-stu-id="659db-119">This option will unlock the device from S mode</span></span>|




