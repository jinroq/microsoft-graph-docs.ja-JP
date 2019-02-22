---
title: androidDeviceOwnerSystemUpdateInstallType 列挙型
description: Android デバイス所有者のシステム更新の種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b6f99ba32a5461913579a23e7fe8f29a3c0b6950
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163659"
---
# <a name="androiddeviceownersystemupdateinstalltype-enum-type"></a><span data-ttu-id="714ea-103">androidDeviceOwnerSystemUpdateInstallType 列挙型</span><span class="sxs-lookup"><span data-stu-id="714ea-103">androidDeviceOwnerSystemUpdateInstallType enum type</span></span>

> <span data-ttu-id="714ea-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="714ea-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="714ea-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="714ea-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="714ea-106">Android デバイス所有者のシステム更新の種類。</span><span class="sxs-lookup"><span data-stu-id="714ea-106">System Update Types for Android Device Owner.</span></span>

## <a name="members"></a><span data-ttu-id="714ea-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="714ea-107">Members</span></span>
|<span data-ttu-id="714ea-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="714ea-108">Member</span></span>|<span data-ttu-id="714ea-109">値</span><span class="sxs-lookup"><span data-stu-id="714ea-109">Value</span></span>|<span data-ttu-id="714ea-110">説明</span><span class="sxs-lookup"><span data-stu-id="714ea-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="714ea-111">devicedefault</span><span class="sxs-lookup"><span data-stu-id="714ea-111">deviceDefault</span></span>|<span data-ttu-id="714ea-112">.0</span><span class="sxs-lookup"><span data-stu-id="714ea-112">0</span></span>|<span data-ttu-id="714ea-113">デバイスの既定の動作。通常、ユーザーにシステム更新プログラムの使用を求めるメッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="714ea-113">Device default behavior, which typically prompts the user to accept system updates.</span></span>|
|<span data-ttu-id="714ea-114">延期</span><span class="sxs-lookup"><span data-stu-id="714ea-114">postpone</span></span>|<span data-ttu-id="714ea-115">1-d</span><span class="sxs-lookup"><span data-stu-id="714ea-115">1</span></span>|<span data-ttu-id="714ea-116">更新プログラムの自動インストールを最大30日間延期します。</span><span class="sxs-lookup"><span data-stu-id="714ea-116">Postpone automatic install of updates up to 30 days.</span></span>|
|<span data-ttu-id="714ea-117">ウィンドウ</span><span class="sxs-lookup"><span data-stu-id="714ea-117">windowed</span></span>|<span data-ttu-id="714ea-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="714ea-118">2</span></span>|<span data-ttu-id="714ea-119">毎日のメンテナンス期間内に自動的にインストールします。</span><span class="sxs-lookup"><span data-stu-id="714ea-119">Install automatically inside a daily maintenance window.</span></span>|
|<span data-ttu-id="714ea-120">自動</span><span class="sxs-lookup"><span data-stu-id="714ea-120">automatic</span></span>|<span data-ttu-id="714ea-121">1/3</span><span class="sxs-lookup"><span data-stu-id="714ea-121">3</span></span>|<span data-ttu-id="714ea-122">可能な限り早く、更新プログラムを自動的にインストールします。</span><span class="sxs-lookup"><span data-stu-id="714ea-122">Automatically install updates as soon as possible.</span></span>|




