---
title: win32LobAppPowerShellScriptDetectionType 列挙型
description: サポートされているすべての Powershell スクリプトの出力検出の種類が含まれます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4dc45a3b7ec8fe2732a89022fd3c74c0959bbc1c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534536"
---
# <a name="win32lobapppowershellscriptdetectiontype-enum-type"></a><span data-ttu-id="a8b3e-103">win32LobAppPowerShellScriptDetectionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="a8b3e-103">win32LobAppPowerShellScriptDetectionType enum type</span></span>

> <span data-ttu-id="a8b3e-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a8b3e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a8b3e-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a8b3e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8b3e-106">サポートされているすべての Powershell スクリプトの出力検出の種類が含まれます。</span><span class="sxs-lookup"><span data-stu-id="a8b3e-106">Contains all supported Powershell Script output detection type.</span></span>

## <a name="members"></a><span data-ttu-id="a8b3e-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="a8b3e-107">Members</span></span>
|<span data-ttu-id="a8b3e-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="a8b3e-108">Member</span></span>|<span data-ttu-id="a8b3e-109">値</span><span class="sxs-lookup"><span data-stu-id="a8b3e-109">Value</span></span>|<span data-ttu-id="a8b3e-110">説明</span><span class="sxs-lookup"><span data-stu-id="a8b3e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8b3e-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="a8b3e-111">notConfigured</span></span>|<span data-ttu-id="a8b3e-112">.0</span><span class="sxs-lookup"><span data-stu-id="a8b3e-112">0</span></span>|<span data-ttu-id="a8b3e-113">構成されていません。</span><span class="sxs-lookup"><span data-stu-id="a8b3e-113">Not configured.</span></span>|
|<span data-ttu-id="a8b3e-114">string</span><span class="sxs-lookup"><span data-stu-id="a8b3e-114">string</span></span>|<span data-ttu-id="a8b3e-115">1 </span><span class="sxs-lookup"><span data-stu-id="a8b3e-115">1</span></span>|<span data-ttu-id="a8b3e-116">出力データの種類は文字列です。</span><span class="sxs-lookup"><span data-stu-id="a8b3e-116">Output data type is string.</span></span>|
|<span data-ttu-id="a8b3e-117">dateTime</span><span class="sxs-lookup"><span data-stu-id="a8b3e-117">dateTime</span></span>|<span data-ttu-id="a8b3e-118">2 </span><span class="sxs-lookup"><span data-stu-id="a8b3e-118">2</span></span>|<span data-ttu-id="a8b3e-119">出力データの種類は、日付/時刻です。</span><span class="sxs-lookup"><span data-stu-id="a8b3e-119">Output data type is date time.</span></span>|
|<span data-ttu-id="a8b3e-120">整数</span><span class="sxs-lookup"><span data-stu-id="a8b3e-120">integer</span></span>|<span data-ttu-id="a8b3e-121">3 </span><span class="sxs-lookup"><span data-stu-id="a8b3e-121">3</span></span>|<span data-ttu-id="a8b3e-122">出力データの種類は整数です。</span><span class="sxs-lookup"><span data-stu-id="a8b3e-122">Output data type is integer.</span></span>|
|<span data-ttu-id="a8b3e-123">浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="a8b3e-123">float</span></span>|<span data-ttu-id="a8b3e-124">4 </span><span class="sxs-lookup"><span data-stu-id="a8b3e-124">4</span></span>|<span data-ttu-id="a8b3e-125">出力データの種類は float です。</span><span class="sxs-lookup"><span data-stu-id="a8b3e-125">Output data type is float.</span></span>|
|<span data-ttu-id="a8b3e-126">バージョン</span><span class="sxs-lookup"><span data-stu-id="a8b3e-126">version</span></span>|<span data-ttu-id="a8b3e-127">5 </span><span class="sxs-lookup"><span data-stu-id="a8b3e-127">5</span></span>|<span data-ttu-id="a8b3e-128">出力データの種類はバージョンです。</span><span class="sxs-lookup"><span data-stu-id="a8b3e-128">Output data type is version.</span></span>|
|<span data-ttu-id="a8b3e-129">ブール値</span><span class="sxs-lookup"><span data-stu-id="a8b3e-129">boolean</span></span>|<span data-ttu-id="a8b3e-130">6 </span><span class="sxs-lookup"><span data-stu-id="a8b3e-130">6</span></span>|<span data-ttu-id="a8b3e-131">Output データ型はブール値です。</span><span class="sxs-lookup"><span data-stu-id="a8b3e-131">Output data type is boolean.</span></span>|





