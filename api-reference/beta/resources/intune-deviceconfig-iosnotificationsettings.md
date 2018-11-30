---
title: iosNotificationSettings リソース タイプ
description: 通知設定を記述するアイテムです。
ms.openlocfilehash: 515bf103c32694a16650986c91a3b719fad93236
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068172"
---
# <a name="iosnotificationsettings-resource-type"></a><span data-ttu-id="15844-103">iosNotificationSettings リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="15844-103">iosNotificationSettings resource type</span></span>

> <span data-ttu-id="15844-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="15844-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="15844-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="15844-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="15844-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="15844-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="15844-107">通知設定を記述するアイテムです。</span><span class="sxs-lookup"><span data-stu-id="15844-107">An item describing notification setting.</span></span>
## <a name="properties"></a><span data-ttu-id="15844-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="15844-108">Properties</span></span>
|<span data-ttu-id="15844-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="15844-109">Property</span></span>|<span data-ttu-id="15844-110">型</span><span class="sxs-lookup"><span data-stu-id="15844-110">Type</span></span>|<span data-ttu-id="15844-111">説明</span><span class="sxs-lookup"><span data-stu-id="15844-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15844-112">bundleID</span><span class="sxs-lookup"><span data-stu-id="15844-112">bundleID</span></span>|<span data-ttu-id="15844-113">String</span><span class="sxs-lookup"><span data-stu-id="15844-113">String</span></span>|<span data-ttu-id="15844-114">これらの通知設定を適用するアプリのバンドル ID。</span><span class="sxs-lookup"><span data-stu-id="15844-114">Bundle id of app to which to apply these notification settings.</span></span>|
|<span data-ttu-id="15844-115">appName</span><span class="sxs-lookup"><span data-stu-id="15844-115">appName</span></span>|<span data-ttu-id="15844-116">String</span><span class="sxs-lookup"><span data-stu-id="15844-116">String</span></span>|<span data-ttu-id="15844-117">bundleID に関連するアプリケーション名。</span><span class="sxs-lookup"><span data-stu-id="15844-117">Application name to be associated with the bundleID.</span></span>|
|<span data-ttu-id="15844-118">publisher</span><span class="sxs-lookup"><span data-stu-id="15844-118">publisher</span></span>|<span data-ttu-id="15844-119">String</span><span class="sxs-lookup"><span data-stu-id="15844-119">String</span></span>|<span data-ttu-id="15844-120">bundleID に関連するパブリッシャー。</span><span class="sxs-lookup"><span data-stu-id="15844-120">Publisher to be associated with the bundleID.</span></span>|
|<span data-ttu-id="15844-121">enabled</span><span class="sxs-lookup"><span data-stu-id="15844-121">enabled</span></span>|<span data-ttu-id="15844-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="15844-122">Boolean</span></span>|<span data-ttu-id="15844-123">通知がこのアプリで許可されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="15844-123">Indicates whether notifications are allowed for this app.</span></span>|
|<span data-ttu-id="15844-124">showInNotificationCenter</span><span class="sxs-lookup"><span data-stu-id="15844-124">showInNotificationCenter</span></span>|<span data-ttu-id="15844-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="15844-125">Boolean</span></span>|<span data-ttu-id="15844-126">通知センターに通知を表示できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="15844-126">Indicates whether notifications can be shown in notification center.</span></span>|
|<span data-ttu-id="15844-127">showOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="15844-127">showOnLockScreen</span></span>|<span data-ttu-id="15844-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="15844-128">Boolean</span></span>|<span data-ttu-id="15844-129">ロック画面に通知を表示できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="15844-129">Indicates whether notifications can be shown on the lock screen.</span></span>|
|<span data-ttu-id="15844-130">alertType</span><span class="sxs-lookup"><span data-stu-id="15844-130">alertType</span></span>|[<span data-ttu-id="15844-131">iosNotificationAlertType</span><span class="sxs-lookup"><span data-stu-id="15844-131">iosNotificationAlertType</span></span>](../resources/intune-deviceconfig-iosnotificationalerttype.md)|<span data-ttu-id="15844-132">このアプリの通知用の警告の種類を示します。</span><span class="sxs-lookup"><span data-stu-id="15844-132">Indicates the type of alert for notifications for this app.</span></span> <span data-ttu-id="15844-133">可能な値は、`deviceDefault`、`banner`、`modal`、`none` です。</span><span class="sxs-lookup"><span data-stu-id="15844-133">Possible values are: `deviceDefault`, `banner`, `modal`, `none`.</span></span>|
|<span data-ttu-id="15844-134">badgesEnabled</span><span class="sxs-lookup"><span data-stu-id="15844-134">badgesEnabled</span></span>|<span data-ttu-id="15844-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="15844-135">Boolean</span></span>|<span data-ttu-id="15844-136">バッジがこのアプリで許可されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="15844-136">Indicates whether badges are allowed for this app.</span></span>|
|<span data-ttu-id="15844-137">soundsEnabled</span><span class="sxs-lookup"><span data-stu-id="15844-137">soundsEnabled</span></span>|<span data-ttu-id="15844-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="15844-138">Boolean</span></span>|<span data-ttu-id="15844-139">サウンドがこのアプリで許可されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="15844-139">Indicates whether sounds are allowed for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="15844-140">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="15844-140">Relationships</span></span>
<span data-ttu-id="15844-141">なし</span><span class="sxs-lookup"><span data-stu-id="15844-141">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="15844-142">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="15844-142">JSON Representation</span></span>
<span data-ttu-id="15844-143">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="15844-143">Here is a JSON representation of the resource.</span></span>
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





