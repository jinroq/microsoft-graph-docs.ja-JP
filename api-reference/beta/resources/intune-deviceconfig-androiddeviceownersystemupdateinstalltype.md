---
title: androidDeviceOwnerSystemUpdateInstallType 列挙型
description: Android デバイスの所有者のシステム更新プログラムの種類。
author: tfitzmac
ms.openlocfilehash: e2dc66851e0fa98d52a3fec30385e0fd27e6f6ca
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323199"
---
# <a name="androiddeviceownersystemupdateinstalltype-enum-type"></a><span data-ttu-id="685f2-103">androidDeviceOwnerSystemUpdateInstallType 列挙型</span><span class="sxs-lookup"><span data-stu-id="685f2-103">androidDeviceOwnerSystemUpdateInstallType enum type</span></span>

> <span data-ttu-id="685f2-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="685f2-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="685f2-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="685f2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="685f2-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="685f2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="685f2-107">Android デバイスの所有者のシステム更新プログラムの種類。</span><span class="sxs-lookup"><span data-stu-id="685f2-107">System Update Types for Android Device Owner.</span></span>
## <a name="members"></a><span data-ttu-id="685f2-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="685f2-108">Members</span></span>
|<span data-ttu-id="685f2-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="685f2-109">Member</span></span>|<span data-ttu-id="685f2-110">値</span><span class="sxs-lookup"><span data-stu-id="685f2-110">Value</span></span>|<span data-ttu-id="685f2-111">説明</span><span class="sxs-lookup"><span data-stu-id="685f2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="685f2-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="685f2-112">deviceDefault</span></span>|<span data-ttu-id="685f2-113">0</span><span class="sxs-lookup"><span data-stu-id="685f2-113">0</span></span>|<span data-ttu-id="685f2-114">デバイス既定の動作、通常システムの更新を許可するユーザーを求められます。</span><span class="sxs-lookup"><span data-stu-id="685f2-114">Device default behavior, which typically prompts the user to accept system updates.</span></span>|
|<span data-ttu-id="685f2-115">延期</span><span class="sxs-lookup"><span data-stu-id="685f2-115">postpone</span></span>|<span data-ttu-id="685f2-116">1</span><span class="sxs-lookup"><span data-stu-id="685f2-116">1</span></span>|<span data-ttu-id="685f2-117">30 日以内に更新プログラムの自動インストールを延期します。</span><span class="sxs-lookup"><span data-stu-id="685f2-117">Postpone automatic install of updates up to 30 days.</span></span>|
|<span data-ttu-id="685f2-118">ウィンドウ表示</span><span class="sxs-lookup"><span data-stu-id="685f2-118">windowed</span></span>|<span data-ttu-id="685f2-119">2</span><span class="sxs-lookup"><span data-stu-id="685f2-119">2</span></span>|<span data-ttu-id="685f2-120">保守時間帯の毎日の中には、自動的にインストールします。</span><span class="sxs-lookup"><span data-stu-id="685f2-120">Install automatically inside a daily maintenance window.</span></span>|
|<span data-ttu-id="685f2-121">自動</span><span class="sxs-lookup"><span data-stu-id="685f2-121">automatic</span></span>|<span data-ttu-id="685f2-122">3</span><span class="sxs-lookup"><span data-stu-id="685f2-122">3</span></span>|<span data-ttu-id="685f2-123">できるだけ早く更新を自動的にインストールします。</span><span class="sxs-lookup"><span data-stu-id="685f2-123">Automatically install updates as soon as possible.</span></span>|





