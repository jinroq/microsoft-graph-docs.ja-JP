---
title: edgeTelemetryMode 列挙型
description: Microsoft 365 analytics に送信された参照データの種類
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c7103bd1bd3ee6869e4a6f76e8a55142e35246e5
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946666"
---
# <a name="edgetelemetrymode-enum-type"></a><span data-ttu-id="7a8b0-103">edgeTelemetryMode 列挙型</span><span class="sxs-lookup"><span data-stu-id="7a8b0-103">edgeTelemetryMode enum type</span></span>

> <span data-ttu-id="7a8b0-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7a8b0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7a8b0-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7a8b0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a8b0-106">Microsoft 365 analytics に送信された参照データの種類</span><span class="sxs-lookup"><span data-stu-id="7a8b0-106">Type of browsing data sent to Microsoft 365 analytics</span></span>

## <a name="members"></a><span data-ttu-id="7a8b0-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="7a8b0-107">Members</span></span>
|<span data-ttu-id="7a8b0-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="7a8b0-108">Member</span></span>|<span data-ttu-id="7a8b0-109">値</span><span class="sxs-lookup"><span data-stu-id="7a8b0-109">Value</span></span>|<span data-ttu-id="7a8b0-110">説明</span><span class="sxs-lookup"><span data-stu-id="7a8b0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a8b0-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="7a8b0-111">notConfigured</span></span>|<span data-ttu-id="7a8b0-112">.0</span><span class="sxs-lookup"><span data-stu-id="7a8b0-112">0</span></span>|<span data-ttu-id="7a8b0-113">既定–収集または送信されたテレメトリデータはありません。</span><span class="sxs-lookup"><span data-stu-id="7a8b0-113">Default – No telemetry data collected or sent</span></span>|
|<span data-ttu-id="7a8b0-114">イントラネット</span><span class="sxs-lookup"><span data-stu-id="7a8b0-114">intranet</span></span>|<span data-ttu-id="7a8b0-115">1-d</span><span class="sxs-lookup"><span data-stu-id="7a8b0-115">1</span></span>|<span data-ttu-id="7a8b0-116">イントラネットの履歴のみを送信できるようにする: イントラネットサイトの閲覧履歴データのみを送信する</span><span class="sxs-lookup"><span data-stu-id="7a8b0-116">Allow sending intranet history only: Only send browsing history data for intranet sites</span></span>|
|<span data-ttu-id="7a8b0-117">経由</span><span class="sxs-lookup"><span data-stu-id="7a8b0-117">internet</span></span>|<span data-ttu-id="7a8b0-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="7a8b0-118">2</span></span>|<span data-ttu-id="7a8b0-119">インターネットの送信履歴のみを許可する: インターネットサイトの閲覧履歴データのみを送信する</span><span class="sxs-lookup"><span data-stu-id="7a8b0-119">Allow sending internet history only: Only send browsing history data for internet sites</span></span>|
|<span data-ttu-id="7a8b0-120">intranetAndInternet</span><span class="sxs-lookup"><span data-stu-id="7a8b0-120">intranetAndInternet</span></span>|<span data-ttu-id="7a8b0-121">1/3</span><span class="sxs-lookup"><span data-stu-id="7a8b0-121">3</span></span>|<span data-ttu-id="7a8b0-122">イントラネットとインターネットの両方の履歴を送信できるようにする: イントラネットおよびインターネットサイトの閲覧履歴データを送信する</span><span class="sxs-lookup"><span data-stu-id="7a8b0-122">Allow sending both intranet and internet history: Send browsing history data for intranet and internet sites</span></span>|




