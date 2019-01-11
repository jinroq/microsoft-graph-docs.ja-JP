---
title: configurationManagerClientState 列挙型
description: 構成マネージャーのクライアントの状態
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 36abbe4451a6e053387b27fce3e9a4e25dcc1a95
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806252"
---
# <a name="configurationmanagerclientstate-enum-type"></a><span data-ttu-id="ee6e9-103">configurationManagerClientState 列挙型</span><span class="sxs-lookup"><span data-stu-id="ee6e9-103">configurationManagerClientState enum type</span></span>

> <span data-ttu-id="ee6e9-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ee6e9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ee6e9-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ee6e9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ee6e9-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ee6e9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ee6e9-107">構成マネージャーのクライアントの状態</span><span class="sxs-lookup"><span data-stu-id="ee6e9-107">Configuration manager client state</span></span>
## <a name="members"></a><span data-ttu-id="ee6e9-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="ee6e9-108">Members</span></span>
|<span data-ttu-id="ee6e9-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="ee6e9-109">Member</span></span>|<span data-ttu-id="ee6e9-110">値</span><span class="sxs-lookup"><span data-stu-id="ee6e9-110">Value</span></span>|<span data-ttu-id="ee6e9-111">説明</span><span class="sxs-lookup"><span data-stu-id="ee6e9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee6e9-112">不明</span><span class="sxs-lookup"><span data-stu-id="ee6e9-112">unknown</span></span>|<span data-ttu-id="ee6e9-113">0</span><span class="sxs-lookup"><span data-stu-id="ee6e9-113">0</span></span>|<span data-ttu-id="ee6e9-114">構成マネージャー エージェント 1806 よりも古いか、インストールされていないか、またはこのデバイスが 30 日間を超えてからの Intune にチェックがないです。</span><span class="sxs-lookup"><span data-stu-id="ee6e9-114">Configuration manager agent is older than 1806 or not installed or this device has not checked into Intune for over 30 days.</span></span>|
|<span data-ttu-id="ee6e9-115">インストールされています。</span><span class="sxs-lookup"><span data-stu-id="ee6e9-115">installed</span></span>|<span data-ttu-id="ee6e9-116">1</span><span class="sxs-lookup"><span data-stu-id="ee6e9-116">1</span></span>|<span data-ttu-id="ee6e9-117">構成マネージャー エージェントがインストールされますが、可能性がありますが表示されない、構成マネージャー コンソールでまだ。</span><span class="sxs-lookup"><span data-stu-id="ee6e9-117">The configuration manager agent is installed but may not be showing up in the configuration manager console yet.</span></span> <span data-ttu-id="ee6e9-118">更新するために、いくつかの時間を待機します。</span><span class="sxs-lookup"><span data-stu-id="ee6e9-118">Wait a few hours for it to refresh.</span></span>|
|<span data-ttu-id="ee6e9-119">正常な状態</span><span class="sxs-lookup"><span data-stu-id="ee6e9-119">healthy</span></span>|<span data-ttu-id="ee6e9-120">7</span><span class="sxs-lookup"><span data-stu-id="ee6e9-120">7</span></span>|<span data-ttu-id="ee6e9-121">このデバイスは、構成マネージャーのサービスを使用して正常に確認できませんでした。</span><span class="sxs-lookup"><span data-stu-id="ee6e9-121">This device was able to check in with the configuration manager service successfully.</span></span>|
|<span data-ttu-id="ee6e9-122">installFailed</span><span class="sxs-lookup"><span data-stu-id="ee6e9-122">installFailed</span></span>|<span data-ttu-id="ee6e9-123">8</span><span class="sxs-lookup"><span data-stu-id="ee6e9-123">8</span></span>|<span data-ttu-id="ee6e9-124">構成マネージャー エージェントをインストールできませんでした。</span><span class="sxs-lookup"><span data-stu-id="ee6e9-124">The configuration manager agent failed to install.</span></span>|
|<span data-ttu-id="ee6e9-125">updateFailed</span><span class="sxs-lookup"><span data-stu-id="ee6e9-125">updateFailed</span></span>|<span data-ttu-id="ee6e9-126">11</span><span class="sxs-lookup"><span data-stu-id="ee6e9-126">11</span></span>|<span data-ttu-id="ee6e9-127">構成マネージャー エージェントのバージョンの y を x のバージョンから更新できませんでした。</span><span class="sxs-lookup"><span data-stu-id="ee6e9-127">The update from version x to version y of the configuration manager agent failed.</span></span> |
|<span data-ttu-id="ee6e9-128">communicationError</span><span class="sxs-lookup"><span data-stu-id="ee6e9-128">communicationError</span></span>|<span data-ttu-id="ee6e9-129">19</span><span class="sxs-lookup"><span data-stu-id="ee6e9-129">19</span></span>|<span data-ttu-id="ee6e9-130">構成マネージャー エージェントが過去に、構成マネージャーのサービスにアクセスできないが、不要になったこと。</span><span class="sxs-lookup"><span data-stu-id="ee6e9-130">The configuration manager agent was able to reach the configuration manager service in the past but is now no longer able to.</span></span> |





