---
title: iosWallpaperDisplayLocation 列挙型
description: 壁紙の列挙型は、位置指定子を表示します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cdf6a0a837d420d37641221bf39b5b64f1046591
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430323"
---
# <a name="ioswallpaperdisplaylocation-enum-type"></a><span data-ttu-id="6b610-103">iosWallpaperDisplayLocation 列挙型</span><span class="sxs-lookup"><span data-stu-id="6b610-103">iosWallpaperDisplayLocation enum type</span></span>

> <span data-ttu-id="6b610-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6b610-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6b610-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6b610-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6b610-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6b610-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b610-107">壁紙の列挙型は、位置指定子を表示します。</span><span class="sxs-lookup"><span data-stu-id="6b610-107">An enum type for wallpaper display location specifier.</span></span>

## <a name="members"></a><span data-ttu-id="6b610-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="6b610-108">Members</span></span>
|<span data-ttu-id="6b610-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="6b610-109">Member</span></span>|<span data-ttu-id="6b610-110">値</span><span class="sxs-lookup"><span data-stu-id="6b610-110">Value</span></span>|<span data-ttu-id="6b610-111">説明</span><span class="sxs-lookup"><span data-stu-id="6b610-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b610-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="6b610-112">notConfigured</span></span>|<span data-ttu-id="6b610-113">0</span><span class="sxs-lookup"><span data-stu-id="6b610-113">0</span></span>|<span data-ttu-id="6b610-114">壁紙の表示を指定した場所がありません。</span><span class="sxs-lookup"><span data-stu-id="6b610-114">No location specified for wallpaper display.</span></span>|
|<span data-ttu-id="6b610-115">lockScreen</span><span class="sxs-lookup"><span data-stu-id="6b610-115">lockScreen</span></span>|<span data-ttu-id="6b610-116">1</span><span class="sxs-lookup"><span data-stu-id="6b610-116">1</span></span>|<span data-ttu-id="6b610-117">ロック画面に設定されている壁紙の画像が表示されます。</span><span class="sxs-lookup"><span data-stu-id="6b610-117">A configured wallpaper image is displayed on Lock screen.</span></span>|
|<span data-ttu-id="6b610-118">ホーム スクリーン</span><span class="sxs-lookup"><span data-stu-id="6b610-118">homeScreen</span></span>|<span data-ttu-id="6b610-119">2</span><span class="sxs-lookup"><span data-stu-id="6b610-119">2</span></span>|<span data-ttu-id="6b610-120">(アイコン一覧) のホーム画面に設定されている壁紙の画像が表示されます。</span><span class="sxs-lookup"><span data-stu-id="6b610-120">A configured wallpaper image is displayed on Home (icon list) screen.</span></span>|
|<span data-ttu-id="6b610-121">lockAndHomeScreens</span><span class="sxs-lookup"><span data-stu-id="6b610-121">lockAndHomeScreens</span></span>|<span data-ttu-id="6b610-122">3</span><span class="sxs-lookup"><span data-stu-id="6b610-122">3</span></span>|<span data-ttu-id="6b610-123">ロック画面とホーム画面に設定されている壁紙の画像が表示されます。</span><span class="sxs-lookup"><span data-stu-id="6b610-123">A configured wallpaper image is displayed on Lock screen and Home screen.</span></span>|




