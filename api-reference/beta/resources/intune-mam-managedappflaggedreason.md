---
title: managedappflaggedreason 列挙型
description: ユーザーにフラグが設定された理由
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 15942be9f9b6d8b25941f0726ff6046feeea386b
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/14/2019
ms.locfileid: "30572160"
---
# <a name="managedappflaggedreason-enum-type"></a><span data-ttu-id="731c4-103">managedappflaggedreason 列挙型</span><span class="sxs-lookup"><span data-stu-id="731c4-103">managedAppFlaggedReason enum type</span></span>

> <span data-ttu-id="731c4-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="731c4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="731c4-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="731c4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="731c4-106">ユーザーにフラグが設定された理由</span><span class="sxs-lookup"><span data-stu-id="731c4-106">The reason for which a user has been flagged</span></span>

## <a name="members"></a><span data-ttu-id="731c4-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="731c4-107">Members</span></span>
|<span data-ttu-id="731c4-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="731c4-108">Member</span></span>|<span data-ttu-id="731c4-109">値</span><span class="sxs-lookup"><span data-stu-id="731c4-109">Value</span></span>|<span data-ttu-id="731c4-110">説明</span><span class="sxs-lookup"><span data-stu-id="731c4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="731c4-111">なし</span><span class="sxs-lookup"><span data-stu-id="731c4-111">none</span></span>|<span data-ttu-id="731c4-112">.0</span><span class="sxs-lookup"><span data-stu-id="731c4-112">0</span></span>|<span data-ttu-id="731c4-113">問題はありません。</span><span class="sxs-lookup"><span data-stu-id="731c4-113">No issue.</span></span>|
|<span data-ttu-id="731c4-114">rootedDevice</span><span class="sxs-lookup"><span data-stu-id="731c4-114">rootedDevice</span></span>|<span data-ttu-id="731c4-115">1</span><span class="sxs-lookup"><span data-stu-id="731c4-115">1</span></span>|<span data-ttu-id="731c4-116">アプリの登録は、ルート/ロック解除されたデバイス上で実行されています。</span><span class="sxs-lookup"><span data-stu-id="731c4-116">The app registration is running on a rooted/unlocked device.</span></span>|
|<span data-ttu-id="731c4-117">androidBootloaderUnlocked</span><span class="sxs-lookup"><span data-stu-id="731c4-117">androidBootloaderUnlocked</span></span>|<span data-ttu-id="731c4-118">2</span><span class="sxs-lookup"><span data-stu-id="731c4-118">2</span></span>|<span data-ttu-id="731c4-119">アプリの登録は、ブートローダーのロックが解除されている Android デバイス上で実行されています。</span><span class="sxs-lookup"><span data-stu-id="731c4-119">The app registration is running on an Android device on which the bootloader is unlocked.</span></span>|
|<span data-ttu-id="731c4-120">androidFactoryRomModified</span><span class="sxs-lookup"><span data-stu-id="731c4-120">androidFactoryRomModified</span></span>|<span data-ttu-id="731c4-121">1/3</span><span class="sxs-lookup"><span data-stu-id="731c4-121">3</span></span>|<span data-ttu-id="731c4-122">アプリの登録は、工場 ROM が変更された Android デバイス上で実行されています。</span><span class="sxs-lookup"><span data-stu-id="731c4-122">The app registration is running on an Android device on which the factory ROM has been modified.</span></span>|




