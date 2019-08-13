---
title: managedAppFlaggedReason 列挙型
description: ユーザーにフラグが設定された理由
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 7aedda5d89d41ba936651c10d81ceeb33dfe603a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36332128"
---
# <a name="managedappflaggedreason-enum-type"></a><span data-ttu-id="caad1-103">managedAppFlaggedReason 列挙型</span><span class="sxs-lookup"><span data-stu-id="caad1-103">managedAppFlaggedReason enum type</span></span>

> <span data-ttu-id="caad1-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="caad1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="caad1-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="caad1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="caad1-106">ユーザーにフラグが設定された理由</span><span class="sxs-lookup"><span data-stu-id="caad1-106">The reason for which a user has been flagged</span></span>

## <a name="members"></a><span data-ttu-id="caad1-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="caad1-107">Members</span></span>
|<span data-ttu-id="caad1-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="caad1-108">Member</span></span>|<span data-ttu-id="caad1-109">値</span><span class="sxs-lookup"><span data-stu-id="caad1-109">Value</span></span>|<span data-ttu-id="caad1-110">説明</span><span class="sxs-lookup"><span data-stu-id="caad1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="caad1-111">none</span><span class="sxs-lookup"><span data-stu-id="caad1-111">none</span></span>|<span data-ttu-id="caad1-112">.0</span><span class="sxs-lookup"><span data-stu-id="caad1-112">0</span></span>|<span data-ttu-id="caad1-113">問題はありません。</span><span class="sxs-lookup"><span data-stu-id="caad1-113">No issue.</span></span>|
|<span data-ttu-id="caad1-114">rootedDevice</span><span class="sxs-lookup"><span data-stu-id="caad1-114">rootedDevice</span></span>|<span data-ttu-id="caad1-115">1-d</span><span class="sxs-lookup"><span data-stu-id="caad1-115">1</span></span>|<span data-ttu-id="caad1-116">アプリの登録は、ルート/ロック解除されたデバイス上で実行されています。</span><span class="sxs-lookup"><span data-stu-id="caad1-116">The app registration is running on a rooted/unlocked device.</span></span>|
|<span data-ttu-id="caad1-117">androidBootloaderUnlocked</span><span class="sxs-lookup"><span data-stu-id="caad1-117">androidBootloaderUnlocked</span></span>|<span data-ttu-id="caad1-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="caad1-118">2</span></span>|<span data-ttu-id="caad1-119">アプリの登録は、ブートローダーのロックが解除されている Android デバイス上で実行されています。</span><span class="sxs-lookup"><span data-stu-id="caad1-119">The app registration is running on an Android device on which the bootloader is unlocked.</span></span>|
|<span data-ttu-id="caad1-120">androidFactoryRomModified</span><span class="sxs-lookup"><span data-stu-id="caad1-120">androidFactoryRomModified</span></span>|<span data-ttu-id="caad1-121">1/3</span><span class="sxs-lookup"><span data-stu-id="caad1-121">3</span></span>|<span data-ttu-id="caad1-122">アプリの登録は、工場 ROM が変更された Android デバイス上で実行されています。</span><span class="sxs-lookup"><span data-stu-id="caad1-122">The app registration is running on an Android device on which the factory ROM has been modified.</span></span>|



