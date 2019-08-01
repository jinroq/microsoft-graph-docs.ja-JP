---
title: mobileAppPublishingState 列挙型
description: アプリの発行状態を示します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 81361cabcd1ebade92e1c81b0c5a1677170473c4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032138"
---
# <a name="mobileapppublishingstate-enum-type"></a><span data-ttu-id="b4e20-103">mobileAppPublishingState 列挙型</span><span class="sxs-lookup"><span data-stu-id="b4e20-103">mobileAppPublishingState enum type</span></span>

> <span data-ttu-id="b4e20-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b4e20-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4e20-105">アプリの発行状態を示します。</span><span class="sxs-lookup"><span data-stu-id="b4e20-105">Indicates the publishing state of an app.</span></span>

## <a name="members"></a><span data-ttu-id="b4e20-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="b4e20-106">Members</span></span>
|<span data-ttu-id="b4e20-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="b4e20-107">Member</span></span>|<span data-ttu-id="b4e20-108">値</span><span class="sxs-lookup"><span data-stu-id="b4e20-108">Value</span></span>|<span data-ttu-id="b4e20-109">説明</span><span class="sxs-lookup"><span data-stu-id="b4e20-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4e20-110">notPublished</span><span class="sxs-lookup"><span data-stu-id="b4e20-110">notPublished</span></span>|<span data-ttu-id="b4e20-111">.0</span><span class="sxs-lookup"><span data-stu-id="b4e20-111">0</span></span>|<span data-ttu-id="b4e20-112">アプリはまだ公開されていません。</span><span class="sxs-lookup"><span data-stu-id="b4e20-112">The app is not yet published.</span></span>|
|<span data-ttu-id="b4e20-113">プロセッシング</span><span class="sxs-lookup"><span data-stu-id="b4e20-113">processing</span></span>|<span data-ttu-id="b4e20-114">1-d</span><span class="sxs-lookup"><span data-stu-id="b4e20-114">1</span></span>|<span data-ttu-id="b4e20-115">アプリは、サービス側の処理を保留しています。</span><span class="sxs-lookup"><span data-stu-id="b4e20-115">The app is pending service-side processing.</span></span>|
|<span data-ttu-id="b4e20-116">済み</span><span class="sxs-lookup"><span data-stu-id="b4e20-116">published</span></span>|<span data-ttu-id="b4e20-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="b4e20-117">2</span></span>|<span data-ttu-id="b4e20-118">アプリが発行されます。</span><span class="sxs-lookup"><span data-stu-id="b4e20-118">The app is published.</span></span>|



