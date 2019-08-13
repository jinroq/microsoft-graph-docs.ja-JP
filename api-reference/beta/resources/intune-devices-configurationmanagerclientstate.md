---
title: configurationManagerClientState 列挙型
description: 構成マネージャーのクライアントの状態
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ba7de7ee3612c4d1e8e419522e8d18587339343c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36370285"
---
# <a name="configurationmanagerclientstate-enum-type"></a><span data-ttu-id="1e25a-103">configurationManagerClientState 列挙型</span><span class="sxs-lookup"><span data-stu-id="1e25a-103">configurationManagerClientState enum type</span></span>

> <span data-ttu-id="1e25a-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1e25a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1e25a-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1e25a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1e25a-106">構成マネージャーのクライアントの状態</span><span class="sxs-lookup"><span data-stu-id="1e25a-106">Configuration manager client state</span></span>

## <a name="members"></a><span data-ttu-id="1e25a-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="1e25a-107">Members</span></span>
|<span data-ttu-id="1e25a-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="1e25a-108">Member</span></span>|<span data-ttu-id="1e25a-109">値</span><span class="sxs-lookup"><span data-stu-id="1e25a-109">Value</span></span>|<span data-ttu-id="1e25a-110">説明</span><span class="sxs-lookup"><span data-stu-id="1e25a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e25a-111">不明</span><span class="sxs-lookup"><span data-stu-id="1e25a-111">unknown</span></span>|<span data-ttu-id="1e25a-112">.0</span><span class="sxs-lookup"><span data-stu-id="1e25a-112">0</span></span>|<span data-ttu-id="1e25a-113">Configuration manager エージェントが1806より古いか、インストールされていないか、またはこのデバイスが30日間以上 Intune にチェックインされていません。</span><span class="sxs-lookup"><span data-stu-id="1e25a-113">Configuration manager agent is older than 1806 or not installed or this device has not checked into Intune for over 30 days.</span></span>|
|<span data-ttu-id="1e25a-114">れる</span><span class="sxs-lookup"><span data-stu-id="1e25a-114">installed</span></span>|<span data-ttu-id="1e25a-115">1-d</span><span class="sxs-lookup"><span data-stu-id="1e25a-115">1</span></span>|<span data-ttu-id="1e25a-116">構成マネージャーエージェントがインストールされていますが、構成マネージャーコンソールに表示されていない可能性があります。</span><span class="sxs-lookup"><span data-stu-id="1e25a-116">The configuration manager agent is installed but may not be showing up in the configuration manager console yet.</span></span> <span data-ttu-id="1e25a-117">更新が完了するまで数時間待機します。</span><span class="sxs-lookup"><span data-stu-id="1e25a-117">Wait a few hours for it to refresh.</span></span>|
|<span data-ttu-id="1e25a-118">稼動</span><span class="sxs-lookup"><span data-stu-id="1e25a-118">healthy</span></span>|<span data-ttu-id="1e25a-119">7</span><span class="sxs-lookup"><span data-stu-id="1e25a-119">7</span></span>|<span data-ttu-id="1e25a-120">このデバイスは、configuration manager サービスを正常にチェックインすることができました。</span><span class="sxs-lookup"><span data-stu-id="1e25a-120">This device was able to check in with the configuration manager service successfully.</span></span>|
|<span data-ttu-id="1e25a-121">installFailed</span><span class="sxs-lookup"><span data-stu-id="1e25a-121">installFailed</span></span>|<span data-ttu-id="1e25a-122">8 </span><span class="sxs-lookup"><span data-stu-id="1e25a-122">8</span></span>|<span data-ttu-id="1e25a-123">構成マネージャーエージェントのインストールに失敗しました。</span><span class="sxs-lookup"><span data-stu-id="1e25a-123">The configuration manager agent failed to install.</span></span>|
|<span data-ttu-id="1e25a-124">updateFailed</span><span class="sxs-lookup"><span data-stu-id="1e25a-124">updateFailed</span></span>|<span data-ttu-id="1e25a-125">#</span><span class="sxs-lookup"><span data-stu-id="1e25a-125">11</span></span>|<span data-ttu-id="1e25a-126">構成マネージャーエージェントのバージョン x からバージョン y への更新に失敗しました。</span><span class="sxs-lookup"><span data-stu-id="1e25a-126">The update from version x to version y of the configuration manager agent failed.</span></span> |
|<span data-ttu-id="1e25a-127">communicationError</span><span class="sxs-lookup"><span data-stu-id="1e25a-127">communicationError</span></span>|<span data-ttu-id="1e25a-128">年</span><span class="sxs-lookup"><span data-stu-id="1e25a-128">19</span></span>|<span data-ttu-id="1e25a-129">構成マネージャーエージェントは、以前に構成マネージャーサービスにアクセスできましたが、現在は利用できなくなりました。</span><span class="sxs-lookup"><span data-stu-id="1e25a-129">The configuration manager agent was able to reach the configuration manager service in the past but is now no longer able to.</span></span> |



