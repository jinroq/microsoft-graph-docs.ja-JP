---
title: edgeTelemetryMode 列挙型
description: Microsoft 365 analytics に送信された参照データの種類
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: fa6ea5a2bf187a753705b369f3f8a2558860c3eb
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36357272"
---
# <a name="edgetelemetrymode-enum-type"></a><span data-ttu-id="ec80d-103">edgeTelemetryMode 列挙型</span><span class="sxs-lookup"><span data-stu-id="ec80d-103">edgeTelemetryMode enum type</span></span>

> <span data-ttu-id="ec80d-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ec80d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ec80d-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ec80d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ec80d-106">Microsoft 365 analytics に送信された参照データの種類</span><span class="sxs-lookup"><span data-stu-id="ec80d-106">Type of browsing data sent to Microsoft 365 analytics</span></span>

## <a name="members"></a><span data-ttu-id="ec80d-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="ec80d-107">Members</span></span>
|<span data-ttu-id="ec80d-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="ec80d-108">Member</span></span>|<span data-ttu-id="ec80d-109">値</span><span class="sxs-lookup"><span data-stu-id="ec80d-109">Value</span></span>|<span data-ttu-id="ec80d-110">説明</span><span class="sxs-lookup"><span data-stu-id="ec80d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec80d-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="ec80d-111">notConfigured</span></span>|<span data-ttu-id="ec80d-112">.0</span><span class="sxs-lookup"><span data-stu-id="ec80d-112">0</span></span>|<span data-ttu-id="ec80d-113">既定–収集または送信されたテレメトリデータはありません。</span><span class="sxs-lookup"><span data-stu-id="ec80d-113">Default – No telemetry data collected or sent</span></span>|
|<span data-ttu-id="ec80d-114">イントラネット</span><span class="sxs-lookup"><span data-stu-id="ec80d-114">intranet</span></span>|<span data-ttu-id="ec80d-115">1-d</span><span class="sxs-lookup"><span data-stu-id="ec80d-115">1</span></span>|<span data-ttu-id="ec80d-116">イントラネットの履歴のみを送信できるようにする: イントラネットサイトの閲覧履歴データのみを送信する</span><span class="sxs-lookup"><span data-stu-id="ec80d-116">Allow sending intranet history only: Only send browsing history data for intranet sites</span></span>|
|<span data-ttu-id="ec80d-117">経由</span><span class="sxs-lookup"><span data-stu-id="ec80d-117">internet</span></span>|<span data-ttu-id="ec80d-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="ec80d-118">2</span></span>|<span data-ttu-id="ec80d-119">インターネットの送信履歴のみを許可する: インターネットサイトの閲覧履歴データのみを送信する</span><span class="sxs-lookup"><span data-stu-id="ec80d-119">Allow sending internet history only: Only send browsing history data for internet sites</span></span>|
|<span data-ttu-id="ec80d-120">intranetAndInternet</span><span class="sxs-lookup"><span data-stu-id="ec80d-120">intranetAndInternet</span></span>|<span data-ttu-id="ec80d-121">1/3</span><span class="sxs-lookup"><span data-stu-id="ec80d-121">3</span></span>|<span data-ttu-id="ec80d-122">イントラネットとインターネットの両方の履歴を送信できるようにする: イントラネットおよびインターネットサイトの閲覧履歴データを送信する</span><span class="sxs-lookup"><span data-stu-id="ec80d-122">Allow sending both intranet and internet history: Send browsing history data for intranet and internet sites</span></span>|



