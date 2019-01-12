---
title: macOSGatekeeperAppSources 列挙型
description: MacOS ゲートキーパーのアプリケーション ソースのオプションです。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5c2c1d553408b7269a53f9fc3500493a44bc3645
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27918115"
---
# <a name="macosgatekeeperappsources-enum-type"></a><span data-ttu-id="94937-103">macOSGatekeeperAppSources 列挙型</span><span class="sxs-lookup"><span data-stu-id="94937-103">macOSGatekeeperAppSources enum type</span></span>

> <span data-ttu-id="94937-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="94937-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="94937-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="94937-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="94937-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="94937-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="94937-107">MacOS ゲートキーパーのアプリケーション ソースのオプションです。</span><span class="sxs-lookup"><span data-stu-id="94937-107">App source options for macOS Gatekeeper.</span></span>
## <a name="members"></a><span data-ttu-id="94937-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="94937-108">Members</span></span>
|<span data-ttu-id="94937-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="94937-109">Member</span></span>|<span data-ttu-id="94937-110">値</span><span class="sxs-lookup"><span data-stu-id="94937-110">Value</span></span>|<span data-ttu-id="94937-111">説明</span><span class="sxs-lookup"><span data-stu-id="94937-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94937-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="94937-112">notConfigured</span></span>|<span data-ttu-id="94937-113">0</span><span class="sxs-lookup"><span data-stu-id="94937-113">0</span></span>|<span data-ttu-id="94937-114">デバイスの既定値でことを目的しません。</span><span class="sxs-lookup"><span data-stu-id="94937-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="94937-115">macAppStore</span><span class="sxs-lookup"><span data-stu-id="94937-115">macAppStore</span></span>|<span data-ttu-id="94937-116">1</span><span class="sxs-lookup"><span data-stu-id="94937-116">1</span></span>|<span data-ttu-id="94937-117">Mac AppStore からのアプリのみを実行することができます。</span><span class="sxs-lookup"><span data-stu-id="94937-117">Only apps from the Mac AppStore can be run.</span></span>|
|<span data-ttu-id="94937-118">macAppStoreAndIdentifiedDevelopers</span><span class="sxs-lookup"><span data-stu-id="94937-118">macAppStoreAndIdentifiedDevelopers</span></span>|<span data-ttu-id="94937-119">2</span><span class="sxs-lookup"><span data-stu-id="94937-119">2</span></span>|<span data-ttu-id="94937-120">Mac AppStore と識別された開発者からの唯一のアプリケーションを実行することができます。</span><span class="sxs-lookup"><span data-stu-id="94937-120">Only apps from the Mac AppStore and identified developers can be run.</span></span>|
|<span data-ttu-id="94937-121">任意の場所</span><span class="sxs-lookup"><span data-stu-id="94937-121">anywhere</span></span>|<span data-ttu-id="94937-122">3</span><span class="sxs-lookup"><span data-stu-id="94937-122">3</span></span>|<span data-ttu-id="94937-123">任意の場所からアプリケーションを実行することができます。</span><span class="sxs-lookup"><span data-stu-id="94937-123">Apps from anywhere can be run.</span></span>|





