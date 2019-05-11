---
title: mobileAppPublishingState 列挙型
description: アプリの発行状態を示します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ce69b2a2743496714fdb2697cec7e37a1efbaf19
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949921"
---
# <a name="mobileapppublishingstate-enum-type"></a><span data-ttu-id="dc4b4-103">mobileAppPublishingState 列挙型</span><span class="sxs-lookup"><span data-stu-id="dc4b4-103">mobileAppPublishingState enum type</span></span>

> <span data-ttu-id="dc4b4-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dc4b4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dc4b4-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="dc4b4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc4b4-106">アプリの発行状態を示します。</span><span class="sxs-lookup"><span data-stu-id="dc4b4-106">Indicates the publishing state of an app.</span></span>

## <a name="members"></a><span data-ttu-id="dc4b4-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="dc4b4-107">Members</span></span>
|<span data-ttu-id="dc4b4-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="dc4b4-108">Member</span></span>|<span data-ttu-id="dc4b4-109">値</span><span class="sxs-lookup"><span data-stu-id="dc4b4-109">Value</span></span>|<span data-ttu-id="dc4b4-110">説明</span><span class="sxs-lookup"><span data-stu-id="dc4b4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc4b4-111">notPublished</span><span class="sxs-lookup"><span data-stu-id="dc4b4-111">notPublished</span></span>|<span data-ttu-id="dc4b4-112">.0</span><span class="sxs-lookup"><span data-stu-id="dc4b4-112">0</span></span>|<span data-ttu-id="dc4b4-113">アプリはまだ公開されていません。</span><span class="sxs-lookup"><span data-stu-id="dc4b4-113">The app is not yet published.</span></span>|
|<span data-ttu-id="dc4b4-114">プロセッシング</span><span class="sxs-lookup"><span data-stu-id="dc4b4-114">processing</span></span>|<span data-ttu-id="dc4b4-115">1-d</span><span class="sxs-lookup"><span data-stu-id="dc4b4-115">1</span></span>|<span data-ttu-id="dc4b4-116">アプリは、サービス側の処理を保留しています。</span><span class="sxs-lookup"><span data-stu-id="dc4b4-116">The app is pending service-side processing.</span></span>|
|<span data-ttu-id="dc4b4-117">済み</span><span class="sxs-lookup"><span data-stu-id="dc4b4-117">published</span></span>|<span data-ttu-id="dc4b4-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="dc4b4-118">2</span></span>|<span data-ttu-id="dc4b4-119">アプリが発行されます。</span><span class="sxs-lookup"><span data-stu-id="dc4b4-119">The app is published.</span></span>|




