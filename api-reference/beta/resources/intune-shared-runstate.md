---
title: runState 列挙型
description: デバイス管理スクリプトの実行状態の種類を示します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 093af5b16854bf65699e469b1afd47fe6b990375
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33939841"
---
# <a name="runstate-enum-type"></a><span data-ttu-id="b78a7-103">runState 列挙型</span><span class="sxs-lookup"><span data-stu-id="b78a7-103">runState enum type</span></span>

> <span data-ttu-id="b78a7-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b78a7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b78a7-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b78a7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b78a7-106">デバイス管理スクリプトの実行状態の種類を示します。</span><span class="sxs-lookup"><span data-stu-id="b78a7-106">Indicates the type of execution status of the device management script.</span></span>

## <a name="members"></a><span data-ttu-id="b78a7-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="b78a7-107">Members</span></span>
|<span data-ttu-id="b78a7-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="b78a7-108">Member</span></span>|<span data-ttu-id="b78a7-109">値</span><span class="sxs-lookup"><span data-stu-id="b78a7-109">Value</span></span>|<span data-ttu-id="b78a7-110">説明</span><span class="sxs-lookup"><span data-stu-id="b78a7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b78a7-111">不明</span><span class="sxs-lookup"><span data-stu-id="b78a7-111">unknown</span></span>|<span data-ttu-id="b78a7-112">.0</span><span class="sxs-lookup"><span data-stu-id="b78a7-112">0</span></span>|<span data-ttu-id="b78a7-113">不明な結果です。</span><span class="sxs-lookup"><span data-stu-id="b78a7-113">Unknown result.</span></span>|
|<span data-ttu-id="b78a7-114">success</span><span class="sxs-lookup"><span data-stu-id="b78a7-114">success</span></span>|<span data-ttu-id="b78a7-115">1-d</span><span class="sxs-lookup"><span data-stu-id="b78a7-115">1</span></span>|<span data-ttu-id="b78a7-116">スクリプトは正常に実行されます。</span><span class="sxs-lookup"><span data-stu-id="b78a7-116">Script is run successfully.</span></span>|
|<span data-ttu-id="b78a7-117">fail</span><span class="sxs-lookup"><span data-stu-id="b78a7-117">fail</span></span>|<span data-ttu-id="b78a7-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="b78a7-118">2</span></span>|<span data-ttu-id="b78a7-119">スクリプトの実行に失敗しました。</span><span class="sxs-lookup"><span data-stu-id="b78a7-119">Script failed to run.</span></span>|




