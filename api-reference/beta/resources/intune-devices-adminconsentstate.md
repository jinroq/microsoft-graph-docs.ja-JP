---
title: adminconstate state 列挙型
description: 管理者の同意状態。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c8a86e8cf427669777c8bd89edd81653449ac8ed
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32571815"
---
# <a name="adminconsentstate-enum-type"></a><span data-ttu-id="9dcb5-103">adminconstate state 列挙型</span><span class="sxs-lookup"><span data-stu-id="9dcb5-103">adminConsentState enum type</span></span>

> <span data-ttu-id="9dcb5-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9dcb5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9dcb5-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9dcb5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9dcb5-106">管理者の同意状態。</span><span class="sxs-lookup"><span data-stu-id="9dcb5-106">Admin consent state.</span></span>

## <a name="members"></a><span data-ttu-id="9dcb5-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="9dcb5-107">Members</span></span>
|<span data-ttu-id="9dcb5-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="9dcb5-108">Member</span></span>|<span data-ttu-id="9dcb5-109">値</span><span class="sxs-lookup"><span data-stu-id="9dcb5-109">Value</span></span>|<span data-ttu-id="9dcb5-110">説明</span><span class="sxs-lookup"><span data-stu-id="9dcb5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9dcb5-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="9dcb5-111">notConfigured</span></span>|<span data-ttu-id="9dcb5-112">.0</span><span class="sxs-lookup"><span data-stu-id="9dcb5-112">0</span></span>|<span data-ttu-id="9dcb5-113">管理者がアイテムを構成しませんでした</span><span class="sxs-lookup"><span data-stu-id="9dcb5-113">Admin did not configure the item</span></span>|
|<span data-ttu-id="9dcb5-114">granted</span><span class="sxs-lookup"><span data-stu-id="9dcb5-114">granted</span></span>|<span data-ttu-id="9dcb5-115">1 </span><span class="sxs-lookup"><span data-stu-id="9dcb5-115">1</span></span>|<span data-ttu-id="9dcb5-116">管理者付与のアイテム</span><span class="sxs-lookup"><span data-stu-id="9dcb5-116">Admin granted item</span></span>|
|<span data-ttu-id="9dcb5-117">notgranted</span><span class="sxs-lookup"><span data-stu-id="9dcb5-117">notGranted</span></span>|<span data-ttu-id="9dcb5-118">2 </span><span class="sxs-lookup"><span data-stu-id="9dcb5-118">2</span></span>|<span data-ttu-id="9dcb5-119">管理者がアイテムを付与することはできません</span><span class="sxs-lookup"><span data-stu-id="9dcb5-119">Admin deos not grant item</span></span>|





