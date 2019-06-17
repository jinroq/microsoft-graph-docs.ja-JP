---
title: win32LobAppPowerShellScriptDetectionType 列挙型
description: サポートされているすべての Powershell スクリプトの出力検出の種類が含まれます。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 894dc61909f17244e3325675e198520cae5657ab
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34987335"
---
# <a name="win32lobapppowershellscriptdetectiontype-enum-type"></a><span data-ttu-id="45f2c-103">win32LobAppPowerShellScriptDetectionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="45f2c-103">win32LobAppPowerShellScriptDetectionType enum type</span></span>

> <span data-ttu-id="45f2c-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="45f2c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="45f2c-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="45f2c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45f2c-106">サポートされているすべての Powershell スクリプトの出力検出の種類が含まれます。</span><span class="sxs-lookup"><span data-stu-id="45f2c-106">Contains all supported Powershell Script output detection type.</span></span>

## <a name="members"></a><span data-ttu-id="45f2c-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="45f2c-107">Members</span></span>
|<span data-ttu-id="45f2c-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="45f2c-108">Member</span></span>|<span data-ttu-id="45f2c-109">値</span><span class="sxs-lookup"><span data-stu-id="45f2c-109">Value</span></span>|<span data-ttu-id="45f2c-110">説明</span><span class="sxs-lookup"><span data-stu-id="45f2c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45f2c-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="45f2c-111">notConfigured</span></span>|<span data-ttu-id="45f2c-112">.0</span><span class="sxs-lookup"><span data-stu-id="45f2c-112">0</span></span>|<span data-ttu-id="45f2c-113">構成されていません。</span><span class="sxs-lookup"><span data-stu-id="45f2c-113">Not configured.</span></span>|
|<span data-ttu-id="45f2c-114">string</span><span class="sxs-lookup"><span data-stu-id="45f2c-114">string</span></span>|<span data-ttu-id="45f2c-115">1-d</span><span class="sxs-lookup"><span data-stu-id="45f2c-115">1</span></span>|<span data-ttu-id="45f2c-116">出力データの種類は文字列です。</span><span class="sxs-lookup"><span data-stu-id="45f2c-116">Output data type is string.</span></span>|
|<span data-ttu-id="45f2c-117">dateTime</span><span class="sxs-lookup"><span data-stu-id="45f2c-117">dateTime</span></span>|<span data-ttu-id="45f2c-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="45f2c-118">2</span></span>|<span data-ttu-id="45f2c-119">出力データの種類は、日付/時刻です。</span><span class="sxs-lookup"><span data-stu-id="45f2c-119">Output data type is date time.</span></span>|
|<span data-ttu-id="45f2c-120">整数</span><span class="sxs-lookup"><span data-stu-id="45f2c-120">integer</span></span>|<span data-ttu-id="45f2c-121">1/3</span><span class="sxs-lookup"><span data-stu-id="45f2c-121">3</span></span>|<span data-ttu-id="45f2c-122">出力データの種類は整数です。</span><span class="sxs-lookup"><span data-stu-id="45f2c-122">Output data type is integer.</span></span>|
|<span data-ttu-id="45f2c-123">浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="45f2c-123">float</span></span>|<span data-ttu-id="45f2c-124">2/4</span><span class="sxs-lookup"><span data-stu-id="45f2c-124">4</span></span>|<span data-ttu-id="45f2c-125">出力データの種類は float です。</span><span class="sxs-lookup"><span data-stu-id="45f2c-125">Output data type is float.</span></span>|
|<span data-ttu-id="45f2c-126">バージョン</span><span class="sxs-lookup"><span data-stu-id="45f2c-126">version</span></span>|<span data-ttu-id="45f2c-127">5</span><span class="sxs-lookup"><span data-stu-id="45f2c-127">5</span></span>|<span data-ttu-id="45f2c-128">出力データの種類はバージョンです。</span><span class="sxs-lookup"><span data-stu-id="45f2c-128">Output data type is version.</span></span>|
|<span data-ttu-id="45f2c-129">ブール値</span><span class="sxs-lookup"><span data-stu-id="45f2c-129">boolean</span></span>|<span data-ttu-id="45f2c-130">シックス</span><span class="sxs-lookup"><span data-stu-id="45f2c-130">6</span></span>|<span data-ttu-id="45f2c-131">Output データ型はブール値です。</span><span class="sxs-lookup"><span data-stu-id="45f2c-131">Output data type is boolean.</span></span>|





