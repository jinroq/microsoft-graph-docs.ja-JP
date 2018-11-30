---
title: androidDeviceOwnerSystemUpdateInstallType 列挙型
description: Android デバイスの所有者のシステム更新プログラムの種類。
ms.openlocfilehash: e9f23fd96ed0965b6693776858082e2df4925f37
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070420"
---
# <a name="androiddeviceownersystemupdateinstalltype-enum-type"></a><span data-ttu-id="ebfed-103">androidDeviceOwnerSystemUpdateInstallType 列挙型</span><span class="sxs-lookup"><span data-stu-id="ebfed-103">androidDeviceOwnerSystemUpdateInstallType enum type</span></span>

> <span data-ttu-id="ebfed-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ebfed-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ebfed-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ebfed-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ebfed-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ebfed-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ebfed-107">Android デバイスの所有者のシステム更新プログラムの種類。</span><span class="sxs-lookup"><span data-stu-id="ebfed-107">System Update Types for Android Device Owner.</span></span>
## <a name="members"></a><span data-ttu-id="ebfed-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="ebfed-108">Members</span></span>
|<span data-ttu-id="ebfed-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="ebfed-109">Member</span></span>|<span data-ttu-id="ebfed-110">値</span><span class="sxs-lookup"><span data-stu-id="ebfed-110">Value</span></span>|<span data-ttu-id="ebfed-111">説明</span><span class="sxs-lookup"><span data-stu-id="ebfed-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebfed-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="ebfed-112">deviceDefault</span></span>|<span data-ttu-id="ebfed-113">0</span><span class="sxs-lookup"><span data-stu-id="ebfed-113">0</span></span>|<span data-ttu-id="ebfed-114">デバイス既定の動作、通常システムの更新を許可するユーザーを求められます。</span><span class="sxs-lookup"><span data-stu-id="ebfed-114">Device default behavior, which typically prompts the user to accept system updates.</span></span>|
|<span data-ttu-id="ebfed-115">延期</span><span class="sxs-lookup"><span data-stu-id="ebfed-115">postpone</span></span>|<span data-ttu-id="ebfed-116">1</span><span class="sxs-lookup"><span data-stu-id="ebfed-116">1</span></span>|<span data-ttu-id="ebfed-117">30 日以内に更新プログラムの自動インストールを延期します。</span><span class="sxs-lookup"><span data-stu-id="ebfed-117">Postpone automatic install of updates up to 30 days.</span></span>|
|<span data-ttu-id="ebfed-118">ウィンドウ表示</span><span class="sxs-lookup"><span data-stu-id="ebfed-118">windowed</span></span>|<span data-ttu-id="ebfed-119">2</span><span class="sxs-lookup"><span data-stu-id="ebfed-119">2</span></span>|<span data-ttu-id="ebfed-120">保守時間帯の毎日の中には、自動的にインストールします。</span><span class="sxs-lookup"><span data-stu-id="ebfed-120">Install automatically inside a daily maintenance window.</span></span>|
|<span data-ttu-id="ebfed-121">自動</span><span class="sxs-lookup"><span data-stu-id="ebfed-121">automatic</span></span>|<span data-ttu-id="ebfed-122">3</span><span class="sxs-lookup"><span data-stu-id="ebfed-122">3</span></span>|<span data-ttu-id="ebfed-123">できるだけ早く更新を自動的にインストールします。</span><span class="sxs-lookup"><span data-stu-id="ebfed-123">Automatically install updates as soon as possible.</span></span>|





