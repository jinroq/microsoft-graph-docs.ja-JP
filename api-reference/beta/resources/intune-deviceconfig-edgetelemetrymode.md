---
title: edgeTelemetryMode 列挙型
description: Microsoft 365 analytics に送信された参照データの種類
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1d671849e34d27403450ae6324b824a92ae9d9b4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566039"
---
# <a name="edgetelemetrymode-enum-type"></a><span data-ttu-id="19740-103">edgeTelemetryMode 列挙型</span><span class="sxs-lookup"><span data-stu-id="19740-103">edgeTelemetryMode enum type</span></span>

> <span data-ttu-id="19740-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="19740-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="19740-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="19740-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19740-106">Microsoft 365 analytics に送信された参照データの種類</span><span class="sxs-lookup"><span data-stu-id="19740-106">Type of browsing data sent to Microsoft 365 analytics</span></span>

## <a name="members"></a><span data-ttu-id="19740-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="19740-107">Members</span></span>
|<span data-ttu-id="19740-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="19740-108">Member</span></span>|<span data-ttu-id="19740-109">値</span><span class="sxs-lookup"><span data-stu-id="19740-109">Value</span></span>|<span data-ttu-id="19740-110">説明</span><span class="sxs-lookup"><span data-stu-id="19740-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19740-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="19740-111">notConfigured</span></span>|<span data-ttu-id="19740-112">.0</span><span class="sxs-lookup"><span data-stu-id="19740-112">0</span></span>|<span data-ttu-id="19740-113">既定–収集または送信されたテレメトリデータはありません。</span><span class="sxs-lookup"><span data-stu-id="19740-113">Default – No telemetry data collected or sent</span></span>|
|<span data-ttu-id="19740-114">イントラネット</span><span class="sxs-lookup"><span data-stu-id="19740-114">intranet</span></span>|<span data-ttu-id="19740-115">1 </span><span class="sxs-lookup"><span data-stu-id="19740-115">1</span></span>|<span data-ttu-id="19740-116">イントラネットの履歴のみを送信できるようにする: イントラネットサイトの閲覧履歴データのみを送信する</span><span class="sxs-lookup"><span data-stu-id="19740-116">Allow sending intranet history only: Only send browsing history data for intranet sites</span></span>|
|<span data-ttu-id="19740-117">経由</span><span class="sxs-lookup"><span data-stu-id="19740-117">internet</span></span>|<span data-ttu-id="19740-118">2 </span><span class="sxs-lookup"><span data-stu-id="19740-118">2</span></span>|<span data-ttu-id="19740-119">インターネットの送信履歴のみを許可する: インターネットサイトの閲覧履歴データのみを送信する</span><span class="sxs-lookup"><span data-stu-id="19740-119">Allow sending internet history only: Only send browsing history data for internet sites</span></span>|
|<span data-ttu-id="19740-120">intranetandinternet</span><span class="sxs-lookup"><span data-stu-id="19740-120">intranetAndInternet</span></span>|<span data-ttu-id="19740-121">3 </span><span class="sxs-lookup"><span data-stu-id="19740-121">3</span></span>|<span data-ttu-id="19740-122">イントラネットとインターネットの両方の履歴を送信できるようにする: イントラネットおよびインターネットサイトの閲覧履歴データを送信する</span><span class="sxs-lookup"><span data-stu-id="19740-122">Allow sending both intranet and internet history: Send browsing history data for intranet and internet sites</span></span>|





