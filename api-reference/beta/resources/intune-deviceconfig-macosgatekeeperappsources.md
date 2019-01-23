---
title: macOSGatekeeperAppSources 列挙型
description: MacOS ゲートキーパーのアプリケーション ソースのオプションです。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 18ab6884d211faccb81e93a40ee91f742d03475f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394391"
---
# <a name="macosgatekeeperappsources-enum-type"></a><span data-ttu-id="a6ede-103">macOSGatekeeperAppSources 列挙型</span><span class="sxs-lookup"><span data-stu-id="a6ede-103">macOSGatekeeperAppSources enum type</span></span>

> <span data-ttu-id="a6ede-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a6ede-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a6ede-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a6ede-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a6ede-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a6ede-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6ede-107">MacOS ゲートキーパーのアプリケーション ソースのオプションです。</span><span class="sxs-lookup"><span data-stu-id="a6ede-107">App source options for macOS Gatekeeper.</span></span>

## <a name="members"></a><span data-ttu-id="a6ede-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="a6ede-108">Members</span></span>
|<span data-ttu-id="a6ede-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="a6ede-109">Member</span></span>|<span data-ttu-id="a6ede-110">値</span><span class="sxs-lookup"><span data-stu-id="a6ede-110">Value</span></span>|<span data-ttu-id="a6ede-111">説明</span><span class="sxs-lookup"><span data-stu-id="a6ede-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6ede-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="a6ede-112">notConfigured</span></span>|<span data-ttu-id="a6ede-113">0</span><span class="sxs-lookup"><span data-stu-id="a6ede-113">0</span></span>|<span data-ttu-id="a6ede-114">デバイスの既定値でことを目的しません。</span><span class="sxs-lookup"><span data-stu-id="a6ede-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="a6ede-115">macAppStore</span><span class="sxs-lookup"><span data-stu-id="a6ede-115">macAppStore</span></span>|<span data-ttu-id="a6ede-116">1</span><span class="sxs-lookup"><span data-stu-id="a6ede-116">1</span></span>|<span data-ttu-id="a6ede-117">Mac AppStore からのアプリのみを実行することができます。</span><span class="sxs-lookup"><span data-stu-id="a6ede-117">Only apps from the Mac AppStore can be run.</span></span>|
|<span data-ttu-id="a6ede-118">macAppStoreAndIdentifiedDevelopers</span><span class="sxs-lookup"><span data-stu-id="a6ede-118">macAppStoreAndIdentifiedDevelopers</span></span>|<span data-ttu-id="a6ede-119">2</span><span class="sxs-lookup"><span data-stu-id="a6ede-119">2</span></span>|<span data-ttu-id="a6ede-120">Mac AppStore と識別された開発者からの唯一のアプリケーションを実行することができます。</span><span class="sxs-lookup"><span data-stu-id="a6ede-120">Only apps from the Mac AppStore and identified developers can be run.</span></span>|
|<span data-ttu-id="a6ede-121">任意の場所</span><span class="sxs-lookup"><span data-stu-id="a6ede-121">anywhere</span></span>|<span data-ttu-id="a6ede-122">3</span><span class="sxs-lookup"><span data-stu-id="a6ede-122">3</span></span>|<span data-ttu-id="a6ede-123">任意の場所からアプリケーションを実行することができます。</span><span class="sxs-lookup"><span data-stu-id="a6ede-123">Apps from anywhere can be run.</span></span>|




