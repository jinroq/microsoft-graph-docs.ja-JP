---
title: mobileAppPublishingState 列挙型
description: アプリの発行状態を示します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0b0823576dd1792b01193d600cdebbe171b47052
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32557839"
---
# <a name="mobileapppublishingstate-enum-type"></a><span data-ttu-id="0dc78-103">mobileAppPublishingState 列挙型</span><span class="sxs-lookup"><span data-stu-id="0dc78-103">mobileAppPublishingState enum type</span></span>

> <span data-ttu-id="0dc78-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0dc78-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0dc78-105">アプリの発行状態を示します。</span><span class="sxs-lookup"><span data-stu-id="0dc78-105">Indicates the publishing state of an app.</span></span>

## <a name="members"></a><span data-ttu-id="0dc78-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="0dc78-106">Members</span></span>
|<span data-ttu-id="0dc78-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="0dc78-107">Member</span></span>|<span data-ttu-id="0dc78-108">値</span><span class="sxs-lookup"><span data-stu-id="0dc78-108">Value</span></span>|<span data-ttu-id="0dc78-109">説明</span><span class="sxs-lookup"><span data-stu-id="0dc78-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0dc78-110">notpublished</span><span class="sxs-lookup"><span data-stu-id="0dc78-110">notPublished</span></span>|<span data-ttu-id="0dc78-111">.0</span><span class="sxs-lookup"><span data-stu-id="0dc78-111">0</span></span>|<span data-ttu-id="0dc78-112">アプリはまだ公開されていません。</span><span class="sxs-lookup"><span data-stu-id="0dc78-112">The app is not yet published.</span></span>|
|<span data-ttu-id="0dc78-113">プロセッシング</span><span class="sxs-lookup"><span data-stu-id="0dc78-113">processing</span></span>|<span data-ttu-id="0dc78-114">1 </span><span class="sxs-lookup"><span data-stu-id="0dc78-114">1</span></span>|<span data-ttu-id="0dc78-115">アプリは、サービス側の処理を保留しています。</span><span class="sxs-lookup"><span data-stu-id="0dc78-115">The app is pending service-side processing.</span></span>|
|<span data-ttu-id="0dc78-116">済み</span><span class="sxs-lookup"><span data-stu-id="0dc78-116">published</span></span>|<span data-ttu-id="0dc78-117">2 </span><span class="sxs-lookup"><span data-stu-id="0dc78-117">2</span></span>|<span data-ttu-id="0dc78-118">アプリが発行されます。</span><span class="sxs-lookup"><span data-stu-id="0dc78-118">The app is published.</span></span>|



