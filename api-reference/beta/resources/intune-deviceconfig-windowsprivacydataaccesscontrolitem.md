---
title: windowsPrivacyDataAccessControlItem リソースの種類
description: プライバシー データのカテゴリごとのアクセス制御レベルを指定します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a772ab511cd57272da8fb1a3a72a17eb1d06737f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407117"
---
# <a name="windowsprivacydataaccesscontrolitem-resource-type"></a><span data-ttu-id="2a61a-103">windowsPrivacyDataAccessControlItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2a61a-103">windowsPrivacyDataAccessControlItem resource type</span></span>

> <span data-ttu-id="2a61a-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2a61a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2a61a-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2a61a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2a61a-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2a61a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a61a-107">プライバシー データのカテゴリごとのアクセス制御レベルを指定します。</span><span class="sxs-lookup"><span data-stu-id="2a61a-107">Specify access control level per privacy data category</span></span>

## <a name="methods"></a><span data-ttu-id="2a61a-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="2a61a-108">Methods</span></span>
|<span data-ttu-id="2a61a-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="2a61a-109">Method</span></span>|<span data-ttu-id="2a61a-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="2a61a-110">Return Type</span></span>|<span data-ttu-id="2a61a-111">説明</span><span class="sxs-lookup"><span data-stu-id="2a61a-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2a61a-112">リスト windowsPrivacyDataAccessControlItems</span><span class="sxs-lookup"><span data-stu-id="2a61a-112">List windowsPrivacyDataAccessControlItems</span></span>](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-list.md)|<span data-ttu-id="2a61a-113">[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="2a61a-113">[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) collection</span></span>|<span data-ttu-id="2a61a-114">[WindowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="2a61a-114">List properties and relationships of the [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) objects.</span></span>|
|[<span data-ttu-id="2a61a-115">WindowsPrivacyDataAccessControlItem を取得します。</span><span class="sxs-lookup"><span data-stu-id="2a61a-115">Get windowsPrivacyDataAccessControlItem</span></span>](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-get.md)|[<span data-ttu-id="2a61a-116">windowsPrivacyDataAccessControlItem</span><span class="sxs-lookup"><span data-stu-id="2a61a-116">windowsPrivacyDataAccessControlItem</span></span>](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|<span data-ttu-id="2a61a-117">[WindowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2a61a-117">Read properties and relationships of the [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>|
|[<span data-ttu-id="2a61a-118">WindowsPrivacyDataAccessControlItem を作成します。</span><span class="sxs-lookup"><span data-stu-id="2a61a-118">Create windowsPrivacyDataAccessControlItem</span></span>](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-create.md)|[<span data-ttu-id="2a61a-119">windowsPrivacyDataAccessControlItem</span><span class="sxs-lookup"><span data-stu-id="2a61a-119">windowsPrivacyDataAccessControlItem</span></span>](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|<span data-ttu-id="2a61a-120">新しい[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="2a61a-120">Create a new [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>|
|[<span data-ttu-id="2a61a-121">WindowsPrivacyDataAccessControlItem を削除します。</span><span class="sxs-lookup"><span data-stu-id="2a61a-121">Delete windowsPrivacyDataAccessControlItem</span></span>](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-delete.md)|<span data-ttu-id="2a61a-122">なし</span><span class="sxs-lookup"><span data-stu-id="2a61a-122">None</span></span>|<span data-ttu-id="2a61a-123">の[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="2a61a-123">Deletes a [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md).</span></span>|
|[<span data-ttu-id="2a61a-124">WindowsPrivacyDataAccessControlItem を更新します。</span><span class="sxs-lookup"><span data-stu-id="2a61a-124">Update windowsPrivacyDataAccessControlItem</span></span>](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-update.md)|[<span data-ttu-id="2a61a-125">windowsPrivacyDataAccessControlItem</span><span class="sxs-lookup"><span data-stu-id="2a61a-125">windowsPrivacyDataAccessControlItem</span></span>](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|<span data-ttu-id="2a61a-126">[WindowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="2a61a-126">Update the properties of a [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2a61a-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2a61a-127">Properties</span></span>
|<span data-ttu-id="2a61a-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2a61a-128">Property</span></span>|<span data-ttu-id="2a61a-129">型</span><span class="sxs-lookup"><span data-stu-id="2a61a-129">Type</span></span>|<span data-ttu-id="2a61a-130">説明</span><span class="sxs-lookup"><span data-stu-id="2a61a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a61a-131">id</span><span class="sxs-lookup"><span data-stu-id="2a61a-131">id</span></span>|<span data-ttu-id="2a61a-132">String</span><span class="sxs-lookup"><span data-stu-id="2a61a-132">String</span></span>|<span data-ttu-id="2a61a-133">WindowsPrivacyDataAccessControlItem のキー。</span><span class="sxs-lookup"><span data-stu-id="2a61a-133">The key of WindowsPrivacyDataAccessControlItem.</span></span>|
|<span data-ttu-id="2a61a-134">accessLevel</span><span class="sxs-lookup"><span data-stu-id="2a61a-134">accessLevel</span></span>|[<span data-ttu-id="2a61a-135">windowsPrivacyDataAccessLevel</span><span class="sxs-lookup"><span data-stu-id="2a61a-135">windowsPrivacyDataAccessLevel</span></span>](../resources/intune-deviceconfig-windowsprivacydataaccesslevel.md)|<span data-ttu-id="2a61a-136">プライバシー データ カテゴリに、指定したアプリケーションを指定するアクセス レベルを示します。</span><span class="sxs-lookup"><span data-stu-id="2a61a-136">This indicates an access level for the privacy data category to which the specified application will be given to.</span></span> <span data-ttu-id="2a61a-137">可能な値は、`notConfigured`、`forceAllow`、`forceDeny`、`userInControl` です。</span><span class="sxs-lookup"><span data-stu-id="2a61a-137">Possible values are: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.</span></span>|
|<span data-ttu-id="2a61a-138">dataCategory</span><span class="sxs-lookup"><span data-stu-id="2a61a-138">dataCategory</span></span>|[<span data-ttu-id="2a61a-139">windowsPrivacyDataCategory</span><span class="sxs-lookup"><span data-stu-id="2a61a-139">windowsPrivacyDataCategory</span></span>](../resources/intune-deviceconfig-windowsprivacydatacategory.md)|<span data-ttu-id="2a61a-140">これは、特定のアクセス制御が適用されるプライバシー データのカテゴリを示します。</span><span class="sxs-lookup"><span data-stu-id="2a61a-140">This indicates a privacy data category to which the specific access control will apply.</span></span> <span data-ttu-id="2a61a-141">使用可能な値: `notConfigured`、 `accountInfo`、 `appsRunInBackground`、 `calendar`、 `callHistory`、 `camera`、 `contacts`、 `diagnosticsInfo`、 `email`、 `location`、 `messaging`、 `microphone`、 `motion`、 `notifications`、 `phone`、 `radios`、 `tasks`、 `syncWithDevices`、 `trustedDevices`.</span><span class="sxs-lookup"><span data-stu-id="2a61a-141">Possible values are: `notConfigured`, `accountInfo`, `appsRunInBackground`, `calendar`, `callHistory`, `camera`, `contacts`, `diagnosticsInfo`, `email`, `location`, `messaging`, `microphone`, `motion`, `notifications`, `phone`, `radios`, `tasks`, `syncWithDevices`, `trustedDevices`.</span></span>|
|<span data-ttu-id="2a61a-142">appPackageFamilyName</span><span class="sxs-lookup"><span data-stu-id="2a61a-142">appPackageFamilyName</span></span>|<span data-ttu-id="2a61a-143">String</span><span class="sxs-lookup"><span data-stu-id="2a61a-143">String</span></span>|<span data-ttu-id="2a61a-144">Windows アプリケーションのパッケージ ファミリ名です。</span><span class="sxs-lookup"><span data-stu-id="2a61a-144">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="2a61a-145">アクセス レベルを設定すると、指定したアプリケーションを適用します。</span><span class="sxs-lookup"><span data-stu-id="2a61a-145">When set, the access level applies to the specified application.</span></span>|
|<span data-ttu-id="2a61a-146">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="2a61a-146">appDisplayName</span></span>|<span data-ttu-id="2a61a-147">String</span><span class="sxs-lookup"><span data-stu-id="2a61a-147">String</span></span>|<span data-ttu-id="2a61a-148">Windows アプリケーションのパッケージ ファミリ名です。</span><span class="sxs-lookup"><span data-stu-id="2a61a-148">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="2a61a-149">アクセス レベルを設定すると、指定したアプリケーションを適用します。</span><span class="sxs-lookup"><span data-stu-id="2a61a-149">When set, the access level applies to the specified application.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2a61a-150">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2a61a-150">Relationships</span></span>
<span data-ttu-id="2a61a-151">なし</span><span class="sxs-lookup"><span data-stu-id="2a61a-151">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2a61a-152">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2a61a-152">JSON Representation</span></span>
<span data-ttu-id="2a61a-153">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2a61a-153">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsPrivacyDataAccessControlItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsPrivacyDataAccessControlItem",
  "id": "String (identifier)",
  "accessLevel": "String",
  "dataCategory": "String",
  "appPackageFamilyName": "String",
  "appDisplayName": "String"
}
```




