---
title: iosNotificationSettings リソース タイプ
description: 通知設定を記述するアイテムです。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1e80a0f8964b72f4e58a987b9aace861ba18c7f9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911743"
---
# <a name="iosnotificationsettings-resource-type"></a><span data-ttu-id="f5dcd-103">iosNotificationSettings リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="f5dcd-103">iosNotificationSettings resource type</span></span>

> <span data-ttu-id="f5dcd-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f5dcd-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f5dcd-105">通知設定を記述するアイテムです。</span><span class="sxs-lookup"><span data-stu-id="f5dcd-105">An item describing notification setting.</span></span>
## <a name="properties"></a><span data-ttu-id="f5dcd-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f5dcd-106">Properties</span></span>
|<span data-ttu-id="f5dcd-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f5dcd-107">Property</span></span>|<span data-ttu-id="f5dcd-108">型</span><span class="sxs-lookup"><span data-stu-id="f5dcd-108">Type</span></span>|<span data-ttu-id="f5dcd-109">説明</span><span class="sxs-lookup"><span data-stu-id="f5dcd-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5dcd-110">bundleID</span><span class="sxs-lookup"><span data-stu-id="f5dcd-110">bundleID</span></span>|<span data-ttu-id="f5dcd-111">String</span><span class="sxs-lookup"><span data-stu-id="f5dcd-111">String</span></span>|<span data-ttu-id="f5dcd-112">これらの通知設定を適用するアプリのバンドル ID。</span><span class="sxs-lookup"><span data-stu-id="f5dcd-112">Bundle id of app to which to apply these notification settings.</span></span>|
|<span data-ttu-id="f5dcd-113">appName</span><span class="sxs-lookup"><span data-stu-id="f5dcd-113">appName</span></span>|<span data-ttu-id="f5dcd-114">String</span><span class="sxs-lookup"><span data-stu-id="f5dcd-114">String</span></span>|<span data-ttu-id="f5dcd-115">bundleID に関連するアプリケーション名。</span><span class="sxs-lookup"><span data-stu-id="f5dcd-115">Application name to be associated with the bundleID.</span></span>|
|<span data-ttu-id="f5dcd-116">publisher</span><span class="sxs-lookup"><span data-stu-id="f5dcd-116">publisher</span></span>|<span data-ttu-id="f5dcd-117">String</span><span class="sxs-lookup"><span data-stu-id="f5dcd-117">String</span></span>|<span data-ttu-id="f5dcd-118">bundleID に関連するパブリッシャー。</span><span class="sxs-lookup"><span data-stu-id="f5dcd-118">Publisher to be associated with the bundleID.</span></span>|
|<span data-ttu-id="f5dcd-119">enabled</span><span class="sxs-lookup"><span data-stu-id="f5dcd-119">enabled</span></span>|<span data-ttu-id="f5dcd-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5dcd-120">Boolean</span></span>|<span data-ttu-id="f5dcd-121">通知がこのアプリで許可されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f5dcd-121">Indicates whether notifications are allowed for this app.</span></span>|
|<span data-ttu-id="f5dcd-122">showInNotificationCenter</span><span class="sxs-lookup"><span data-stu-id="f5dcd-122">showInNotificationCenter</span></span>|<span data-ttu-id="f5dcd-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5dcd-123">Boolean</span></span>|<span data-ttu-id="f5dcd-124">通知センターに通知を表示できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f5dcd-124">Indicates whether notifications can be shown in notification center.</span></span>|
|<span data-ttu-id="f5dcd-125">showOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="f5dcd-125">showOnLockScreen</span></span>|<span data-ttu-id="f5dcd-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5dcd-126">Boolean</span></span>|<span data-ttu-id="f5dcd-127">ロック画面に通知を表示できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f5dcd-127">Indicates whether notifications can be shown on the lock screen.</span></span>|
|<span data-ttu-id="f5dcd-128">alertType</span><span class="sxs-lookup"><span data-stu-id="f5dcd-128">alertType</span></span>|[<span data-ttu-id="f5dcd-129">iosNotificationAlertType</span><span class="sxs-lookup"><span data-stu-id="f5dcd-129">iosNotificationAlertType</span></span>](../resources/intune-deviceconfig-iosnotificationalerttype.md)|<span data-ttu-id="f5dcd-130">このアプリの通知用の警告の種類を示します。</span><span class="sxs-lookup"><span data-stu-id="f5dcd-130">Indicates the type of alert for notifications for this app.</span></span> <span data-ttu-id="f5dcd-131">可能な値は、`deviceDefault`、`banner`、`modal`、`none` です。</span><span class="sxs-lookup"><span data-stu-id="f5dcd-131">Possible values are: `deviceDefault`, `banner`, `modal`, `none`.</span></span>|
|<span data-ttu-id="f5dcd-132">badgesEnabled</span><span class="sxs-lookup"><span data-stu-id="f5dcd-132">badgesEnabled</span></span>|<span data-ttu-id="f5dcd-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5dcd-133">Boolean</span></span>|<span data-ttu-id="f5dcd-134">バッジがこのアプリで許可されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f5dcd-134">Indicates whether badges are allowed for this app.</span></span>|
|<span data-ttu-id="f5dcd-135">soundsEnabled</span><span class="sxs-lookup"><span data-stu-id="f5dcd-135">soundsEnabled</span></span>|<span data-ttu-id="f5dcd-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5dcd-136">Boolean</span></span>|<span data-ttu-id="f5dcd-137">サウンドがこのアプリで許可されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f5dcd-137">Indicates whether sounds are allowed for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f5dcd-138">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f5dcd-138">Relationships</span></span>
<span data-ttu-id="f5dcd-139">なし</span><span class="sxs-lookup"><span data-stu-id="f5dcd-139">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f5dcd-140">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f5dcd-140">JSON Representation</span></span>
<span data-ttu-id="f5dcd-141">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f5dcd-141">Here is a JSON representation of the resource.</span></span>
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



