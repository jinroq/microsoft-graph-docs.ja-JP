---
title: androidDeviceOwnerSystemUpdateInstallType 列挙型
description: Android デバイス所有者のシステム更新の種類。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 2cfc91de723bb10e39545b570d94ec1944221f9c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971502"
---
# <a name="androiddeviceownersystemupdateinstalltype-enum-type"></a><span data-ttu-id="54c3f-103">androidDeviceOwnerSystemUpdateInstallType 列挙型</span><span class="sxs-lookup"><span data-stu-id="54c3f-103">androidDeviceOwnerSystemUpdateInstallType enum type</span></span>

> <span data-ttu-id="54c3f-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="54c3f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="54c3f-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="54c3f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54c3f-106">Android デバイス所有者のシステム更新の種類。</span><span class="sxs-lookup"><span data-stu-id="54c3f-106">System Update Types for Android Device Owner.</span></span>

## <a name="members"></a><span data-ttu-id="54c3f-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="54c3f-107">Members</span></span>
|<span data-ttu-id="54c3f-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="54c3f-108">Member</span></span>|<span data-ttu-id="54c3f-109">値</span><span class="sxs-lookup"><span data-stu-id="54c3f-109">Value</span></span>|<span data-ttu-id="54c3f-110">説明</span><span class="sxs-lookup"><span data-stu-id="54c3f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54c3f-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="54c3f-111">deviceDefault</span></span>|<span data-ttu-id="54c3f-112">.0</span><span class="sxs-lookup"><span data-stu-id="54c3f-112">0</span></span>|<span data-ttu-id="54c3f-113">デバイスの既定の動作。通常、ユーザーにシステム更新プログラムの使用を求めるメッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="54c3f-113">Device default behavior, which typically prompts the user to accept system updates.</span></span>|
|<span data-ttu-id="54c3f-114">延期</span><span class="sxs-lookup"><span data-stu-id="54c3f-114">postpone</span></span>|<span data-ttu-id="54c3f-115">1-d</span><span class="sxs-lookup"><span data-stu-id="54c3f-115">1</span></span>|<span data-ttu-id="54c3f-116">更新プログラムの自動インストールを最大30日間延期します。</span><span class="sxs-lookup"><span data-stu-id="54c3f-116">Postpone automatic install of updates up to 30 days.</span></span>|
|<span data-ttu-id="54c3f-117">ウィンドウ</span><span class="sxs-lookup"><span data-stu-id="54c3f-117">windowed</span></span>|<span data-ttu-id="54c3f-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="54c3f-118">2</span></span>|<span data-ttu-id="54c3f-119">毎日のメンテナンス期間内に自動的にインストールします。</span><span class="sxs-lookup"><span data-stu-id="54c3f-119">Install automatically inside a daily maintenance window.</span></span>|
|<span data-ttu-id="54c3f-120">自動</span><span class="sxs-lookup"><span data-stu-id="54c3f-120">automatic</span></span>|<span data-ttu-id="54c3f-121">1/3</span><span class="sxs-lookup"><span data-stu-id="54c3f-121">3</span></span>|<span data-ttu-id="54c3f-122">可能な限り早く、更新プログラムを自動的にインストールします。</span><span class="sxs-lookup"><span data-stu-id="54c3f-122">Automatically install updates as soon as possible.</span></span>|





