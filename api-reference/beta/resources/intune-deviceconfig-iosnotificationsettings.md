---
title: iosNotificationSettings リソース タイプ
description: 通知設定を記述するアイテムです。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c0d656c7df770c59d0787dcf40ad1081bb8984cd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35970417"
---
# <a name="iosnotificationsettings-resource-type"></a><span data-ttu-id="18de8-103">iosNotificationSettings リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="18de8-103">iosNotificationSettings resource type</span></span>

> <span data-ttu-id="18de8-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="18de8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="18de8-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="18de8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18de8-106">通知設定を記述するアイテムです。</span><span class="sxs-lookup"><span data-stu-id="18de8-106">An item describing notification setting.</span></span>

## <a name="properties"></a><span data-ttu-id="18de8-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="18de8-107">Properties</span></span>
|<span data-ttu-id="18de8-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="18de8-108">Property</span></span>|<span data-ttu-id="18de8-109">型</span><span class="sxs-lookup"><span data-stu-id="18de8-109">Type</span></span>|<span data-ttu-id="18de8-110">説明</span><span class="sxs-lookup"><span data-stu-id="18de8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18de8-111">bundleID</span><span class="sxs-lookup"><span data-stu-id="18de8-111">bundleID</span></span>|<span data-ttu-id="18de8-112">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="18de8-112">String</span></span>|<span data-ttu-id="18de8-113">これらの通知設定を適用するアプリのバンドル ID。</span><span class="sxs-lookup"><span data-stu-id="18de8-113">Bundle id of app to which to apply these notification settings.</span></span>|
|<span data-ttu-id="18de8-114">appName</span><span class="sxs-lookup"><span data-stu-id="18de8-114">appName</span></span>|<span data-ttu-id="18de8-115">String</span><span class="sxs-lookup"><span data-stu-id="18de8-115">String</span></span>|<span data-ttu-id="18de8-116">bundleID に関連するアプリケーション名。</span><span class="sxs-lookup"><span data-stu-id="18de8-116">Application name to be associated with the bundleID.</span></span>|
|<span data-ttu-id="18de8-117">publisher</span><span class="sxs-lookup"><span data-stu-id="18de8-117">publisher</span></span>|<span data-ttu-id="18de8-118">String</span><span class="sxs-lookup"><span data-stu-id="18de8-118">String</span></span>|<span data-ttu-id="18de8-119">bundleID に関連するパブリッシャー。</span><span class="sxs-lookup"><span data-stu-id="18de8-119">Publisher to be associated with the bundleID.</span></span>|
|<span data-ttu-id="18de8-120">enabled</span><span class="sxs-lookup"><span data-stu-id="18de8-120">enabled</span></span>|<span data-ttu-id="18de8-121">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="18de8-121">Boolean</span></span>|<span data-ttu-id="18de8-122">通知がこのアプリで許可されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="18de8-122">Indicates whether notifications are allowed for this app.</span></span>|
|<span data-ttu-id="18de8-123">showInNotificationCenter</span><span class="sxs-lookup"><span data-stu-id="18de8-123">showInNotificationCenter</span></span>|<span data-ttu-id="18de8-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="18de8-124">Boolean</span></span>|<span data-ttu-id="18de8-125">通知センターに通知を表示できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="18de8-125">Indicates whether notifications can be shown in notification center.</span></span>|
|<span data-ttu-id="18de8-126">showOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="18de8-126">showOnLockScreen</span></span>|<span data-ttu-id="18de8-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="18de8-127">Boolean</span></span>|<span data-ttu-id="18de8-128">ロック画面に通知を表示できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="18de8-128">Indicates whether notifications can be shown on the lock screen.</span></span>|
|<span data-ttu-id="18de8-129">alertType</span><span class="sxs-lookup"><span data-stu-id="18de8-129">alertType</span></span>|[<span data-ttu-id="18de8-130">iosNotificationAlertType</span><span class="sxs-lookup"><span data-stu-id="18de8-130">iosNotificationAlertType</span></span>](../resources/intune-deviceconfig-iosnotificationalerttype.md)|<span data-ttu-id="18de8-131">このアプリの通知用の警告の種類を示します。</span><span class="sxs-lookup"><span data-stu-id="18de8-131">Indicates the type of alert for notifications for this app.</span></span> <span data-ttu-id="18de8-132">可能な値は、`deviceDefault`、`banner`、`modal`、`none` です。</span><span class="sxs-lookup"><span data-stu-id="18de8-132">Possible values are: `deviceDefault`, `banner`, `modal`, `none`.</span></span>|
|<span data-ttu-id="18de8-133">badgesEnabled</span><span class="sxs-lookup"><span data-stu-id="18de8-133">badgesEnabled</span></span>|<span data-ttu-id="18de8-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="18de8-134">Boolean</span></span>|<span data-ttu-id="18de8-135">バッジがこのアプリで許可されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="18de8-135">Indicates whether badges are allowed for this app.</span></span>|
|<span data-ttu-id="18de8-136">soundsEnabled</span><span class="sxs-lookup"><span data-stu-id="18de8-136">soundsEnabled</span></span>|<span data-ttu-id="18de8-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="18de8-137">Boolean</span></span>|<span data-ttu-id="18de8-138">サウンドがこのアプリで許可されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="18de8-138">Indicates whether sounds are allowed for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="18de8-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="18de8-139">Relationships</span></span>
<span data-ttu-id="18de8-140">なし</span><span class="sxs-lookup"><span data-stu-id="18de8-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="18de8-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="18de8-141">JSON Representation</span></span>
<span data-ttu-id="18de8-142">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="18de8-142">Here is a JSON representation of the resource.</span></span>
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





