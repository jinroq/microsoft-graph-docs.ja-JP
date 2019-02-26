---
title: iosNotificationSettings リソース タイプ
description: 通知設定を記述するアイテムです。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2876146e7e20ad94a7356f623a5b2e17443a18f8
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172703"
---
# <a name="iosnotificationsettings-resource-type"></a><span data-ttu-id="de436-103">iosNotificationSettings リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="de436-103">iosNotificationSettings resource type</span></span>

> <span data-ttu-id="de436-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="de436-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="de436-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="de436-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de436-106">通知設定を記述するアイテムです。</span><span class="sxs-lookup"><span data-stu-id="de436-106">An item describing notification setting.</span></span>

## <a name="properties"></a><span data-ttu-id="de436-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="de436-107">Properties</span></span>
|<span data-ttu-id="de436-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="de436-108">Property</span></span>|<span data-ttu-id="de436-109">型</span><span class="sxs-lookup"><span data-stu-id="de436-109">Type</span></span>|<span data-ttu-id="de436-110">説明</span><span class="sxs-lookup"><span data-stu-id="de436-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de436-111">bundleID</span><span class="sxs-lookup"><span data-stu-id="de436-111">bundleID</span></span>|<span data-ttu-id="de436-112">String</span><span class="sxs-lookup"><span data-stu-id="de436-112">String</span></span>|<span data-ttu-id="de436-113">これらの通知設定を適用するアプリのバンドル ID。</span><span class="sxs-lookup"><span data-stu-id="de436-113">Bundle id of app to which to apply these notification settings.</span></span>|
|<span data-ttu-id="de436-114">appName</span><span class="sxs-lookup"><span data-stu-id="de436-114">appName</span></span>|<span data-ttu-id="de436-115">String</span><span class="sxs-lookup"><span data-stu-id="de436-115">String</span></span>|<span data-ttu-id="de436-116">bundleID に関連するアプリケーション名。</span><span class="sxs-lookup"><span data-stu-id="de436-116">Application name to be associated with the bundleID.</span></span>|
|<span data-ttu-id="de436-117">publisher</span><span class="sxs-lookup"><span data-stu-id="de436-117">publisher</span></span>|<span data-ttu-id="de436-118">String</span><span class="sxs-lookup"><span data-stu-id="de436-118">String</span></span>|<span data-ttu-id="de436-119">bundleID に関連するパブリッシャー。</span><span class="sxs-lookup"><span data-stu-id="de436-119">Publisher to be associated with the bundleID.</span></span>|
|<span data-ttu-id="de436-120">enabled</span><span class="sxs-lookup"><span data-stu-id="de436-120">enabled</span></span>|<span data-ttu-id="de436-121">ブール型</span><span class="sxs-lookup"><span data-stu-id="de436-121">Boolean</span></span>|<span data-ttu-id="de436-122">通知がこのアプリで許可されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="de436-122">Indicates whether notifications are allowed for this app.</span></span>|
|<span data-ttu-id="de436-123">showInNotificationCenter</span><span class="sxs-lookup"><span data-stu-id="de436-123">showInNotificationCenter</span></span>|<span data-ttu-id="de436-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="de436-124">Boolean</span></span>|<span data-ttu-id="de436-125">通知センターに通知を表示できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="de436-125">Indicates whether notifications can be shown in notification center.</span></span>|
|<span data-ttu-id="de436-126">showOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="de436-126">showOnLockScreen</span></span>|<span data-ttu-id="de436-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="de436-127">Boolean</span></span>|<span data-ttu-id="de436-128">ロック画面に通知を表示できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="de436-128">Indicates whether notifications can be shown on the lock screen.</span></span>|
|<span data-ttu-id="de436-129">alertType</span><span class="sxs-lookup"><span data-stu-id="de436-129">alertType</span></span>|[<span data-ttu-id="de436-130">iosnotificationalerttype</span><span class="sxs-lookup"><span data-stu-id="de436-130">iosNotificationAlertType</span></span>](../resources/intune-deviceconfig-iosnotificationalerttype.md)|<span data-ttu-id="de436-131">このアプリの通知用の警告の種類を示します。</span><span class="sxs-lookup"><span data-stu-id="de436-131">Indicates the type of alert for notifications for this app.</span></span> <span data-ttu-id="de436-132">可能な値は、`deviceDefault`、`banner`、`modal`、`none` です。</span><span class="sxs-lookup"><span data-stu-id="de436-132">Possible values are: `deviceDefault`, `banner`, `modal`, `none`.</span></span>|
|<span data-ttu-id="de436-133">badgesEnabled</span><span class="sxs-lookup"><span data-stu-id="de436-133">badgesEnabled</span></span>|<span data-ttu-id="de436-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="de436-134">Boolean</span></span>|<span data-ttu-id="de436-135">バッジがこのアプリで許可されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="de436-135">Indicates whether badges are allowed for this app.</span></span>|
|<span data-ttu-id="de436-136">soundsEnabled</span><span class="sxs-lookup"><span data-stu-id="de436-136">soundsEnabled</span></span>|<span data-ttu-id="de436-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="de436-137">Boolean</span></span>|<span data-ttu-id="de436-138">サウンドがこのアプリで許可されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="de436-138">Indicates whether sounds are allowed for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="de436-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="de436-139">Relationships</span></span>
<span data-ttu-id="de436-140">なし</span><span class="sxs-lookup"><span data-stu-id="de436-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="de436-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="de436-141">JSON Representation</span></span>
<span data-ttu-id="de436-142">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="de436-142">Here is a JSON representation of the resource.</span></span>
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




