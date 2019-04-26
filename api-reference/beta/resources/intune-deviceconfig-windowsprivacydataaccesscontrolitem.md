---
title: windowsPrivacyDataAccessControlItem リソースの種類
description: プライバシーデータカテゴリごとにアクセス制御レベルを指定する
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 18cae7e3afe2d9deb0efd55092b1fc1f5e3693b8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563785"
---
# <a name="windowsprivacydataaccesscontrolitem-resource-type"></a><span data-ttu-id="93561-103">windowsPrivacyDataAccessControlItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="93561-103">windowsPrivacyDataAccessControlItem resource type</span></span>

> <span data-ttu-id="93561-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="93561-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="93561-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="93561-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="93561-106">プライバシーデータカテゴリごとにアクセス制御レベルを指定する</span><span class="sxs-lookup"><span data-stu-id="93561-106">Specify access control level per privacy data category</span></span>

## <a name="methods"></a><span data-ttu-id="93561-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="93561-107">Methods</span></span>
|<span data-ttu-id="93561-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="93561-108">Method</span></span>|<span data-ttu-id="93561-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="93561-109">Return Type</span></span>|<span data-ttu-id="93561-110">説明</span><span class="sxs-lookup"><span data-stu-id="93561-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="93561-111">リスト windowsPrivacyDataAccessControlItems</span><span class="sxs-lookup"><span data-stu-id="93561-111">List windowsPrivacyDataAccessControlItems</span></span>](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-list.md)|<span data-ttu-id="93561-112">[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="93561-112">[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) collection</span></span>|<span data-ttu-id="93561-113">[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="93561-113">List properties and relationships of the [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) objects.</span></span>|
|[<span data-ttu-id="93561-114">windowsPrivacyDataAccessControlItem を取得する</span><span class="sxs-lookup"><span data-stu-id="93561-114">Get windowsPrivacyDataAccessControlItem</span></span>](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-get.md)|[<span data-ttu-id="93561-115">windowsPrivacyDataAccessControlItem</span><span class="sxs-lookup"><span data-stu-id="93561-115">windowsPrivacyDataAccessControlItem</span></span>](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|<span data-ttu-id="93561-116">[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="93561-116">Read properties and relationships of the [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>|
|[<span data-ttu-id="93561-117">windowsPrivacyDataAccessControlItem を作成する</span><span class="sxs-lookup"><span data-stu-id="93561-117">Create windowsPrivacyDataAccessControlItem</span></span>](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-create.md)|[<span data-ttu-id="93561-118">windowsPrivacyDataAccessControlItem</span><span class="sxs-lookup"><span data-stu-id="93561-118">windowsPrivacyDataAccessControlItem</span></span>](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|<span data-ttu-id="93561-119">新しい[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="93561-119">Create a new [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>|
|[<span data-ttu-id="93561-120">windowsPrivacyDataAccessControlItem の削除</span><span class="sxs-lookup"><span data-stu-id="93561-120">Delete windowsPrivacyDataAccessControlItem</span></span>](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-delete.md)|<span data-ttu-id="93561-121">なし</span><span class="sxs-lookup"><span data-stu-id="93561-121">None</span></span>|<span data-ttu-id="93561-122">[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="93561-122">Deletes a [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md).</span></span>|
|[<span data-ttu-id="93561-123">windowsPrivacyDataAccessControlItem の更新</span><span class="sxs-lookup"><span data-stu-id="93561-123">Update windowsPrivacyDataAccessControlItem</span></span>](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-update.md)|[<span data-ttu-id="93561-124">windowsPrivacyDataAccessControlItem</span><span class="sxs-lookup"><span data-stu-id="93561-124">windowsPrivacyDataAccessControlItem</span></span>](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|<span data-ttu-id="93561-125">[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="93561-125">Update the properties of a [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="93561-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="93561-126">Properties</span></span>
|<span data-ttu-id="93561-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="93561-127">Property</span></span>|<span data-ttu-id="93561-128">型</span><span class="sxs-lookup"><span data-stu-id="93561-128">Type</span></span>|<span data-ttu-id="93561-129">説明</span><span class="sxs-lookup"><span data-stu-id="93561-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93561-130">id</span><span class="sxs-lookup"><span data-stu-id="93561-130">id</span></span>|<span data-ttu-id="93561-131">String</span><span class="sxs-lookup"><span data-stu-id="93561-131">String</span></span>|<span data-ttu-id="93561-132">WindowsPrivacyDataAccessControlItem のキー。</span><span class="sxs-lookup"><span data-stu-id="93561-132">The key of WindowsPrivacyDataAccessControlItem.</span></span>|
|<span data-ttu-id="93561-133">accessLevel</span><span class="sxs-lookup"><span data-stu-id="93561-133">accessLevel</span></span>|[<span data-ttu-id="93561-134">windowsPrivacyDataAccessLevel</span><span class="sxs-lookup"><span data-stu-id="93561-134">windowsPrivacyDataAccessLevel</span></span>](../resources/intune-deviceconfig-windowsprivacydataaccesslevel.md)|<span data-ttu-id="93561-135">これは、指定されたアプリケーションに割り当てられるプライバシーデータカテゴリのアクセスレベルを示します。</span><span class="sxs-lookup"><span data-stu-id="93561-135">This indicates an access level for the privacy data category to which the specified application will be given to.</span></span> <span data-ttu-id="93561-136">使用可能な値は、`notConfigured`、`forceAllow`、`forceDeny`、`userInControl` です。</span><span class="sxs-lookup"><span data-stu-id="93561-136">Possible values are: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.</span></span>|
|<span data-ttu-id="93561-137">引数 datacategory</span><span class="sxs-lookup"><span data-stu-id="93561-137">dataCategory</span></span>|[<span data-ttu-id="93561-138">windowsPrivacyDataCategory</span><span class="sxs-lookup"><span data-stu-id="93561-138">windowsPrivacyDataCategory</span></span>](../resources/intune-deviceconfig-windowsprivacydatacategory.md)|<span data-ttu-id="93561-139">これは、特定のアクセス制御が適用されるプライバシーデータカテゴリを示します。</span><span class="sxs-lookup"><span data-stu-id="93561-139">This indicates a privacy data category to which the specific access control will apply.</span></span> <span data-ttu-id="93561-140">可能な値: `notConfigured`、 `accountInfo` `appsRunInBackground` `calendar` `callHistory` `camera` `contacts` `diagnosticsInfo` `email` `location` `messaging` `microphone`、、、、、、、、、、、、 `motion` `notifications` `phone` `radios` `tasks` `syncWithDevices` `trustedDevices`.</span><span class="sxs-lookup"><span data-stu-id="93561-140">Possible values are: `notConfigured`, `accountInfo`, `appsRunInBackground`, `calendar`, `callHistory`, `camera`, `contacts`, `diagnosticsInfo`, `email`, `location`, `messaging`, `microphone`, `motion`, `notifications`, `phone`, `radios`, `tasks`, `syncWithDevices`, `trustedDevices`.</span></span>|
|<span data-ttu-id="93561-141">app・パッケージ efamilyname</span><span class="sxs-lookup"><span data-stu-id="93561-141">appPackageFamilyName</span></span>|<span data-ttu-id="93561-142">String</span><span class="sxs-lookup"><span data-stu-id="93561-142">String</span></span>|<span data-ttu-id="93561-143">Windows アプリのパッケージファミリ名。</span><span class="sxs-lookup"><span data-stu-id="93561-143">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="93561-144">設定すると、指定したアプリケーションにアクセスレベルが適用されます。</span><span class="sxs-lookup"><span data-stu-id="93561-144">When set, the access level applies to the specified application.</span></span>|
|<span data-ttu-id="93561-145">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="93561-145">appDisplayName</span></span>|<span data-ttu-id="93561-146">String</span><span class="sxs-lookup"><span data-stu-id="93561-146">String</span></span>|<span data-ttu-id="93561-147">Windows アプリのパッケージファミリ名。</span><span class="sxs-lookup"><span data-stu-id="93561-147">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="93561-148">設定すると、指定したアプリケーションにアクセスレベルが適用されます。</span><span class="sxs-lookup"><span data-stu-id="93561-148">When set, the access level applies to the specified application.</span></span>|

## <a name="relationships"></a><span data-ttu-id="93561-149">関係</span><span class="sxs-lookup"><span data-stu-id="93561-149">Relationships</span></span>
<span data-ttu-id="93561-150">なし</span><span class="sxs-lookup"><span data-stu-id="93561-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="93561-151">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="93561-151">JSON Representation</span></span>
<span data-ttu-id="93561-152">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="93561-152">Here is a JSON representation of the resource.</span></span>
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





