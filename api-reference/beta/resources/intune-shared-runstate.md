---
title: runstate 列挙型
description: デバイス管理スクリプトの実行状態の種類を示します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 706ef0d5ea87796c951d2fcb8c7357643fba7afb
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30146775"
---
# <a name="runstate-enum-type"></a><span data-ttu-id="db611-103">runstate 列挙型</span><span class="sxs-lookup"><span data-stu-id="db611-103">runState enum type</span></span>

> <span data-ttu-id="db611-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="db611-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="db611-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="db611-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db611-106">デバイス管理スクリプトの実行状態の種類を示します。</span><span class="sxs-lookup"><span data-stu-id="db611-106">Indicates the type of execution status of the device management script.</span></span>

## <a name="members"></a><span data-ttu-id="db611-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="db611-107">Members</span></span>
|<span data-ttu-id="db611-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="db611-108">Member</span></span>|<span data-ttu-id="db611-109">値</span><span class="sxs-lookup"><span data-stu-id="db611-109">Value</span></span>|<span data-ttu-id="db611-110">説明</span><span class="sxs-lookup"><span data-stu-id="db611-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db611-111">不明</span><span class="sxs-lookup"><span data-stu-id="db611-111">unknown</span></span>|<span data-ttu-id="db611-112">.0</span><span class="sxs-lookup"><span data-stu-id="db611-112">0</span></span>|<span data-ttu-id="db611-113">不明な結果です。</span><span class="sxs-lookup"><span data-stu-id="db611-113">Unknown result.</span></span>|
|<span data-ttu-id="db611-114">success</span><span class="sxs-lookup"><span data-stu-id="db611-114">success</span></span>|<span data-ttu-id="db611-115">1-d</span><span class="sxs-lookup"><span data-stu-id="db611-115">1</span></span>|<span data-ttu-id="db611-116">スクリプトは正常に実行されます。</span><span class="sxs-lookup"><span data-stu-id="db611-116">Script is run successfully.</span></span>|
|<span data-ttu-id="db611-117">失敗</span><span class="sxs-lookup"><span data-stu-id="db611-117">fail</span></span>|<span data-ttu-id="db611-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="db611-118">2</span></span>|<span data-ttu-id="db611-119">スクリプトの実行に失敗しました。</span><span class="sxs-lookup"><span data-stu-id="db611-119">Script failed to run.</span></span>|




