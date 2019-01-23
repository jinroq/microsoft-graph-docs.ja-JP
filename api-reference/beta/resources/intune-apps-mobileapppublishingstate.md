---
title: mobileAppPublishingState 列挙型
description: アプリケーションの発行状態を示します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: db10e62e714e50ccdf9bac933b2746cb52ea25eb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423882"
---
# <a name="mobileapppublishingstate-enum-type"></a><span data-ttu-id="b735c-103">mobileAppPublishingState 列挙型</span><span class="sxs-lookup"><span data-stu-id="b735c-103">mobileAppPublishingState enum type</span></span>

> <span data-ttu-id="b735c-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b735c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b735c-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b735c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b735c-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b735c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b735c-107">アプリケーションの発行状態を示します。</span><span class="sxs-lookup"><span data-stu-id="b735c-107">Indicates the publishing state of an app.</span></span>

## <a name="members"></a><span data-ttu-id="b735c-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="b735c-108">Members</span></span>
|<span data-ttu-id="b735c-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="b735c-109">Member</span></span>|<span data-ttu-id="b735c-110">値</span><span class="sxs-lookup"><span data-stu-id="b735c-110">Value</span></span>|<span data-ttu-id="b735c-111">説明</span><span class="sxs-lookup"><span data-stu-id="b735c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b735c-112">notPublished</span><span class="sxs-lookup"><span data-stu-id="b735c-112">notPublished</span></span>|<span data-ttu-id="b735c-113">0</span><span class="sxs-lookup"><span data-stu-id="b735c-113">0</span></span>|<span data-ttu-id="b735c-114">アプリケーションはまだ公開されていません。</span><span class="sxs-lookup"><span data-stu-id="b735c-114">The app is not yet published.</span></span>|
|<span data-ttu-id="b735c-115">処理</span><span class="sxs-lookup"><span data-stu-id="b735c-115">processing</span></span>|<span data-ttu-id="b735c-116">1</span><span class="sxs-lookup"><span data-stu-id="b735c-116">1</span></span>|<span data-ttu-id="b735c-117">アプリケーションは、サービス側の処理を保留中です。</span><span class="sxs-lookup"><span data-stu-id="b735c-117">The app is pending service-side processing.</span></span>|
|<span data-ttu-id="b735c-118">公開</span><span class="sxs-lookup"><span data-stu-id="b735c-118">published</span></span>|<span data-ttu-id="b735c-119">2</span><span class="sxs-lookup"><span data-stu-id="b735c-119">2</span></span>|<span data-ttu-id="b735c-120">アプリケーションが発行されます。</span><span class="sxs-lookup"><span data-stu-id="b735c-120">The app is published.</span></span>|




