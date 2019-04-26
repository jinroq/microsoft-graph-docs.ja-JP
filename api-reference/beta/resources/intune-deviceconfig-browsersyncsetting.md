---
title: browsersyncsetting 列挙型
description: Microsoft Edge ブラウザーの設定の同期を許可 (未構成) または禁止 (ブロック) します。 デバイス間での同期を禁止し、ユーザーによる上書きを許可するオプション。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f08031e970f56c071a4dd01af0542bd56924edd5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549384"
---
# <a name="browsersyncsetting-enum-type"></a><span data-ttu-id="b9dc4-104">browsersyncsetting 列挙型</span><span class="sxs-lookup"><span data-stu-id="b9dc4-104">browserSyncSetting enum type</span></span>

> <span data-ttu-id="b9dc4-105">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b9dc4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9dc4-106">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b9dc4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9dc4-107">Microsoft Edge ブラウザーの設定の同期を許可 (未構成) または禁止 (ブロック) します。</span><span class="sxs-lookup"><span data-stu-id="b9dc4-107">Allow(Not Configured) or prevent(Block) the syncing of Microsoft Edge Browser settings.</span></span> <span data-ttu-id="b9dc4-108">デバイス間での同期を禁止し、ユーザーによる上書きを許可するオプション。</span><span class="sxs-lookup"><span data-stu-id="b9dc4-108">Option to prevent syncing across devices, but allow user override.</span></span>

## <a name="members"></a><span data-ttu-id="b9dc4-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="b9dc4-109">Members</span></span>
|<span data-ttu-id="b9dc4-110">メンバー</span><span class="sxs-lookup"><span data-stu-id="b9dc4-110">Member</span></span>|<span data-ttu-id="b9dc4-111">値</span><span class="sxs-lookup"><span data-stu-id="b9dc4-111">Value</span></span>|<span data-ttu-id="b9dc4-112">説明</span><span class="sxs-lookup"><span data-stu-id="b9dc4-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9dc4-113">notConfigured</span><span class="sxs-lookup"><span data-stu-id="b9dc4-113">notConfigured</span></span>|<span data-ttu-id="b9dc4-114">.0</span><span class="sxs-lookup"><span data-stu-id="b9dc4-114">0</span></span>|<span data-ttu-id="b9dc4-115">Default –デバイス間でのブラウザー設定の同期を許可します。</span><span class="sxs-lookup"><span data-stu-id="b9dc4-115">Default – Allow syncing of browser settings across devices.</span></span>|
|<span data-ttu-id="b9dc4-116">blockedWithUserOverride</span><span class="sxs-lookup"><span data-stu-id="b9dc4-116">blockedWithUserOverride</span></span>|<span data-ttu-id="b9dc4-117">1 </span><span class="sxs-lookup"><span data-stu-id="b9dc4-117">1</span></span>|<span data-ttu-id="b9dc4-118">ユーザーのデバイス間でブラウザー設定を同期できないようにして、ユーザーが設定を上書きできるようにします。</span><span class="sxs-lookup"><span data-stu-id="b9dc4-118">Prevent syncing of browser settings across user devices, allow user override of setting.</span></span>|
|<span data-ttu-id="b9dc4-119">ブロック</span><span class="sxs-lookup"><span data-stu-id="b9dc4-119">blocked</span></span>|<span data-ttu-id="b9dc4-120">2 </span><span class="sxs-lookup"><span data-stu-id="b9dc4-120">2</span></span>|<span data-ttu-id="b9dc4-121">ユーザーデバイス間でのブラウザー設定の同期を完全に防止します。</span><span class="sxs-lookup"><span data-stu-id="b9dc4-121">Absolutely prevent syncing of browser settings across user devices.</span></span>|





