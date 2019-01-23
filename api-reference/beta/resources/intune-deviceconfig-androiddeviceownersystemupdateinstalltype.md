---
title: androidDeviceOwnerSystemUpdateInstallType 列挙型
description: Android デバイスの所有者のシステム更新プログラムの種類。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8d7caaa3c79062bba6b8aa06ea11389e1370fba5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419178"
---
# <a name="androiddeviceownersystemupdateinstalltype-enum-type"></a><span data-ttu-id="a2696-103">androidDeviceOwnerSystemUpdateInstallType 列挙型</span><span class="sxs-lookup"><span data-stu-id="a2696-103">androidDeviceOwnerSystemUpdateInstallType enum type</span></span>

> <span data-ttu-id="a2696-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a2696-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a2696-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a2696-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a2696-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a2696-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2696-107">Android デバイスの所有者のシステム更新プログラムの種類。</span><span class="sxs-lookup"><span data-stu-id="a2696-107">System Update Types for Android Device Owner.</span></span>

## <a name="members"></a><span data-ttu-id="a2696-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="a2696-108">Members</span></span>
|<span data-ttu-id="a2696-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="a2696-109">Member</span></span>|<span data-ttu-id="a2696-110">値</span><span class="sxs-lookup"><span data-stu-id="a2696-110">Value</span></span>|<span data-ttu-id="a2696-111">説明</span><span class="sxs-lookup"><span data-stu-id="a2696-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2696-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="a2696-112">deviceDefault</span></span>|<span data-ttu-id="a2696-113">0</span><span class="sxs-lookup"><span data-stu-id="a2696-113">0</span></span>|<span data-ttu-id="a2696-114">デバイス既定の動作、通常システムの更新を許可するユーザーを求められます。</span><span class="sxs-lookup"><span data-stu-id="a2696-114">Device default behavior, which typically prompts the user to accept system updates.</span></span>|
|<span data-ttu-id="a2696-115">延期</span><span class="sxs-lookup"><span data-stu-id="a2696-115">postpone</span></span>|<span data-ttu-id="a2696-116">1</span><span class="sxs-lookup"><span data-stu-id="a2696-116">1</span></span>|<span data-ttu-id="a2696-117">30 日以内に更新プログラムの自動インストールを延期します。</span><span class="sxs-lookup"><span data-stu-id="a2696-117">Postpone automatic install of updates up to 30 days.</span></span>|
|<span data-ttu-id="a2696-118">ウィンドウ表示</span><span class="sxs-lookup"><span data-stu-id="a2696-118">windowed</span></span>|<span data-ttu-id="a2696-119">2</span><span class="sxs-lookup"><span data-stu-id="a2696-119">2</span></span>|<span data-ttu-id="a2696-120">保守時間帯の毎日の中には、自動的にインストールします。</span><span class="sxs-lookup"><span data-stu-id="a2696-120">Install automatically inside a daily maintenance window.</span></span>|
|<span data-ttu-id="a2696-121">自動</span><span class="sxs-lookup"><span data-stu-id="a2696-121">automatic</span></span>|<span data-ttu-id="a2696-122">3</span><span class="sxs-lookup"><span data-stu-id="a2696-122">3</span></span>|<span data-ttu-id="a2696-123">できるだけ早く更新を自動的にインストールします。</span><span class="sxs-lookup"><span data-stu-id="a2696-123">Automatically install updates as soon as possible.</span></span>|




