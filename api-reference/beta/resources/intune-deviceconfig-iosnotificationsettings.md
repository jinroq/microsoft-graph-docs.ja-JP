---
title: iosNotificationSettings リソース タイプ
description: 通知設定を記述するアイテムです。
author: tfitzmac
ms.openlocfilehash: c24e0719e634d2939f88280431538b41fb0a1b5f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359193"
---
# <a name="iosnotificationsettings-resource-type"></a><span data-ttu-id="7a4cf-103">iosNotificationSettings リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="7a4cf-103">iosNotificationSettings resource type</span></span>

> <span data-ttu-id="7a4cf-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7a4cf-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7a4cf-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7a4cf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7a4cf-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7a4cf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7a4cf-107">通知設定を記述するアイテムです。</span><span class="sxs-lookup"><span data-stu-id="7a4cf-107">An item describing notification setting.</span></span>
## <a name="properties"></a><span data-ttu-id="7a4cf-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7a4cf-108">Properties</span></span>
|<span data-ttu-id="7a4cf-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7a4cf-109">Property</span></span>|<span data-ttu-id="7a4cf-110">種類</span><span class="sxs-lookup"><span data-stu-id="7a4cf-110">Type</span></span>|<span data-ttu-id="7a4cf-111">説明</span><span class="sxs-lookup"><span data-stu-id="7a4cf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a4cf-112">bundleID</span><span class="sxs-lookup"><span data-stu-id="7a4cf-112">bundleID</span></span>|<span data-ttu-id="7a4cf-113">String</span><span class="sxs-lookup"><span data-stu-id="7a4cf-113">String</span></span>|<span data-ttu-id="7a4cf-114">これらの通知設定を適用するアプリのバンドル ID。</span><span class="sxs-lookup"><span data-stu-id="7a4cf-114">Bundle id of app to which to apply these notification settings.</span></span>|
|<span data-ttu-id="7a4cf-115">appName</span><span class="sxs-lookup"><span data-stu-id="7a4cf-115">appName</span></span>|<span data-ttu-id="7a4cf-116">String</span><span class="sxs-lookup"><span data-stu-id="7a4cf-116">String</span></span>|<span data-ttu-id="7a4cf-117">bundleID に関連するアプリケーション名。</span><span class="sxs-lookup"><span data-stu-id="7a4cf-117">Application name to be associated with the bundleID.</span></span>|
|<span data-ttu-id="7a4cf-118">publisher</span><span class="sxs-lookup"><span data-stu-id="7a4cf-118">publisher</span></span>|<span data-ttu-id="7a4cf-119">String</span><span class="sxs-lookup"><span data-stu-id="7a4cf-119">String</span></span>|<span data-ttu-id="7a4cf-120">bundleID に関連するパブリッシャー。</span><span class="sxs-lookup"><span data-stu-id="7a4cf-120">Publisher to be associated with the bundleID.</span></span>|
|<span data-ttu-id="7a4cf-121">enabled</span><span class="sxs-lookup"><span data-stu-id="7a4cf-121">enabled</span></span>|<span data-ttu-id="7a4cf-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="7a4cf-122">Boolean</span></span>|<span data-ttu-id="7a4cf-123">通知がこのアプリで許可されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7a4cf-123">Indicates whether notifications are allowed for this app.</span></span>|
|<span data-ttu-id="7a4cf-124">showInNotificationCenter</span><span class="sxs-lookup"><span data-stu-id="7a4cf-124">showInNotificationCenter</span></span>|<span data-ttu-id="7a4cf-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="7a4cf-125">Boolean</span></span>|<span data-ttu-id="7a4cf-126">通知センターに通知を表示できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7a4cf-126">Indicates whether notifications can be shown in notification center.</span></span>|
|<span data-ttu-id="7a4cf-127">showOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="7a4cf-127">showOnLockScreen</span></span>|<span data-ttu-id="7a4cf-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="7a4cf-128">Boolean</span></span>|<span data-ttu-id="7a4cf-129">ロック画面に通知を表示できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7a4cf-129">Indicates whether notifications can be shown on the lock screen.</span></span>|
|<span data-ttu-id="7a4cf-130">alertType</span><span class="sxs-lookup"><span data-stu-id="7a4cf-130">alertType</span></span>|[<span data-ttu-id="7a4cf-131">iosNotificationAlertType</span><span class="sxs-lookup"><span data-stu-id="7a4cf-131">iosNotificationAlertType</span></span>](../resources/intune-deviceconfig-iosnotificationalerttype.md)|<span data-ttu-id="7a4cf-132">このアプリの通知用の警告の種類を示します。</span><span class="sxs-lookup"><span data-stu-id="7a4cf-132">Indicates the type of alert for notifications for this app.</span></span> <span data-ttu-id="7a4cf-133">可能な値は、`deviceDefault`、`banner`、`modal`、`none` です。</span><span class="sxs-lookup"><span data-stu-id="7a4cf-133">Possible values are: `deviceDefault`, `banner`, `modal`, `none`.</span></span>|
|<span data-ttu-id="7a4cf-134">badgesEnabled</span><span class="sxs-lookup"><span data-stu-id="7a4cf-134">badgesEnabled</span></span>|<span data-ttu-id="7a4cf-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="7a4cf-135">Boolean</span></span>|<span data-ttu-id="7a4cf-136">バッジがこのアプリで許可されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7a4cf-136">Indicates whether badges are allowed for this app.</span></span>|
|<span data-ttu-id="7a4cf-137">soundsEnabled</span><span class="sxs-lookup"><span data-stu-id="7a4cf-137">soundsEnabled</span></span>|<span data-ttu-id="7a4cf-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="7a4cf-138">Boolean</span></span>|<span data-ttu-id="7a4cf-139">サウンドがこのアプリで許可されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7a4cf-139">Indicates whether sounds are allowed for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7a4cf-140">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7a4cf-140">Relationships</span></span>
<span data-ttu-id="7a4cf-141">なし</span><span class="sxs-lookup"><span data-stu-id="7a4cf-141">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7a4cf-142">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7a4cf-142">JSON Representation</span></span>
<span data-ttu-id="7a4cf-143">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7a4cf-143">Here is a JSON representation of the resource.</span></span>
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





