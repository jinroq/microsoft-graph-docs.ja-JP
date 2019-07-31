---
title: mobileAppPublishingState 列挙型
description: アプリの発行状態を示します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 98cdcc5db786de9ca38a9a25bfb21ba00e8418b5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971663"
---
# <a name="mobileapppublishingstate-enum-type"></a><span data-ttu-id="92041-103">mobileAppPublishingState 列挙型</span><span class="sxs-lookup"><span data-stu-id="92041-103">mobileAppPublishingState enum type</span></span>

> <span data-ttu-id="92041-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="92041-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92041-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="92041-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92041-106">アプリの発行状態を示します。</span><span class="sxs-lookup"><span data-stu-id="92041-106">Indicates the publishing state of an app.</span></span>

## <a name="members"></a><span data-ttu-id="92041-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="92041-107">Members</span></span>
|<span data-ttu-id="92041-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="92041-108">Member</span></span>|<span data-ttu-id="92041-109">値</span><span class="sxs-lookup"><span data-stu-id="92041-109">Value</span></span>|<span data-ttu-id="92041-110">説明</span><span class="sxs-lookup"><span data-stu-id="92041-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92041-111">notPublished</span><span class="sxs-lookup"><span data-stu-id="92041-111">notPublished</span></span>|<span data-ttu-id="92041-112">.0</span><span class="sxs-lookup"><span data-stu-id="92041-112">0</span></span>|<span data-ttu-id="92041-113">アプリはまだ公開されていません。</span><span class="sxs-lookup"><span data-stu-id="92041-113">The app is not yet published.</span></span>|
|<span data-ttu-id="92041-114">プロセッシング</span><span class="sxs-lookup"><span data-stu-id="92041-114">processing</span></span>|<span data-ttu-id="92041-115">1-d</span><span class="sxs-lookup"><span data-stu-id="92041-115">1</span></span>|<span data-ttu-id="92041-116">アプリは、サービス側の処理を保留しています。</span><span class="sxs-lookup"><span data-stu-id="92041-116">The app is pending service-side processing.</span></span>|
|<span data-ttu-id="92041-117">済み</span><span class="sxs-lookup"><span data-stu-id="92041-117">published</span></span>|<span data-ttu-id="92041-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="92041-118">2</span></span>|<span data-ttu-id="92041-119">アプリが発行されます。</span><span class="sxs-lookup"><span data-stu-id="92041-119">The app is published.</span></span>|





