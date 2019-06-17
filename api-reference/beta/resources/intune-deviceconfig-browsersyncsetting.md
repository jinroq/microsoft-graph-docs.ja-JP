---
title: browserSyncSetting 列挙型
description: Microsoft Edge ブラウザーの設定の同期を許可 (未構成) または禁止 (ブロック) します。 デバイス間での同期を禁止し、ユーザーによる上書きを許可するオプション。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 014d1920dac25d5344016ff5bbd1af1ede659f4d
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34990177"
---
# <a name="browsersyncsetting-enum-type"></a><span data-ttu-id="8d322-104">browserSyncSetting 列挙型</span><span class="sxs-lookup"><span data-stu-id="8d322-104">browserSyncSetting enum type</span></span>

> <span data-ttu-id="8d322-105">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8d322-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8d322-106">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8d322-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d322-107">Microsoft Edge ブラウザーの設定の同期を許可 (未構成) または禁止 (ブロック) します。</span><span class="sxs-lookup"><span data-stu-id="8d322-107">Allow(Not Configured) or prevent(Block) the syncing of Microsoft Edge Browser settings.</span></span> <span data-ttu-id="8d322-108">デバイス間での同期を禁止し、ユーザーによる上書きを許可するオプション。</span><span class="sxs-lookup"><span data-stu-id="8d322-108">Option to prevent syncing across devices, but allow user override.</span></span>

## <a name="members"></a><span data-ttu-id="8d322-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="8d322-109">Members</span></span>
|<span data-ttu-id="8d322-110">メンバー</span><span class="sxs-lookup"><span data-stu-id="8d322-110">Member</span></span>|<span data-ttu-id="8d322-111">値</span><span class="sxs-lookup"><span data-stu-id="8d322-111">Value</span></span>|<span data-ttu-id="8d322-112">説明</span><span class="sxs-lookup"><span data-stu-id="8d322-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d322-113">notConfigured</span><span class="sxs-lookup"><span data-stu-id="8d322-113">notConfigured</span></span>|<span data-ttu-id="8d322-114">.0</span><span class="sxs-lookup"><span data-stu-id="8d322-114">0</span></span>|<span data-ttu-id="8d322-115">Default –デバイス間でのブラウザー設定の同期を許可します。</span><span class="sxs-lookup"><span data-stu-id="8d322-115">Default – Allow syncing of browser settings across devices.</span></span>|
|<span data-ttu-id="8d322-116">blockedWithUserOverride</span><span class="sxs-lookup"><span data-stu-id="8d322-116">blockedWithUserOverride</span></span>|<span data-ttu-id="8d322-117">1-d</span><span class="sxs-lookup"><span data-stu-id="8d322-117">1</span></span>|<span data-ttu-id="8d322-118">ユーザーのデバイス間でブラウザー設定を同期できないようにして、ユーザーが設定を上書きできるようにします。</span><span class="sxs-lookup"><span data-stu-id="8d322-118">Prevent syncing of browser settings across user devices, allow user override of setting.</span></span>|
|<span data-ttu-id="8d322-119">ブロック</span><span class="sxs-lookup"><span data-stu-id="8d322-119">blocked</span></span>|<span data-ttu-id="8d322-120">pbm-2</span><span class="sxs-lookup"><span data-stu-id="8d322-120">2</span></span>|<span data-ttu-id="8d322-121">ユーザーデバイス間でのブラウザー設定の同期を完全に防止します。</span><span class="sxs-lookup"><span data-stu-id="8d322-121">Absolutely prevent syncing of browser settings across user devices.</span></span>|





