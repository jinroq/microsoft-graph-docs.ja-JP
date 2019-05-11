---
title: managedAppFlaggedReason 列挙型
description: ユーザーにフラグが設定された理由
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2e2e8d473ba1dad1db8cd53d990a4cd8150b5544
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940744"
---
# <a name="managedappflaggedreason-enum-type"></a><span data-ttu-id="f0edd-103">managedAppFlaggedReason 列挙型</span><span class="sxs-lookup"><span data-stu-id="f0edd-103">managedAppFlaggedReason enum type</span></span>

> <span data-ttu-id="f0edd-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f0edd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f0edd-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f0edd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0edd-106">ユーザーにフラグが設定された理由</span><span class="sxs-lookup"><span data-stu-id="f0edd-106">The reason for which a user has been flagged</span></span>

## <a name="members"></a><span data-ttu-id="f0edd-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="f0edd-107">Members</span></span>
|<span data-ttu-id="f0edd-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="f0edd-108">Member</span></span>|<span data-ttu-id="f0edd-109">値</span><span class="sxs-lookup"><span data-stu-id="f0edd-109">Value</span></span>|<span data-ttu-id="f0edd-110">説明</span><span class="sxs-lookup"><span data-stu-id="f0edd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0edd-111">none</span><span class="sxs-lookup"><span data-stu-id="f0edd-111">none</span></span>|<span data-ttu-id="f0edd-112">.0</span><span class="sxs-lookup"><span data-stu-id="f0edd-112">0</span></span>|<span data-ttu-id="f0edd-113">問題はありません。</span><span class="sxs-lookup"><span data-stu-id="f0edd-113">No issue.</span></span>|
|<span data-ttu-id="f0edd-114">rootedDevice</span><span class="sxs-lookup"><span data-stu-id="f0edd-114">rootedDevice</span></span>|<span data-ttu-id="f0edd-115">1-d</span><span class="sxs-lookup"><span data-stu-id="f0edd-115">1</span></span>|<span data-ttu-id="f0edd-116">アプリの登録は、ルート/ロック解除されたデバイス上で実行されています。</span><span class="sxs-lookup"><span data-stu-id="f0edd-116">The app registration is running on a rooted/unlocked device.</span></span>|
|<span data-ttu-id="f0edd-117">androidBootloaderUnlocked</span><span class="sxs-lookup"><span data-stu-id="f0edd-117">androidBootloaderUnlocked</span></span>|<span data-ttu-id="f0edd-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="f0edd-118">2</span></span>|<span data-ttu-id="f0edd-119">アプリの登録は、ブートローダーのロックが解除されている Android デバイス上で実行されています。</span><span class="sxs-lookup"><span data-stu-id="f0edd-119">The app registration is running on an Android device on which the bootloader is unlocked.</span></span>|
|<span data-ttu-id="f0edd-120">androidFactoryRomModified</span><span class="sxs-lookup"><span data-stu-id="f0edd-120">androidFactoryRomModified</span></span>|<span data-ttu-id="f0edd-121">1/3</span><span class="sxs-lookup"><span data-stu-id="f0edd-121">3</span></span>|<span data-ttu-id="f0edd-122">アプリの登録は、工場 ROM が変更された Android デバイス上で実行されています。</span><span class="sxs-lookup"><span data-stu-id="f0edd-122">The app registration is running on an Android device on which the factory ROM has been modified.</span></span>|




