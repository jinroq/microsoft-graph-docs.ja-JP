---
title: iosNotificationSettings リソース タイプ
description: 通知設定を記述するアイテムです。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 434278967fa5ffe781b53595edae69bffc725289
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34995673"
---
# <a name="iosnotificationsettings-resource-type"></a><span data-ttu-id="15f4d-103">iosNotificationSettings リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="15f4d-103">iosNotificationSettings resource type</span></span>

> <span data-ttu-id="15f4d-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="15f4d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="15f4d-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="15f4d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15f4d-106">通知設定を記述するアイテムです。</span><span class="sxs-lookup"><span data-stu-id="15f4d-106">An item describing notification setting.</span></span>

## <a name="properties"></a><span data-ttu-id="15f4d-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="15f4d-107">Properties</span></span>
|<span data-ttu-id="15f4d-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="15f4d-108">Property</span></span>|<span data-ttu-id="15f4d-109">型</span><span class="sxs-lookup"><span data-stu-id="15f4d-109">Type</span></span>|<span data-ttu-id="15f4d-110">説明</span><span class="sxs-lookup"><span data-stu-id="15f4d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15f4d-111">bundleID</span><span class="sxs-lookup"><span data-stu-id="15f4d-111">bundleID</span></span>|<span data-ttu-id="15f4d-112">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="15f4d-112">String</span></span>|<span data-ttu-id="15f4d-113">これらの通知設定を適用するアプリのバンドル ID。</span><span class="sxs-lookup"><span data-stu-id="15f4d-113">Bundle id of app to which to apply these notification settings.</span></span>|
|<span data-ttu-id="15f4d-114">appName</span><span class="sxs-lookup"><span data-stu-id="15f4d-114">appName</span></span>|<span data-ttu-id="15f4d-115">String</span><span class="sxs-lookup"><span data-stu-id="15f4d-115">String</span></span>|<span data-ttu-id="15f4d-116">bundleID に関連するアプリケーション名。</span><span class="sxs-lookup"><span data-stu-id="15f4d-116">Application name to be associated with the bundleID.</span></span>|
|<span data-ttu-id="15f4d-117">publisher</span><span class="sxs-lookup"><span data-stu-id="15f4d-117">publisher</span></span>|<span data-ttu-id="15f4d-118">String</span><span class="sxs-lookup"><span data-stu-id="15f4d-118">String</span></span>|<span data-ttu-id="15f4d-119">bundleID に関連するパブリッシャー。</span><span class="sxs-lookup"><span data-stu-id="15f4d-119">Publisher to be associated with the bundleID.</span></span>|
|<span data-ttu-id="15f4d-120">enabled</span><span class="sxs-lookup"><span data-stu-id="15f4d-120">enabled</span></span>|<span data-ttu-id="15f4d-121">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="15f4d-121">Boolean</span></span>|<span data-ttu-id="15f4d-122">通知がこのアプリで許可されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="15f4d-122">Indicates whether notifications are allowed for this app.</span></span>|
|<span data-ttu-id="15f4d-123">showInNotificationCenter</span><span class="sxs-lookup"><span data-stu-id="15f4d-123">showInNotificationCenter</span></span>|<span data-ttu-id="15f4d-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="15f4d-124">Boolean</span></span>|<span data-ttu-id="15f4d-125">通知センターに通知を表示できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="15f4d-125">Indicates whether notifications can be shown in notification center.</span></span>|
|<span data-ttu-id="15f4d-126">showOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="15f4d-126">showOnLockScreen</span></span>|<span data-ttu-id="15f4d-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="15f4d-127">Boolean</span></span>|<span data-ttu-id="15f4d-128">ロック画面に通知を表示できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="15f4d-128">Indicates whether notifications can be shown on the lock screen.</span></span>|
|<span data-ttu-id="15f4d-129">alertType</span><span class="sxs-lookup"><span data-stu-id="15f4d-129">alertType</span></span>|[<span data-ttu-id="15f4d-130">iosNotificationAlertType</span><span class="sxs-lookup"><span data-stu-id="15f4d-130">iosNotificationAlertType</span></span>](../resources/intune-deviceconfig-iosnotificationalerttype.md)|<span data-ttu-id="15f4d-131">このアプリの通知用の警告の種類を示します。</span><span class="sxs-lookup"><span data-stu-id="15f4d-131">Indicates the type of alert for notifications for this app.</span></span> <span data-ttu-id="15f4d-132">可能な値は、`deviceDefault`、`banner`、`modal`、`none` です。</span><span class="sxs-lookup"><span data-stu-id="15f4d-132">Possible values are: `deviceDefault`, `banner`, `modal`, `none`.</span></span>|
|<span data-ttu-id="15f4d-133">badgesEnabled</span><span class="sxs-lookup"><span data-stu-id="15f4d-133">badgesEnabled</span></span>|<span data-ttu-id="15f4d-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="15f4d-134">Boolean</span></span>|<span data-ttu-id="15f4d-135">バッジがこのアプリで許可されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="15f4d-135">Indicates whether badges are allowed for this app.</span></span>|
|<span data-ttu-id="15f4d-136">soundsEnabled</span><span class="sxs-lookup"><span data-stu-id="15f4d-136">soundsEnabled</span></span>|<span data-ttu-id="15f4d-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="15f4d-137">Boolean</span></span>|<span data-ttu-id="15f4d-138">サウンドがこのアプリで許可されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="15f4d-138">Indicates whether sounds are allowed for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="15f4d-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="15f4d-139">Relationships</span></span>
<span data-ttu-id="15f4d-140">なし</span><span class="sxs-lookup"><span data-stu-id="15f4d-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="15f4d-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="15f4d-141">JSON Representation</span></span>
<span data-ttu-id="15f4d-142">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="15f4d-142">Here is a JSON representation of the resource.</span></span>
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





