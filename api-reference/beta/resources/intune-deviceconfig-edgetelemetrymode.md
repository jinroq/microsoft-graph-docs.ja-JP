---
title: edgeTelemetryMode 列挙型
description: Microsoft 365 分析機能に送信されるデータの参照の種類
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 81d429f7629a5d6a6f2593785605902065d9f1c7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430416"
---
# <a name="edgetelemetrymode-enum-type"></a><span data-ttu-id="274c3-103">edgeTelemetryMode 列挙型</span><span class="sxs-lookup"><span data-stu-id="274c3-103">edgeTelemetryMode enum type</span></span>

> <span data-ttu-id="274c3-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="274c3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="274c3-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="274c3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="274c3-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="274c3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="274c3-107">Microsoft 365 分析機能に送信されるデータの参照の種類</span><span class="sxs-lookup"><span data-stu-id="274c3-107">Type of browsing data sent to Microsoft 365 analytics</span></span>

## <a name="members"></a><span data-ttu-id="274c3-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="274c3-108">Members</span></span>
|<span data-ttu-id="274c3-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="274c3-109">Member</span></span>|<span data-ttu-id="274c3-110">値</span><span class="sxs-lookup"><span data-stu-id="274c3-110">Value</span></span>|<span data-ttu-id="274c3-111">説明</span><span class="sxs-lookup"><span data-stu-id="274c3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="274c3-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="274c3-112">notConfigured</span></span>|<span data-ttu-id="274c3-113">0</span><span class="sxs-lookup"><span data-stu-id="274c3-113">0</span></span>|<span data-ttu-id="274c3-114">既定: 遠隔測定データを収集または送信</span><span class="sxs-lookup"><span data-stu-id="274c3-114">Default – No telemetry data collected or sent</span></span>|
|<span data-ttu-id="274c3-115">イントラネット</span><span class="sxs-lookup"><span data-stu-id="274c3-115">intranet</span></span>|<span data-ttu-id="274c3-116">1</span><span class="sxs-lookup"><span data-stu-id="274c3-116">1</span></span>|<span data-ttu-id="274c3-117">イントラネットの履歴のみを送信することを許可する: イントラネットのサイトの履歴データを参照するだけの送信</span><span class="sxs-lookup"><span data-stu-id="274c3-117">Allow sending intranet history only: Only send browsing history data for intranet sites</span></span>|
|<span data-ttu-id="274c3-118">internet</span><span class="sxs-lookup"><span data-stu-id="274c3-118">internet</span></span>|<span data-ttu-id="274c3-119">2</span><span class="sxs-lookup"><span data-stu-id="274c3-119">2</span></span>|<span data-ttu-id="274c3-120">インターネットの履歴のみを送信することを許可する: インターネット サイトの履歴データを参照するだけの送信</span><span class="sxs-lookup"><span data-stu-id="274c3-120">Allow sending internet history only: Only send browsing history data for internet sites</span></span>|
|<span data-ttu-id="274c3-121">intranetAndInternet</span><span class="sxs-lookup"><span data-stu-id="274c3-121">intranetAndInternet</span></span>|<span data-ttu-id="274c3-122">3</span><span class="sxs-lookup"><span data-stu-id="274c3-122">3</span></span>|<span data-ttu-id="274c3-123">イントラネットとインターネットの両方の履歴を送信することを許可する: イントラネットとインターネットのサイトの履歴データを参照する送信</span><span class="sxs-lookup"><span data-stu-id="274c3-123">Allow sending both intranet and internet history: Send browsing history data for intranet and internet sites</span></span>|




