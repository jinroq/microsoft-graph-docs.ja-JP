---
title: iosNotificationSettings リソース タイプ
description: 通知設定を記述するアイテムです。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3ce016579729353f69f2e7671ff67b5da0004536
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260383"
---
# <a name="iosnotificationsettings-resource-type"></a><span data-ttu-id="c6824-103">iosNotificationSettings リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="c6824-103">iosNotificationSettings resource type</span></span>

> <span data-ttu-id="c6824-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c6824-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c6824-105">通知設定を記述するアイテムです。</span><span class="sxs-lookup"><span data-stu-id="c6824-105">An item describing notification setting.</span></span>

## <a name="properties"></a><span data-ttu-id="c6824-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c6824-106">Properties</span></span>
|<span data-ttu-id="c6824-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c6824-107">Property</span></span>|<span data-ttu-id="c6824-108">型</span><span class="sxs-lookup"><span data-stu-id="c6824-108">Type</span></span>|<span data-ttu-id="c6824-109">説明</span><span class="sxs-lookup"><span data-stu-id="c6824-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6824-110">bundleID</span><span class="sxs-lookup"><span data-stu-id="c6824-110">bundleID</span></span>|<span data-ttu-id="c6824-111">String</span><span class="sxs-lookup"><span data-stu-id="c6824-111">String</span></span>|<span data-ttu-id="c6824-112">これらの通知設定を適用するアプリのバンドル ID。</span><span class="sxs-lookup"><span data-stu-id="c6824-112">Bundle id of app to which to apply these notification settings.</span></span>|
|<span data-ttu-id="c6824-113">appName</span><span class="sxs-lookup"><span data-stu-id="c6824-113">appName</span></span>|<span data-ttu-id="c6824-114">String</span><span class="sxs-lookup"><span data-stu-id="c6824-114">String</span></span>|<span data-ttu-id="c6824-115">bundleID に関連するアプリケーション名。</span><span class="sxs-lookup"><span data-stu-id="c6824-115">Application name to be associated with the bundleID.</span></span>|
|<span data-ttu-id="c6824-116">publisher</span><span class="sxs-lookup"><span data-stu-id="c6824-116">publisher</span></span>|<span data-ttu-id="c6824-117">String</span><span class="sxs-lookup"><span data-stu-id="c6824-117">String</span></span>|<span data-ttu-id="c6824-118">bundleID に関連するパブリッシャー。</span><span class="sxs-lookup"><span data-stu-id="c6824-118">Publisher to be associated with the bundleID.</span></span>|
|<span data-ttu-id="c6824-119">enabled</span><span class="sxs-lookup"><span data-stu-id="c6824-119">enabled</span></span>|<span data-ttu-id="c6824-120">ブール型</span><span class="sxs-lookup"><span data-stu-id="c6824-120">Boolean</span></span>|<span data-ttu-id="c6824-121">通知がこのアプリで許可されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c6824-121">Indicates whether notifications are allowed for this app.</span></span>|
|<span data-ttu-id="c6824-122">showInNotificationCenter</span><span class="sxs-lookup"><span data-stu-id="c6824-122">showInNotificationCenter</span></span>|<span data-ttu-id="c6824-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6824-123">Boolean</span></span>|<span data-ttu-id="c6824-124">通知センターに通知を表示できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c6824-124">Indicates whether notifications can be shown in notification center.</span></span>|
|<span data-ttu-id="c6824-125">showOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="c6824-125">showOnLockScreen</span></span>|<span data-ttu-id="c6824-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6824-126">Boolean</span></span>|<span data-ttu-id="c6824-127">ロック画面に通知を表示できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c6824-127">Indicates whether notifications can be shown on the lock screen.</span></span>|
|<span data-ttu-id="c6824-128">alertType</span><span class="sxs-lookup"><span data-stu-id="c6824-128">alertType</span></span>|[<span data-ttu-id="c6824-129">iosnotificationalerttype</span><span class="sxs-lookup"><span data-stu-id="c6824-129">iosNotificationAlertType</span></span>](../resources/intune-deviceconfig-iosnotificationalerttype.md)|<span data-ttu-id="c6824-130">このアプリの通知用の警告の種類を示します。</span><span class="sxs-lookup"><span data-stu-id="c6824-130">Indicates the type of alert for notifications for this app.</span></span> <span data-ttu-id="c6824-131">可能な値は、`deviceDefault`、`banner`、`modal`、`none` です。</span><span class="sxs-lookup"><span data-stu-id="c6824-131">Possible values are: `deviceDefault`, `banner`, `modal`, `none`.</span></span>|
|<span data-ttu-id="c6824-132">badgesEnabled</span><span class="sxs-lookup"><span data-stu-id="c6824-132">badgesEnabled</span></span>|<span data-ttu-id="c6824-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6824-133">Boolean</span></span>|<span data-ttu-id="c6824-134">バッジがこのアプリで許可されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c6824-134">Indicates whether badges are allowed for this app.</span></span>|
|<span data-ttu-id="c6824-135">soundsEnabled</span><span class="sxs-lookup"><span data-stu-id="c6824-135">soundsEnabled</span></span>|<span data-ttu-id="c6824-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6824-136">Boolean</span></span>|<span data-ttu-id="c6824-137">サウンドがこのアプリで許可されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c6824-137">Indicates whether sounds are allowed for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c6824-138">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c6824-138">Relationships</span></span>
<span data-ttu-id="c6824-139">なし</span><span class="sxs-lookup"><span data-stu-id="c6824-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c6824-140">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c6824-140">JSON Representation</span></span>
<span data-ttu-id="c6824-141">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c6824-141">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosNotificationSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosNotificationSettings",
  "bundleID": "String",
  "appName": "String",
  "publisher": "String",
  "enabled": true,
  "showInNotificationCenter": true,
  "showOnLockScreen": true,
  "alertType": "String",
  "badgesEnabled": true,
  "soundsEnabled": true
}
```



