---
title: iosNotificationSettings リソース タイプ
description: 通知設定を記述するアイテムです。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7db0b6ba438522db0795f6897daba8b5c43258c5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420501"
---
# <a name="iosnotificationsettings-resource-type"></a><span data-ttu-id="cc961-103">iosNotificationSettings リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="cc961-103">iosNotificationSettings resource type</span></span>

> <span data-ttu-id="cc961-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="cc961-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="cc961-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cc961-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cc961-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="cc961-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cc961-107">通知設定を記述するアイテムです。</span><span class="sxs-lookup"><span data-stu-id="cc961-107">An item describing notification setting.</span></span>

## <a name="properties"></a><span data-ttu-id="cc961-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cc961-108">Properties</span></span>
|<span data-ttu-id="cc961-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cc961-109">Property</span></span>|<span data-ttu-id="cc961-110">型</span><span class="sxs-lookup"><span data-stu-id="cc961-110">Type</span></span>|<span data-ttu-id="cc961-111">説明</span><span class="sxs-lookup"><span data-stu-id="cc961-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc961-112">bundleID</span><span class="sxs-lookup"><span data-stu-id="cc961-112">bundleID</span></span>|<span data-ttu-id="cc961-113">String</span><span class="sxs-lookup"><span data-stu-id="cc961-113">String</span></span>|<span data-ttu-id="cc961-114">これらの通知設定を適用するアプリのバンドル ID。</span><span class="sxs-lookup"><span data-stu-id="cc961-114">Bundle id of app to which to apply these notification settings.</span></span>|
|<span data-ttu-id="cc961-115">appName</span><span class="sxs-lookup"><span data-stu-id="cc961-115">appName</span></span>|<span data-ttu-id="cc961-116">String</span><span class="sxs-lookup"><span data-stu-id="cc961-116">String</span></span>|<span data-ttu-id="cc961-117">bundleID に関連するアプリケーション名。</span><span class="sxs-lookup"><span data-stu-id="cc961-117">Application name to be associated with the bundleID.</span></span>|
|<span data-ttu-id="cc961-118">publisher</span><span class="sxs-lookup"><span data-stu-id="cc961-118">publisher</span></span>|<span data-ttu-id="cc961-119">String</span><span class="sxs-lookup"><span data-stu-id="cc961-119">String</span></span>|<span data-ttu-id="cc961-120">bundleID に関連するパブリッシャー。</span><span class="sxs-lookup"><span data-stu-id="cc961-120">Publisher to be associated with the bundleID.</span></span>|
|<span data-ttu-id="cc961-121">enabled</span><span class="sxs-lookup"><span data-stu-id="cc961-121">enabled</span></span>|<span data-ttu-id="cc961-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="cc961-122">Boolean</span></span>|<span data-ttu-id="cc961-123">通知がこのアプリで許可されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="cc961-123">Indicates whether notifications are allowed for this app.</span></span>|
|<span data-ttu-id="cc961-124">showInNotificationCenter</span><span class="sxs-lookup"><span data-stu-id="cc961-124">showInNotificationCenter</span></span>|<span data-ttu-id="cc961-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="cc961-125">Boolean</span></span>|<span data-ttu-id="cc961-126">通知センターに通知を表示できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="cc961-126">Indicates whether notifications can be shown in notification center.</span></span>|
|<span data-ttu-id="cc961-127">showOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="cc961-127">showOnLockScreen</span></span>|<span data-ttu-id="cc961-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="cc961-128">Boolean</span></span>|<span data-ttu-id="cc961-129">ロック画面に通知を表示できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="cc961-129">Indicates whether notifications can be shown on the lock screen.</span></span>|
|<span data-ttu-id="cc961-130">alertType</span><span class="sxs-lookup"><span data-stu-id="cc961-130">alertType</span></span>|[<span data-ttu-id="cc961-131">iosNotificationAlertType</span><span class="sxs-lookup"><span data-stu-id="cc961-131">iosNotificationAlertType</span></span>](../resources/intune-deviceconfig-iosnotificationalerttype.md)|<span data-ttu-id="cc961-132">このアプリの通知用の警告の種類を示します。</span><span class="sxs-lookup"><span data-stu-id="cc961-132">Indicates the type of alert for notifications for this app.</span></span> <span data-ttu-id="cc961-133">可能な値は、`deviceDefault`、`banner`、`modal`、`none` です。</span><span class="sxs-lookup"><span data-stu-id="cc961-133">Possible values are: `deviceDefault`, `banner`, `modal`, `none`.</span></span>|
|<span data-ttu-id="cc961-134">badgesEnabled</span><span class="sxs-lookup"><span data-stu-id="cc961-134">badgesEnabled</span></span>|<span data-ttu-id="cc961-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="cc961-135">Boolean</span></span>|<span data-ttu-id="cc961-136">バッジがこのアプリで許可されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="cc961-136">Indicates whether badges are allowed for this app.</span></span>|
|<span data-ttu-id="cc961-137">soundsEnabled</span><span class="sxs-lookup"><span data-stu-id="cc961-137">soundsEnabled</span></span>|<span data-ttu-id="cc961-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="cc961-138">Boolean</span></span>|<span data-ttu-id="cc961-139">サウンドがこのアプリで許可されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="cc961-139">Indicates whether sounds are allowed for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cc961-140">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="cc961-140">Relationships</span></span>
<span data-ttu-id="cc961-141">なし</span><span class="sxs-lookup"><span data-stu-id="cc961-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cc961-142">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cc961-142">JSON Representation</span></span>
<span data-ttu-id="cc961-143">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="cc961-143">Here is a JSON representation of the resource.</span></span>
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




