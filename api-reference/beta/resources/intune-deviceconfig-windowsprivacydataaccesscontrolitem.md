---
title: windowsPrivacyDataAccessControlItem リソースの種類
description: プライバシー データのカテゴリごとのアクセス制御レベルを指定します。
author: tfitzmac
ms.openlocfilehash: 3655282d7b3b6ff31268f9fe536a4a8f6ac85341
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314988"
---
# <a name="windowsprivacydataaccesscontrolitem-resource-type"></a><span data-ttu-id="21ab3-103">windowsPrivacyDataAccessControlItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="21ab3-103">windowsPrivacyDataAccessControlItem resource type</span></span>

> <span data-ttu-id="21ab3-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="21ab3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="21ab3-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="21ab3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="21ab3-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="21ab3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="21ab3-107">プライバシー データのカテゴリごとのアクセス制御レベルを指定します。</span><span class="sxs-lookup"><span data-stu-id="21ab3-107">Specify access control level per privacy data category</span></span>
## <a name="methods"></a><span data-ttu-id="21ab3-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="21ab3-108">Methods</span></span>
|<span data-ttu-id="21ab3-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="21ab3-109">Method</span></span>|<span data-ttu-id="21ab3-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="21ab3-110">Return Type</span></span>|<span data-ttu-id="21ab3-111">説明</span><span class="sxs-lookup"><span data-stu-id="21ab3-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="21ab3-112">リスト windowsPrivacyDataAccessControlItems</span><span class="sxs-lookup"><span data-stu-id="21ab3-112">List windowsPrivacyDataAccessControlItems</span></span>](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-list.md)|<span data-ttu-id="21ab3-113">[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="21ab3-113">[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) collection</span></span>|<span data-ttu-id="21ab3-114">[WindowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="21ab3-114">List properties and relationships of the [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) objects.</span></span>|
|[<span data-ttu-id="21ab3-115">WindowsPrivacyDataAccessControlItem を取得します。</span><span class="sxs-lookup"><span data-stu-id="21ab3-115">Get windowsPrivacyDataAccessControlItem</span></span>](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-get.md)|[<span data-ttu-id="21ab3-116">windowsPrivacyDataAccessControlItem</span><span class="sxs-lookup"><span data-stu-id="21ab3-116">windowsPrivacyDataAccessControlItem</span></span>](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|<span data-ttu-id="21ab3-117">[WindowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="21ab3-117">Read properties and relationships of the [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>|
|[<span data-ttu-id="21ab3-118">WindowsPrivacyDataAccessControlItem を作成します。</span><span class="sxs-lookup"><span data-stu-id="21ab3-118">Create windowsPrivacyDataAccessControlItem</span></span>](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-create.md)|[<span data-ttu-id="21ab3-119">windowsPrivacyDataAccessControlItem</span><span class="sxs-lookup"><span data-stu-id="21ab3-119">windowsPrivacyDataAccessControlItem</span></span>](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|<span data-ttu-id="21ab3-120">新しい[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="21ab3-120">Create a new [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>|
|[<span data-ttu-id="21ab3-121">WindowsPrivacyDataAccessControlItem を削除します。</span><span class="sxs-lookup"><span data-stu-id="21ab3-121">Delete windowsPrivacyDataAccessControlItem</span></span>](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-delete.md)|<span data-ttu-id="21ab3-122">なし</span><span class="sxs-lookup"><span data-stu-id="21ab3-122">None</span></span>|<span data-ttu-id="21ab3-123">の[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="21ab3-123">Deletes a [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md).</span></span>|
|[<span data-ttu-id="21ab3-124">WindowsPrivacyDataAccessControlItem を更新します。</span><span class="sxs-lookup"><span data-stu-id="21ab3-124">Update windowsPrivacyDataAccessControlItem</span></span>](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-update.md)|[<span data-ttu-id="21ab3-125">windowsPrivacyDataAccessControlItem</span><span class="sxs-lookup"><span data-stu-id="21ab3-125">windowsPrivacyDataAccessControlItem</span></span>](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|<span data-ttu-id="21ab3-126">[WindowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="21ab3-126">Update the properties of a [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="21ab3-127">Properties</span><span class="sxs-lookup"><span data-stu-id="21ab3-127">Properties</span></span>
|<span data-ttu-id="21ab3-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="21ab3-128">Property</span></span>|<span data-ttu-id="21ab3-129">種類</span><span class="sxs-lookup"><span data-stu-id="21ab3-129">Type</span></span>|<span data-ttu-id="21ab3-130">説明</span><span class="sxs-lookup"><span data-stu-id="21ab3-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21ab3-131">ID</span><span class="sxs-lookup"><span data-stu-id="21ab3-131">id</span></span>|<span data-ttu-id="21ab3-132">String</span><span class="sxs-lookup"><span data-stu-id="21ab3-132">String</span></span>|<span data-ttu-id="21ab3-133">WindowsPrivacyDataAccessControlItem のキー。</span><span class="sxs-lookup"><span data-stu-id="21ab3-133">The key of WindowsPrivacyDataAccessControlItem.</span></span>|
|<span data-ttu-id="21ab3-134">accessLevel</span><span class="sxs-lookup"><span data-stu-id="21ab3-134">accessLevel</span></span>|[<span data-ttu-id="21ab3-135">windowsPrivacyDataAccessLevel</span><span class="sxs-lookup"><span data-stu-id="21ab3-135">windowsPrivacyDataAccessLevel</span></span>](../resources/intune-deviceconfig-windowsprivacydataaccesslevel.md)|<span data-ttu-id="21ab3-136">プライバシー データ カテゴリに、指定したアプリケーションを指定するアクセス レベルを示します。</span><span class="sxs-lookup"><span data-stu-id="21ab3-136">This indicates an access level for the privacy data category to which the specified application will be given to.</span></span> <span data-ttu-id="21ab3-137">可能な値は、`notConfigured`、`forceAllow`、`forceDeny`、`userInControl` です。</span><span class="sxs-lookup"><span data-stu-id="21ab3-137">Possible values are: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.</span></span>|
|<span data-ttu-id="21ab3-138">dataCategory</span><span class="sxs-lookup"><span data-stu-id="21ab3-138">dataCategory</span></span>|[<span data-ttu-id="21ab3-139">windowsPrivacyDataCategory</span><span class="sxs-lookup"><span data-stu-id="21ab3-139">windowsPrivacyDataCategory</span></span>](../resources/intune-deviceconfig-windowsprivacydatacategory.md)|<span data-ttu-id="21ab3-140">これは、特定のアクセス制御が適用されるプライバシー データのカテゴリを示します。</span><span class="sxs-lookup"><span data-stu-id="21ab3-140">This indicates a privacy data category to which the specific access control will apply.</span></span> <span data-ttu-id="21ab3-141">使用可能な値: `notConfigured`、 `accountInfo`、 `appsRunInBackground`、 `calendar`、 `callHistory`、 `camera`、 `contacts`、 `diagnosticsInfo`、 `email`、 `location`、 `messaging`、 `microphone`、 `motion`、 `notifications`、 `phone`、 `radios`、 `tasks`、 `syncWithDevices`、 `trustedDevices`.</span><span class="sxs-lookup"><span data-stu-id="21ab3-141">Possible values are: `notConfigured`, `accountInfo`, `appsRunInBackground`, `calendar`, `callHistory`, `camera`, `contacts`, `diagnosticsInfo`, `email`, `location`, `messaging`, `microphone`, `motion`, `notifications`, `phone`, `radios`, `tasks`, `syncWithDevices`, `trustedDevices`.</span></span>|
|<span data-ttu-id="21ab3-142">appPackageFamilyName</span><span class="sxs-lookup"><span data-stu-id="21ab3-142">appPackageFamilyName</span></span>|<span data-ttu-id="21ab3-143">String</span><span class="sxs-lookup"><span data-stu-id="21ab3-143">String</span></span>|<span data-ttu-id="21ab3-144">Windows アプリケーションのパッケージ ファミリ名です。</span><span class="sxs-lookup"><span data-stu-id="21ab3-144">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="21ab3-145">アクセス レベルを設定すると、指定したアプリケーションを適用します。</span><span class="sxs-lookup"><span data-stu-id="21ab3-145">When set, the access level applies to the specified application.</span></span>|
|<span data-ttu-id="21ab3-146">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="21ab3-146">appDisplayName</span></span>|<span data-ttu-id="21ab3-147">String</span><span class="sxs-lookup"><span data-stu-id="21ab3-147">String</span></span>|<span data-ttu-id="21ab3-148">Windows アプリケーションのパッケージ ファミリ名です。</span><span class="sxs-lookup"><span data-stu-id="21ab3-148">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="21ab3-149">アクセス レベルを設定すると、指定したアプリケーションを適用します。</span><span class="sxs-lookup"><span data-stu-id="21ab3-149">When set, the access level applies to the specified application.</span></span>|

## <a name="relationships"></a><span data-ttu-id="21ab3-150">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="21ab3-150">Relationships</span></span>
<span data-ttu-id="21ab3-151">なし</span><span class="sxs-lookup"><span data-stu-id="21ab3-151">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="21ab3-152">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="21ab3-152">JSON Representation</span></span>
<span data-ttu-id="21ab3-153">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="21ab3-153">Here is a JSON representation of the resource.</span></span>
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





