---
title: mobileAppPublishingState 列挙型
description: アプリの発行状態を示します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: b117e328d5f99f1a382e5a9964fbeec51b594910
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36367450"
---
# <a name="mobileapppublishingstate-enum-type"></a><span data-ttu-id="7579d-103">mobileAppPublishingState 列挙型</span><span class="sxs-lookup"><span data-stu-id="7579d-103">mobileAppPublishingState enum type</span></span>

> <span data-ttu-id="7579d-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7579d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7579d-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7579d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7579d-106">アプリの発行状態を示します。</span><span class="sxs-lookup"><span data-stu-id="7579d-106">Indicates the publishing state of an app.</span></span>

## <a name="members"></a><span data-ttu-id="7579d-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="7579d-107">Members</span></span>
|<span data-ttu-id="7579d-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="7579d-108">Member</span></span>|<span data-ttu-id="7579d-109">値</span><span class="sxs-lookup"><span data-stu-id="7579d-109">Value</span></span>|<span data-ttu-id="7579d-110">説明</span><span class="sxs-lookup"><span data-stu-id="7579d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7579d-111">notPublished</span><span class="sxs-lookup"><span data-stu-id="7579d-111">notPublished</span></span>|<span data-ttu-id="7579d-112">.0</span><span class="sxs-lookup"><span data-stu-id="7579d-112">0</span></span>|<span data-ttu-id="7579d-113">アプリはまだ公開されていません。</span><span class="sxs-lookup"><span data-stu-id="7579d-113">The app is not yet published.</span></span>|
|<span data-ttu-id="7579d-114">プロセッシング</span><span class="sxs-lookup"><span data-stu-id="7579d-114">processing</span></span>|<span data-ttu-id="7579d-115">1-d</span><span class="sxs-lookup"><span data-stu-id="7579d-115">1</span></span>|<span data-ttu-id="7579d-116">アプリは、サービス側の処理を保留しています。</span><span class="sxs-lookup"><span data-stu-id="7579d-116">The app is pending service-side processing.</span></span>|
|<span data-ttu-id="7579d-117">済み</span><span class="sxs-lookup"><span data-stu-id="7579d-117">published</span></span>|<span data-ttu-id="7579d-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="7579d-118">2</span></span>|<span data-ttu-id="7579d-119">アプリが発行されます。</span><span class="sxs-lookup"><span data-stu-id="7579d-119">The app is published.</span></span>|



