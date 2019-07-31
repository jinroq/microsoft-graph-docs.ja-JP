---
title: browserSyncSetting 列挙型
description: Microsoft Edge ブラウザーの設定の同期を許可 (未構成) または禁止 (ブロック) します。 デバイス間での同期を禁止し、ユーザーによる上書きを許可するオプション。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 423d90521529193d2debf778f136a38fb8bbfefa
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971061"
---
# <a name="browsersyncsetting-enum-type"></a><span data-ttu-id="652f8-104">browserSyncSetting 列挙型</span><span class="sxs-lookup"><span data-stu-id="652f8-104">browserSyncSetting enum type</span></span>

> <span data-ttu-id="652f8-105">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="652f8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="652f8-106">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="652f8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="652f8-107">Microsoft Edge ブラウザーの設定の同期を許可 (未構成) または禁止 (ブロック) します。</span><span class="sxs-lookup"><span data-stu-id="652f8-107">Allow(Not Configured) or prevent(Block) the syncing of Microsoft Edge Browser settings.</span></span> <span data-ttu-id="652f8-108">デバイス間での同期を禁止し、ユーザーによる上書きを許可するオプション。</span><span class="sxs-lookup"><span data-stu-id="652f8-108">Option to prevent syncing across devices, but allow user override.</span></span>

## <a name="members"></a><span data-ttu-id="652f8-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="652f8-109">Members</span></span>
|<span data-ttu-id="652f8-110">メンバー</span><span class="sxs-lookup"><span data-stu-id="652f8-110">Member</span></span>|<span data-ttu-id="652f8-111">値</span><span class="sxs-lookup"><span data-stu-id="652f8-111">Value</span></span>|<span data-ttu-id="652f8-112">説明</span><span class="sxs-lookup"><span data-stu-id="652f8-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="652f8-113">notConfigured</span><span class="sxs-lookup"><span data-stu-id="652f8-113">notConfigured</span></span>|<span data-ttu-id="652f8-114">.0</span><span class="sxs-lookup"><span data-stu-id="652f8-114">0</span></span>|<span data-ttu-id="652f8-115">Default –デバイス間でのブラウザー設定の同期を許可します。</span><span class="sxs-lookup"><span data-stu-id="652f8-115">Default – Allow syncing of browser settings across devices.</span></span>|
|<span data-ttu-id="652f8-116">blockedWithUserOverride</span><span class="sxs-lookup"><span data-stu-id="652f8-116">blockedWithUserOverride</span></span>|<span data-ttu-id="652f8-117">1-d</span><span class="sxs-lookup"><span data-stu-id="652f8-117">1</span></span>|<span data-ttu-id="652f8-118">ユーザーのデバイス間でブラウザー設定を同期できないようにして、ユーザーが設定を上書きできるようにします。</span><span class="sxs-lookup"><span data-stu-id="652f8-118">Prevent syncing of browser settings across user devices, allow user override of setting.</span></span>|
|<span data-ttu-id="652f8-119">ブロック</span><span class="sxs-lookup"><span data-stu-id="652f8-119">blocked</span></span>|<span data-ttu-id="652f8-120">pbm-2</span><span class="sxs-lookup"><span data-stu-id="652f8-120">2</span></span>|<span data-ttu-id="652f8-121">ユーザーデバイス間でのブラウザー設定の同期を完全に防止します。</span><span class="sxs-lookup"><span data-stu-id="652f8-121">Absolutely prevent syncing of browser settings across user devices.</span></span>|





