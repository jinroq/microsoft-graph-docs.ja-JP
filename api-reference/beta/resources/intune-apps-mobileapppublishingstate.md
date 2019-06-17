---
title: mobileAppPublishingState 列挙型
description: アプリの発行状態を示します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 34e2d06701513e4070384307f49f5dfd0d2b50de
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34991857"
---
# <a name="mobileapppublishingstate-enum-type"></a><span data-ttu-id="4edb0-103">mobileAppPublishingState 列挙型</span><span class="sxs-lookup"><span data-stu-id="4edb0-103">mobileAppPublishingState enum type</span></span>

> <span data-ttu-id="4edb0-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4edb0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4edb0-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4edb0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4edb0-106">アプリの発行状態を示します。</span><span class="sxs-lookup"><span data-stu-id="4edb0-106">Indicates the publishing state of an app.</span></span>

## <a name="members"></a><span data-ttu-id="4edb0-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="4edb0-107">Members</span></span>
|<span data-ttu-id="4edb0-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="4edb0-108">Member</span></span>|<span data-ttu-id="4edb0-109">値</span><span class="sxs-lookup"><span data-stu-id="4edb0-109">Value</span></span>|<span data-ttu-id="4edb0-110">説明</span><span class="sxs-lookup"><span data-stu-id="4edb0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4edb0-111">notPublished</span><span class="sxs-lookup"><span data-stu-id="4edb0-111">notPublished</span></span>|<span data-ttu-id="4edb0-112">.0</span><span class="sxs-lookup"><span data-stu-id="4edb0-112">0</span></span>|<span data-ttu-id="4edb0-113">アプリはまだ公開されていません。</span><span class="sxs-lookup"><span data-stu-id="4edb0-113">The app is not yet published.</span></span>|
|<span data-ttu-id="4edb0-114">プロセッシング</span><span class="sxs-lookup"><span data-stu-id="4edb0-114">processing</span></span>|<span data-ttu-id="4edb0-115">1-d</span><span class="sxs-lookup"><span data-stu-id="4edb0-115">1</span></span>|<span data-ttu-id="4edb0-116">アプリは、サービス側の処理を保留しています。</span><span class="sxs-lookup"><span data-stu-id="4edb0-116">The app is pending service-side processing.</span></span>|
|<span data-ttu-id="4edb0-117">済み</span><span class="sxs-lookup"><span data-stu-id="4edb0-117">published</span></span>|<span data-ttu-id="4edb0-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="4edb0-118">2</span></span>|<span data-ttu-id="4edb0-119">アプリが発行されます。</span><span class="sxs-lookup"><span data-stu-id="4edb0-119">The app is published.</span></span>|





