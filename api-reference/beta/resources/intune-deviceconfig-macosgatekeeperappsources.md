---
title: macOSGatekeeperAppSources 列挙型
description: MacOS ゲートキーパーのアプリケーション ソースのオプションです。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 6c784dba6a79b6a9d406e3632d2ac4beaf2a47ba
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888369"
---
# <a name="macosgatekeeperappsources-enum-type"></a><span data-ttu-id="f2172-103">macOSGatekeeperAppSources 列挙型</span><span class="sxs-lookup"><span data-stu-id="f2172-103">macOSGatekeeperAppSources enum type</span></span>

> <span data-ttu-id="f2172-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f2172-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f2172-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f2172-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f2172-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f2172-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f2172-107">MacOS ゲートキーパーのアプリケーション ソースのオプションです。</span><span class="sxs-lookup"><span data-stu-id="f2172-107">App source options for macOS Gatekeeper.</span></span>
## <a name="members"></a><span data-ttu-id="f2172-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="f2172-108">Members</span></span>
|<span data-ttu-id="f2172-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="f2172-109">Member</span></span>|<span data-ttu-id="f2172-110">値</span><span class="sxs-lookup"><span data-stu-id="f2172-110">Value</span></span>|<span data-ttu-id="f2172-111">説明</span><span class="sxs-lookup"><span data-stu-id="f2172-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2172-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="f2172-112">notConfigured</span></span>|<span data-ttu-id="f2172-113">0</span><span class="sxs-lookup"><span data-stu-id="f2172-113">0</span></span>|<span data-ttu-id="f2172-114">デバイスの既定値でことを目的しません。</span><span class="sxs-lookup"><span data-stu-id="f2172-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="f2172-115">macAppStore</span><span class="sxs-lookup"><span data-stu-id="f2172-115">macAppStore</span></span>|<span data-ttu-id="f2172-116">1</span><span class="sxs-lookup"><span data-stu-id="f2172-116">1</span></span>|<span data-ttu-id="f2172-117">Mac AppStore からのアプリのみを実行することができます。</span><span class="sxs-lookup"><span data-stu-id="f2172-117">Only apps from the Mac AppStore can be run.</span></span>|
|<span data-ttu-id="f2172-118">macAppStoreAndIdentifiedDevelopers</span><span class="sxs-lookup"><span data-stu-id="f2172-118">macAppStoreAndIdentifiedDevelopers</span></span>|<span data-ttu-id="f2172-119">2</span><span class="sxs-lookup"><span data-stu-id="f2172-119">2</span></span>|<span data-ttu-id="f2172-120">Mac AppStore と識別された開発者からの唯一のアプリケーションを実行することができます。</span><span class="sxs-lookup"><span data-stu-id="f2172-120">Only apps from the Mac AppStore and identified developers can be run.</span></span>|
|<span data-ttu-id="f2172-121">任意の場所</span><span class="sxs-lookup"><span data-stu-id="f2172-121">anywhere</span></span>|<span data-ttu-id="f2172-122">3</span><span class="sxs-lookup"><span data-stu-id="f2172-122">3</span></span>|<span data-ttu-id="f2172-123">任意の場所からアプリケーションを実行することができます。</span><span class="sxs-lookup"><span data-stu-id="f2172-123">Apps from anywhere can be run.</span></span>|





