---
title: configurationmanagerclientstate 列挙型
description: 構成マネージャーのクライアントの状態
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1f6231ecebf407172f2c7178a130d90200868292
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32454245"
---
# <a name="configurationmanagerclientstate-enum-type"></a><span data-ttu-id="0ad8f-103">configurationmanagerclientstate 列挙型</span><span class="sxs-lookup"><span data-stu-id="0ad8f-103">configurationManagerClientState enum type</span></span>

> <span data-ttu-id="0ad8f-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0ad8f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0ad8f-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0ad8f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ad8f-106">構成マネージャーのクライアントの状態</span><span class="sxs-lookup"><span data-stu-id="0ad8f-106">Configuration manager client state</span></span>

## <a name="members"></a><span data-ttu-id="0ad8f-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="0ad8f-107">Members</span></span>
|<span data-ttu-id="0ad8f-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="0ad8f-108">Member</span></span>|<span data-ttu-id="0ad8f-109">値</span><span class="sxs-lookup"><span data-stu-id="0ad8f-109">Value</span></span>|<span data-ttu-id="0ad8f-110">説明</span><span class="sxs-lookup"><span data-stu-id="0ad8f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ad8f-111">不明</span><span class="sxs-lookup"><span data-stu-id="0ad8f-111">unknown</span></span>|<span data-ttu-id="0ad8f-112">.0</span><span class="sxs-lookup"><span data-stu-id="0ad8f-112">0</span></span>|<span data-ttu-id="0ad8f-113">Configuration manager エージェントが1806より古いか、インストールされていないか、またはこのデバイスが30日間以上 Intune にチェックインされていません。</span><span class="sxs-lookup"><span data-stu-id="0ad8f-113">Configuration manager agent is older than 1806 or not installed or this device has not checked into Intune for over 30 days.</span></span>|
|<span data-ttu-id="0ad8f-114">れる</span><span class="sxs-lookup"><span data-stu-id="0ad8f-114">installed</span></span>|<span data-ttu-id="0ad8f-115">1-d</span><span class="sxs-lookup"><span data-stu-id="0ad8f-115">1</span></span>|<span data-ttu-id="0ad8f-116">構成マネージャーエージェントがインストールされていますが、構成マネージャーコンソールに表示されていない可能性があります。</span><span class="sxs-lookup"><span data-stu-id="0ad8f-116">The configuration manager agent is installed but may not be showing up in the configuration manager console yet.</span></span> <span data-ttu-id="0ad8f-117">更新が完了するまで数時間待機します。</span><span class="sxs-lookup"><span data-stu-id="0ad8f-117">Wait a few hours for it to refresh.</span></span>|
|<span data-ttu-id="0ad8f-118">稼動</span><span class="sxs-lookup"><span data-stu-id="0ad8f-118">healthy</span></span>|<span data-ttu-id="0ad8f-119">7</span><span class="sxs-lookup"><span data-stu-id="0ad8f-119">7</span></span>|<span data-ttu-id="0ad8f-120">このデバイスは、configuration manager サービスを正常にチェックインすることができました。</span><span class="sxs-lookup"><span data-stu-id="0ad8f-120">This device was able to check in with the configuration manager service successfully.</span></span>|
|<span data-ttu-id="0ad8f-121">installfailed</span><span class="sxs-lookup"><span data-stu-id="0ad8f-121">installFailed</span></span>|<span data-ttu-id="0ad8f-122">~</span><span class="sxs-lookup"><span data-stu-id="0ad8f-122">8</span></span>|<span data-ttu-id="0ad8f-123">構成マネージャーエージェントのインストールに失敗しました。</span><span class="sxs-lookup"><span data-stu-id="0ad8f-123">The configuration manager agent failed to install.</span></span>|
|<span data-ttu-id="0ad8f-124">updatefailed</span><span class="sxs-lookup"><span data-stu-id="0ad8f-124">updateFailed</span></span>|<span data-ttu-id="0ad8f-125">#</span><span class="sxs-lookup"><span data-stu-id="0ad8f-125">11</span></span>|<span data-ttu-id="0ad8f-126">構成マネージャーエージェントのバージョン x からバージョン y への更新に失敗しました。</span><span class="sxs-lookup"><span data-stu-id="0ad8f-126">The update from version x to version y of the configuration manager agent failed.</span></span> |
|<span data-ttu-id="0ad8f-127">communicationError</span><span class="sxs-lookup"><span data-stu-id="0ad8f-127">communicationError</span></span>|<span data-ttu-id="0ad8f-128">年</span><span class="sxs-lookup"><span data-stu-id="0ad8f-128">19</span></span>|<span data-ttu-id="0ad8f-129">構成マネージャーエージェントは、以前に構成マネージャーサービスにアクセスできましたが、現在は利用できなくなりました。</span><span class="sxs-lookup"><span data-stu-id="0ad8f-129">The configuration manager agent was able to reach the configuration manager service in the past but is now no longer able to.</span></span> |





