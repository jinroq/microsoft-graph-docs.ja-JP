---
title: androidDeviceOwnerSystemUpdateInstallType 列挙型
description: Android デバイス所有者のシステム更新の種類。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2beb0b2eba9c7c67a04d141ecff1463d4ae550ef
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34983765"
---
# <a name="androiddeviceownersystemupdateinstalltype-enum-type"></a><span data-ttu-id="6582c-103">androidDeviceOwnerSystemUpdateInstallType 列挙型</span><span class="sxs-lookup"><span data-stu-id="6582c-103">androidDeviceOwnerSystemUpdateInstallType enum type</span></span>

> <span data-ttu-id="6582c-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6582c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6582c-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6582c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6582c-106">Android デバイス所有者のシステム更新の種類。</span><span class="sxs-lookup"><span data-stu-id="6582c-106">System Update Types for Android Device Owner.</span></span>

## <a name="members"></a><span data-ttu-id="6582c-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="6582c-107">Members</span></span>
|<span data-ttu-id="6582c-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="6582c-108">Member</span></span>|<span data-ttu-id="6582c-109">値</span><span class="sxs-lookup"><span data-stu-id="6582c-109">Value</span></span>|<span data-ttu-id="6582c-110">説明</span><span class="sxs-lookup"><span data-stu-id="6582c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6582c-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="6582c-111">deviceDefault</span></span>|<span data-ttu-id="6582c-112">.0</span><span class="sxs-lookup"><span data-stu-id="6582c-112">0</span></span>|<span data-ttu-id="6582c-113">デバイスの既定の動作。通常、ユーザーにシステム更新プログラムの使用を求めるメッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="6582c-113">Device default behavior, which typically prompts the user to accept system updates.</span></span>|
|<span data-ttu-id="6582c-114">延期</span><span class="sxs-lookup"><span data-stu-id="6582c-114">postpone</span></span>|<span data-ttu-id="6582c-115">1-d</span><span class="sxs-lookup"><span data-stu-id="6582c-115">1</span></span>|<span data-ttu-id="6582c-116">更新プログラムの自動インストールを最大30日間延期します。</span><span class="sxs-lookup"><span data-stu-id="6582c-116">Postpone automatic install of updates up to 30 days.</span></span>|
|<span data-ttu-id="6582c-117">ウィンドウ</span><span class="sxs-lookup"><span data-stu-id="6582c-117">windowed</span></span>|<span data-ttu-id="6582c-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="6582c-118">2</span></span>|<span data-ttu-id="6582c-119">毎日のメンテナンス期間内に自動的にインストールします。</span><span class="sxs-lookup"><span data-stu-id="6582c-119">Install automatically inside a daily maintenance window.</span></span>|
|<span data-ttu-id="6582c-120">自動</span><span class="sxs-lookup"><span data-stu-id="6582c-120">automatic</span></span>|<span data-ttu-id="6582c-121">1/3</span><span class="sxs-lookup"><span data-stu-id="6582c-121">3</span></span>|<span data-ttu-id="6582c-122">可能な限り早く、更新プログラムを自動的にインストールします。</span><span class="sxs-lookup"><span data-stu-id="6582c-122">Automatically install updates as soon as possible.</span></span>|





