---
title: browserSyncSetting 列挙型
description: Allow(Not Configured) または prevent(Block) がマイクロソフトのエッジのブラウザーの設定の同期します。 防止するオプションはデバイス間で同期しますが、ユーザーのオーバーライドを許可します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8dce2b82b1eea5e4b06ed0f6949ba6a403b073a8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431590"
---
# <a name="browsersyncsetting-enum-type"></a><span data-ttu-id="2dc91-104">browserSyncSetting 列挙型</span><span class="sxs-lookup"><span data-stu-id="2dc91-104">browserSyncSetting enum type</span></span>

> <span data-ttu-id="2dc91-105">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2dc91-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2dc91-106">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2dc91-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2dc91-107">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2dc91-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2dc91-108">Allow(Not Configured) または prevent(Block) がマイクロソフトのエッジのブラウザーの設定の同期します。</span><span class="sxs-lookup"><span data-stu-id="2dc91-108">Allow(Not Configured) or prevent(Block) the syncing of Microsoft Edge Browser settings.</span></span> <span data-ttu-id="2dc91-109">防止するオプションはデバイス間で同期しますが、ユーザーのオーバーライドを許可します。</span><span class="sxs-lookup"><span data-stu-id="2dc91-109">Option to prevent syncing across devices, but allow user override.</span></span>

## <a name="members"></a><span data-ttu-id="2dc91-110">メンバー</span><span class="sxs-lookup"><span data-stu-id="2dc91-110">Members</span></span>
|<span data-ttu-id="2dc91-111">メンバー</span><span class="sxs-lookup"><span data-stu-id="2dc91-111">Member</span></span>|<span data-ttu-id="2dc91-112">値</span><span class="sxs-lookup"><span data-stu-id="2dc91-112">Value</span></span>|<span data-ttu-id="2dc91-113">説明</span><span class="sxs-lookup"><span data-stu-id="2dc91-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2dc91-114">notConfigured</span><span class="sxs-lookup"><span data-stu-id="2dc91-114">notConfigured</span></span>|<span data-ttu-id="2dc91-115">0</span><span class="sxs-lookup"><span data-stu-id="2dc91-115">0</span></span>|<span data-ttu-id="2dc91-116">既定 – 複数のデバイスのブラウザーの設定の同期を許可します。</span><span class="sxs-lookup"><span data-stu-id="2dc91-116">Default – Allow syncing of browser settings across devices.</span></span>|
|<span data-ttu-id="2dc91-117">blockedWithUserOverride</span><span class="sxs-lookup"><span data-stu-id="2dc91-117">blockedWithUserOverride</span></span>|<span data-ttu-id="2dc91-118">1</span><span class="sxs-lookup"><span data-stu-id="2dc91-118">1</span></span>|<span data-ttu-id="2dc91-119">複数のユーザーのデバイスのブラウザーの設定の同期を防ぐため、設定のユーザーの上書きを許可します。</span><span class="sxs-lookup"><span data-stu-id="2dc91-119">Prevent syncing of browser settings across user devices, allow user override of setting.</span></span>|
|<span data-ttu-id="2dc91-120">ブロック</span><span class="sxs-lookup"><span data-stu-id="2dc91-120">blocked</span></span>|<span data-ttu-id="2dc91-121">2</span><span class="sxs-lookup"><span data-stu-id="2dc91-121">2</span></span>|<span data-ttu-id="2dc91-122">絶対に複数のユーザーのデバイスのブラウザーの設定の同期を防ぐためです。</span><span class="sxs-lookup"><span data-stu-id="2dc91-122">Absolutely prevent syncing of browser settings across user devices.</span></span>|




