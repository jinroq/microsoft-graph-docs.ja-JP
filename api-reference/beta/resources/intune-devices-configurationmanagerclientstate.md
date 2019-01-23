---
title: configurationManagerClientState 列挙型
description: 構成マネージャーのクライアントの状態
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 82f4b677001346f9bd32c1bc54bed6e7fbac253d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425786"
---
# <a name="configurationmanagerclientstate-enum-type"></a><span data-ttu-id="37092-103">configurationManagerClientState 列挙型</span><span class="sxs-lookup"><span data-stu-id="37092-103">configurationManagerClientState enum type</span></span>

> <span data-ttu-id="37092-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="37092-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="37092-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="37092-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="37092-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="37092-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37092-107">構成マネージャーのクライアントの状態</span><span class="sxs-lookup"><span data-stu-id="37092-107">Configuration manager client state</span></span>

## <a name="members"></a><span data-ttu-id="37092-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="37092-108">Members</span></span>
|<span data-ttu-id="37092-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="37092-109">Member</span></span>|<span data-ttu-id="37092-110">値</span><span class="sxs-lookup"><span data-stu-id="37092-110">Value</span></span>|<span data-ttu-id="37092-111">説明</span><span class="sxs-lookup"><span data-stu-id="37092-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37092-112">不明</span><span class="sxs-lookup"><span data-stu-id="37092-112">unknown</span></span>|<span data-ttu-id="37092-113">0</span><span class="sxs-lookup"><span data-stu-id="37092-113">0</span></span>|<span data-ttu-id="37092-114">構成マネージャー エージェント 1806 よりも古いか、インストールされていないか、またはこのデバイスが 30 日間を超えてからの Intune にチェックがないです。</span><span class="sxs-lookup"><span data-stu-id="37092-114">Configuration manager agent is older than 1806 or not installed or this device has not checked into Intune for over 30 days.</span></span>|
|<span data-ttu-id="37092-115">インストールされています。</span><span class="sxs-lookup"><span data-stu-id="37092-115">installed</span></span>|<span data-ttu-id="37092-116">1</span><span class="sxs-lookup"><span data-stu-id="37092-116">1</span></span>|<span data-ttu-id="37092-117">構成マネージャー エージェントがインストールされますが、可能性がありますが表示されない、構成マネージャー コンソールでまだ。</span><span class="sxs-lookup"><span data-stu-id="37092-117">The configuration manager agent is installed but may not be showing up in the configuration manager console yet.</span></span> <span data-ttu-id="37092-118">更新するために、いくつかの時間を待機します。</span><span class="sxs-lookup"><span data-stu-id="37092-118">Wait a few hours for it to refresh.</span></span>|
|<span data-ttu-id="37092-119">正常な状態</span><span class="sxs-lookup"><span data-stu-id="37092-119">healthy</span></span>|<span data-ttu-id="37092-120">7</span><span class="sxs-lookup"><span data-stu-id="37092-120">7</span></span>|<span data-ttu-id="37092-121">このデバイスは、構成マネージャーのサービスを使用して正常に確認できませんでした。</span><span class="sxs-lookup"><span data-stu-id="37092-121">This device was able to check in with the configuration manager service successfully.</span></span>|
|<span data-ttu-id="37092-122">installFailed</span><span class="sxs-lookup"><span data-stu-id="37092-122">installFailed</span></span>|<span data-ttu-id="37092-123">8</span><span class="sxs-lookup"><span data-stu-id="37092-123">8</span></span>|<span data-ttu-id="37092-124">構成マネージャー エージェントをインストールできませんでした。</span><span class="sxs-lookup"><span data-stu-id="37092-124">The configuration manager agent failed to install.</span></span>|
|<span data-ttu-id="37092-125">updateFailed</span><span class="sxs-lookup"><span data-stu-id="37092-125">updateFailed</span></span>|<span data-ttu-id="37092-126">11</span><span class="sxs-lookup"><span data-stu-id="37092-126">11</span></span>|<span data-ttu-id="37092-127">構成マネージャー エージェントのバージョンの y を x のバージョンから更新できませんでした。</span><span class="sxs-lookup"><span data-stu-id="37092-127">The update from version x to version y of the configuration manager agent failed.</span></span> |
|<span data-ttu-id="37092-128">communicationError</span><span class="sxs-lookup"><span data-stu-id="37092-128">communicationError</span></span>|<span data-ttu-id="37092-129">19</span><span class="sxs-lookup"><span data-stu-id="37092-129">19</span></span>|<span data-ttu-id="37092-130">構成マネージャー エージェントが過去に、構成マネージャーのサービスにアクセスできないが、不要になったこと。</span><span class="sxs-lookup"><span data-stu-id="37092-130">The configuration manager agent was able to reach the configuration manager service in the past but is now no longer able to.</span></span> |




