---
title: browsersyncsetting 列挙型
description: Microsoft Edge ブラウザーの設定の同期を許可 (未構成) または禁止 (ブロック) します。 デバイス間での同期を禁止し、ユーザーによる上書きを許可するオプション。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f08031e970f56c071a4dd01af0542bd56924edd5
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31789746"
---
# <a name="browsersyncsetting-enum-type"></a><span data-ttu-id="ba9c8-104">browsersyncsetting 列挙型</span><span class="sxs-lookup"><span data-stu-id="ba9c8-104">browserSyncSetting enum type</span></span>

> <span data-ttu-id="ba9c8-105">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ba9c8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ba9c8-106">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ba9c8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba9c8-107">Microsoft Edge ブラウザーの設定の同期を許可 (未構成) または禁止 (ブロック) します。</span><span class="sxs-lookup"><span data-stu-id="ba9c8-107">Allow(Not Configured) or prevent(Block) the syncing of Microsoft Edge Browser settings.</span></span> <span data-ttu-id="ba9c8-108">デバイス間での同期を禁止し、ユーザーによる上書きを許可するオプション。</span><span class="sxs-lookup"><span data-stu-id="ba9c8-108">Option to prevent syncing across devices, but allow user override.</span></span>

## <a name="members"></a><span data-ttu-id="ba9c8-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="ba9c8-109">Members</span></span>
|<span data-ttu-id="ba9c8-110">メンバー</span><span class="sxs-lookup"><span data-stu-id="ba9c8-110">Member</span></span>|<span data-ttu-id="ba9c8-111">値</span><span class="sxs-lookup"><span data-stu-id="ba9c8-111">Value</span></span>|<span data-ttu-id="ba9c8-112">説明</span><span class="sxs-lookup"><span data-stu-id="ba9c8-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba9c8-113">notConfigured</span><span class="sxs-lookup"><span data-stu-id="ba9c8-113">notConfigured</span></span>|<span data-ttu-id="ba9c8-114">.0</span><span class="sxs-lookup"><span data-stu-id="ba9c8-114">0</span></span>|<span data-ttu-id="ba9c8-115">Default –デバイス間でのブラウザー設定の同期を許可します。</span><span class="sxs-lookup"><span data-stu-id="ba9c8-115">Default – Allow syncing of browser settings across devices.</span></span>|
|<span data-ttu-id="ba9c8-116">blockedWithUserOverride</span><span class="sxs-lookup"><span data-stu-id="ba9c8-116">blockedWithUserOverride</span></span>|<span data-ttu-id="ba9c8-117">1-d</span><span class="sxs-lookup"><span data-stu-id="ba9c8-117">1</span></span>|<span data-ttu-id="ba9c8-118">ユーザーのデバイス間でブラウザー設定を同期できないようにして、ユーザーが設定を上書きできるようにします。</span><span class="sxs-lookup"><span data-stu-id="ba9c8-118">Prevent syncing of browser settings across user devices, allow user override of setting.</span></span>|
|<span data-ttu-id="ba9c8-119">ブロック</span><span class="sxs-lookup"><span data-stu-id="ba9c8-119">blocked</span></span>|<span data-ttu-id="ba9c8-120">pbm-2</span><span class="sxs-lookup"><span data-stu-id="ba9c8-120">2</span></span>|<span data-ttu-id="ba9c8-121">ユーザーデバイス間でのブラウザー設定の同期を完全に防止します。</span><span class="sxs-lookup"><span data-stu-id="ba9c8-121">Absolutely prevent syncing of browser settings across user devices.</span></span>|





