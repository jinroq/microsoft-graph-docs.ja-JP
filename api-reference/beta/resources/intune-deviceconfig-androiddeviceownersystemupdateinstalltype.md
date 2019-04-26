---
title: androidDeviceOwnerSystemUpdateInstallType 列挙型
description: Android デバイス所有者のシステム更新の種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 86f5e5d2c698652e7155c300fdd51e50442a1c44
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32556341"
---
# <a name="androiddeviceownersystemupdateinstalltype-enum-type"></a><span data-ttu-id="e55c8-103">androidDeviceOwnerSystemUpdateInstallType 列挙型</span><span class="sxs-lookup"><span data-stu-id="e55c8-103">androidDeviceOwnerSystemUpdateInstallType enum type</span></span>

> <span data-ttu-id="e55c8-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e55c8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e55c8-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e55c8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e55c8-106">Android デバイス所有者のシステム更新の種類。</span><span class="sxs-lookup"><span data-stu-id="e55c8-106">System Update Types for Android Device Owner.</span></span>

## <a name="members"></a><span data-ttu-id="e55c8-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="e55c8-107">Members</span></span>
|<span data-ttu-id="e55c8-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="e55c8-108">Member</span></span>|<span data-ttu-id="e55c8-109">値</span><span class="sxs-lookup"><span data-stu-id="e55c8-109">Value</span></span>|<span data-ttu-id="e55c8-110">説明</span><span class="sxs-lookup"><span data-stu-id="e55c8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e55c8-111">devicedefault</span><span class="sxs-lookup"><span data-stu-id="e55c8-111">deviceDefault</span></span>|<span data-ttu-id="e55c8-112">.0</span><span class="sxs-lookup"><span data-stu-id="e55c8-112">0</span></span>|<span data-ttu-id="e55c8-113">デバイスの既定の動作。通常、ユーザーにシステム更新プログラムの使用を求めるメッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="e55c8-113">Device default behavior, which typically prompts the user to accept system updates.</span></span>|
|<span data-ttu-id="e55c8-114">延期</span><span class="sxs-lookup"><span data-stu-id="e55c8-114">postpone</span></span>|<span data-ttu-id="e55c8-115">1 </span><span class="sxs-lookup"><span data-stu-id="e55c8-115">1</span></span>|<span data-ttu-id="e55c8-116">更新プログラムの自動インストールを最大30日間延期します。</span><span class="sxs-lookup"><span data-stu-id="e55c8-116">Postpone automatic install of updates up to 30 days.</span></span>|
|<span data-ttu-id="e55c8-117">ウィンドウ</span><span class="sxs-lookup"><span data-stu-id="e55c8-117">windowed</span></span>|<span data-ttu-id="e55c8-118">2 </span><span class="sxs-lookup"><span data-stu-id="e55c8-118">2</span></span>|<span data-ttu-id="e55c8-119">毎日のメンテナンス期間内に自動的にインストールします。</span><span class="sxs-lookup"><span data-stu-id="e55c8-119">Install automatically inside a daily maintenance window.</span></span>|
|<span data-ttu-id="e55c8-120">自動</span><span class="sxs-lookup"><span data-stu-id="e55c8-120">automatic</span></span>|<span data-ttu-id="e55c8-121">3 </span><span class="sxs-lookup"><span data-stu-id="e55c8-121">3</span></span>|<span data-ttu-id="e55c8-122">可能な限り早く、更新プログラムを自動的にインストールします。</span><span class="sxs-lookup"><span data-stu-id="e55c8-122">Automatically install updates as soon as possible.</span></span>|





