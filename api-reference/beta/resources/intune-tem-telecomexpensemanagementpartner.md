---
title: telecomExpenseManagementPartner リソースの種類
description: telecomExpenseManagementPartner リソースは、特定の TEM サービスのメタデータおよび状態を表します。 貴社がパートナーと協力関係を結ぶと、パートナーが TEM 機能をオンまたはオフに切り替える機能を有効または無効にできます。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3e1d148366a9ff67b643bad37e6aef5ed67653d1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401853"
---
# <a name="telecomexpensemanagementpartner-resource-type"></a><span data-ttu-id="a3317-104">telecomExpenseManagementPartner リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a3317-104">telecomExpenseManagementPartner resource type</span></span>

> <span data-ttu-id="a3317-105">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a3317-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a3317-106">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a3317-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a3317-107">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a3317-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3317-108">telecomExpenseManagementPartner リソースは、特定の TEM サービスのメタデータおよび状態を表します。</span><span class="sxs-lookup"><span data-stu-id="a3317-108">telecomExpenseManagementPartner resources represent the metadata and status of a given TEM service.</span></span> <span data-ttu-id="a3317-109">貴社がパートナーと協力関係を結ぶと、パートナーが TEM 機能をオンまたはオフに切り替える機能を有効または無効にできます。</span><span class="sxs-lookup"><span data-stu-id="a3317-109">Once your organization has onboarded with a partner, the partner can be enabled or disabled to switch TEM functionality on or off.</span></span>

