---
title: configurationManagerClientState 列挙型
description: 構成マネージャーのクライアントの状態
author: tfitzmac
ms.openlocfilehash: dc67a5fb1c517e65da937996ed65adaa621fa3c5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354048"
---
# <a name="configurationmanagerclientstate-enum-type"></a><span data-ttu-id="f3b76-103">configurationManagerClientState 列挙型</span><span class="sxs-lookup"><span data-stu-id="f3b76-103">configurationManagerClientState enum type</span></span>

> <span data-ttu-id="f3b76-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f3b76-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f3b76-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f3b76-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f3b76-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f3b76-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f3b76-107">構成マネージャーのクライアントの状態</span><span class="sxs-lookup"><span data-stu-id="f3b76-107">Configuration manager client state</span></span>
## <a name="members"></a><span data-ttu-id="f3b76-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="f3b76-108">Members</span></span>
|<span data-ttu-id="f3b76-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="f3b76-109">Member</span></span>|<span data-ttu-id="f3b76-110">値</span><span class="sxs-lookup"><span data-stu-id="f3b76-110">Value</span></span>|<span data-ttu-id="f3b76-111">説明</span><span class="sxs-lookup"><span data-stu-id="f3b76-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3b76-112">不明</span><span class="sxs-lookup"><span data-stu-id="f3b76-112">unknown</span></span>|<span data-ttu-id="f3b76-113">0</span><span class="sxs-lookup"><span data-stu-id="f3b76-113">0</span></span>|<span data-ttu-id="f3b76-114">構成マネージャー エージェント 1806 よりも古いか、インストールされていないか、またはこのデバイスが 30 日間を超えてからの Intune にチェックがないです。</span><span class="sxs-lookup"><span data-stu-id="f3b76-114">Configuration manager agent is older than 1806 or not installed or this device has not checked into Intune for over 30 days.</span></span>|
|<span data-ttu-id="f3b76-115">インストールされています。</span><span class="sxs-lookup"><span data-stu-id="f3b76-115">installed</span></span>|<span data-ttu-id="f3b76-116">1</span><span class="sxs-lookup"><span data-stu-id="f3b76-116">1</span></span>|<span data-ttu-id="f3b76-117">構成マネージャー エージェントがインストールされますが、可能性がありますが表示されない、構成マネージャー コンソールでまだ。</span><span class="sxs-lookup"><span data-stu-id="f3b76-117">The configuration manager agent is installed but may not be showing up in the configuration manager console yet.</span></span> <span data-ttu-id="f3b76-118">更新するために、いくつかの時間を待機します。</span><span class="sxs-lookup"><span data-stu-id="f3b76-118">Wait a few hours for it to refresh.</span></span>|
|<span data-ttu-id="f3b76-119">正常な状態</span><span class="sxs-lookup"><span data-stu-id="f3b76-119">healthy</span></span>|<span data-ttu-id="f3b76-120">7</span><span class="sxs-lookup"><span data-stu-id="f3b76-120">7</span></span>|<span data-ttu-id="f3b76-121">このデバイスは、構成マネージャーのサービスを使用して正常に確認できませんでした。</span><span class="sxs-lookup"><span data-stu-id="f3b76-121">This device was able to check in with the configuration manager service successfully.</span></span>|
|<span data-ttu-id="f3b76-122">installFailed</span><span class="sxs-lookup"><span data-stu-id="f3b76-122">installFailed</span></span>|<span data-ttu-id="f3b76-123">8</span><span class="sxs-lookup"><span data-stu-id="f3b76-123">8</span></span>|<span data-ttu-id="f3b76-124">構成マネージャー エージェントをインストールできませんでした。</span><span class="sxs-lookup"><span data-stu-id="f3b76-124">The configuration manager agent failed to install.</span></span>|
|<span data-ttu-id="f3b76-125">updateFailed</span><span class="sxs-lookup"><span data-stu-id="f3b76-125">updateFailed</span></span>|<span data-ttu-id="f3b76-126">11</span><span class="sxs-lookup"><span data-stu-id="f3b76-126">11</span></span>|<span data-ttu-id="f3b76-127">構成マネージャー エージェントのバージョンの y を x のバージョンから更新できませんでした。</span><span class="sxs-lookup"><span data-stu-id="f3b76-127">The update from version x to version y of the configuration manager agent failed.</span></span> |
|<span data-ttu-id="f3b76-128">communicationError</span><span class="sxs-lookup"><span data-stu-id="f3b76-128">communicationError</span></span>|<span data-ttu-id="f3b76-129">19</span><span class="sxs-lookup"><span data-stu-id="f3b76-129">19</span></span>|<span data-ttu-id="f3b76-130">構成マネージャー エージェントが過去に、構成マネージャーのサービスにアクセスできないが、不要になったこと。</span><span class="sxs-lookup"><span data-stu-id="f3b76-130">The configuration manager agent was able to reach the configuration manager service in the past but is now no longer able to.</span></span> |