## <a name="methods"></a><span data-ttu-id="a3317-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="a3317-110">Methods</span></span>
|<span data-ttu-id="a3317-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="a3317-111">Method</span></span>|<span data-ttu-id="a3317-112">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a3317-112">Return Type</span></span>|<span data-ttu-id="a3317-113">説明</span><span class="sxs-lookup"><span data-stu-id="a3317-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a3317-114">telecomExpenseManagementPartners のリスト</span><span class="sxs-lookup"><span data-stu-id="a3317-114">List telecomExpenseManagementPartners</span></span>](../api/intune-tem-telecomexpensemanagementpartner-list.md)|<span data-ttu-id="a3317-115">[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a3317-115">[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) collection</span></span>|<span data-ttu-id="a3317-116">[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="a3317-116">List properties and relationships of the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) objects.</span></span>|
|[<span data-ttu-id="a3317-117">telecomExpenseManagementPartner の取得</span><span class="sxs-lookup"><span data-stu-id="a3317-117">Get telecomExpenseManagementPartner</span></span>](../api/intune-tem-telecomexpensemanagementpartner-get.md)|[<span data-ttu-id="a3317-118">telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="a3317-118">telecomExpenseManagementPartner</span></span>](../resources/intune-tem-telecomexpensemanagementpartner.md)|<span data-ttu-id="a3317-119">[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="a3317-119">Read properties and relationships of the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>|
|[<span data-ttu-id="a3317-120">telecomExpenseManagementPartner の作成</span><span class="sxs-lookup"><span data-stu-id="a3317-120">Create telecomExpenseManagementPartner</span></span>](../api/intune-tem-telecomexpensemanagementpartner-create.md)|[<span data-ttu-id="a3317-121">telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="a3317-121">telecomExpenseManagementPartner</span></span>](../resources/intune-tem-telecomexpensemanagementpartner.md)|<span data-ttu-id="a3317-122">新しい [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="a3317-122">Create a new [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>|
|[<span data-ttu-id="a3317-123">telecomExpenseManagementPartner の削除</span><span class="sxs-lookup"><span data-stu-id="a3317-123">Delete telecomExpenseManagementPartner</span></span>](../api/intune-tem-telecomexpensemanagementpartner-delete.md)|<span data-ttu-id="a3317-124">なし</span><span class="sxs-lookup"><span data-stu-id="a3317-124">None</span></span>|<span data-ttu-id="a3317-125">[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="a3317-125">Deletes a [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span></span>|
|[<span data-ttu-id="a3317-126">telecomExpenseManagementPartner の更新</span><span class="sxs-lookup"><span data-stu-id="a3317-126">Update telecomExpenseManagementPartner</span></span>](../api/intune-tem-telecomexpensemanagementpartner-update.md)|[<span data-ttu-id="a3317-127">telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="a3317-127">telecomExpenseManagementPartner</span></span>](../resources/intune-tem-telecomexpensemanagementpartner.md)|<span data-ttu-id="a3317-128">[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a3317-128">Update the properties of a [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a3317-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a3317-129">Properties</span></span>
|<span data-ttu-id="a3317-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a3317-130">Property</span></span>|<span data-ttu-id="a3317-131">型</span><span class="sxs-lookup"><span data-stu-id="a3317-131">Type</span></span>|<span data-ttu-id="a3317-132">説明</span><span class="sxs-lookup"><span data-stu-id="a3317-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3317-133">id</span><span class="sxs-lookup"><span data-stu-id="a3317-133">id</span></span>|<span data-ttu-id="a3317-134">String</span><span class="sxs-lookup"><span data-stu-id="a3317-134">String</span></span>|<span data-ttu-id="a3317-135">TEM パートナーの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="a3317-135">Unique identifier of the TEM partner.</span></span>|
|<span data-ttu-id="a3317-136">displayName</span><span class="sxs-lookup"><span data-stu-id="a3317-136">displayName</span></span>|<span data-ttu-id="a3317-137">String</span><span class="sxs-lookup"><span data-stu-id="a3317-137">String</span></span>|<span data-ttu-id="a3317-138">TEM パートナーの表示名。</span><span class="sxs-lookup"><span data-stu-id="a3317-138">Display name of the TEM partner.</span></span>|
|<span data-ttu-id="a3317-139">url</span><span class="sxs-lookup"><span data-stu-id="a3317-139">url</span></span>|<span data-ttu-id="a3317-140">String</span><span class="sxs-lookup"><span data-stu-id="a3317-140">String</span></span>|<span data-ttu-id="a3317-141">TEM パートナーの管理用コントロール パネルの URL。管理者はここで TEM サービスを構成できます。</span><span class="sxs-lookup"><span data-stu-id="a3317-141">URL of the TEM partner's administrative control panel, where an administrator can configure their TEM service.</span></span>|
|<span data-ttu-id="a3317-142">appAuthorized</span><span class="sxs-lookup"><span data-stu-id="a3317-142">appAuthorized</span></span>|<span data-ttu-id="a3317-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="a3317-143">Boolean</span></span>|<span data-ttu-id="a3317-144">パートナーの AAD アプリに Intune へのアクセスが承認されているかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="a3317-144">Whether the partner's AAD app has been authorized to access Intune.</span></span>|
|<span data-ttu-id="a3317-145">enabled</span><span class="sxs-lookup"><span data-stu-id="a3317-145">enabled</span></span>|<span data-ttu-id="a3317-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="a3317-146">Boolean</span></span>|<span data-ttu-id="a3317-147">TEM サービスへの Intune の接続が現在有効であるか、無効であるかを指定します。</span><span class="sxs-lookup"><span data-stu-id="a3317-147">Whether Intune's connection to the TEM service is currently enabled or disabled.</span></span>|
|<span data-ttu-id="a3317-148">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="a3317-148">lastConnectionDateTime</span></span>|<span data-ttu-id="a3317-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a3317-149">DateTimeOffset</span></span>|<span data-ttu-id="a3317-150">TEM パートナーによって Intune に対して最後に送信された要求のタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="a3317-150">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a3317-151">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a3317-151">Relationships</span></span>
<span data-ttu-id="a3317-152">なし</span><span class="sxs-lookup"><span data-stu-id="a3317-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a3317-153">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a3317-153">JSON Representation</span></span>
<span data-ttu-id="a3317-154">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a3317-154">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.telecomExpenseManagementPartner"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.telecomExpenseManagementPartner",
  "id": "String (identifier)",
  "displayName": "String",
  "url": "String",
  "appAuthorized": true,
  "enabled": true,
  "lastConnectionDateTime": "String (timestamp)"
}
```




