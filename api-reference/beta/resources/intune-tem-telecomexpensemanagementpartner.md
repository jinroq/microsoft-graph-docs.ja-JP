---
title: telecomExpenseManagementPartner リソースの種類
description: telecomExpenseManagementPartner リソースは、特定の TEM サービスのメタデータおよび状態を表します。 貴社がパートナーと協力関係を結ぶと、パートナーが TEM 機能をオンまたはオフに切り替える機能を有効または無効にできます。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d6f0a0fd7b98627adfb49c88f619c6d8d6fd9fbe
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34991003"
---
# <a name="telecomexpensemanagementpartner-resource-type"></a><span data-ttu-id="1a90b-104">telecomExpenseManagementPartner リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1a90b-104">telecomExpenseManagementPartner resource type</span></span>

> <span data-ttu-id="1a90b-105">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1a90b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1a90b-106">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1a90b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a90b-107">telecomExpenseManagementPartner リソースは、特定の TEM サービスのメタデータおよび状態を表します。</span><span class="sxs-lookup"><span data-stu-id="1a90b-107">telecomExpenseManagementPartner resources represent the metadata and status of a given TEM service.</span></span> <span data-ttu-id="1a90b-108">貴社がパートナーと協力関係を結ぶと、パートナーが TEM 機能をオンまたはオフに切り替える機能を有効または無効にできます。</span><span class="sxs-lookup"><span data-stu-id="1a90b-108">Once your organization has onboarded with a partner, the partner can be enabled or disabled to switch TEM functionality on or off.</span></span>

## <a name="methods"></a><span data-ttu-id="1a90b-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="1a90b-109">Methods</span></span>
|<span data-ttu-id="1a90b-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="1a90b-110">Method</span></span>|<span data-ttu-id="1a90b-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="1a90b-111">Return Type</span></span>|<span data-ttu-id="1a90b-112">説明</span><span class="sxs-lookup"><span data-stu-id="1a90b-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1a90b-113">telecomExpenseManagementPartners のリスト</span><span class="sxs-lookup"><span data-stu-id="1a90b-113">List telecomExpenseManagementPartners</span></span>](../api/intune-tem-telecomexpensemanagementpartner-list.md)|<span data-ttu-id="1a90b-114">[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1a90b-114">[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) collection</span></span>|<span data-ttu-id="1a90b-115">[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="1a90b-115">List properties and relationships of the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) objects.</span></span>|
|[<span data-ttu-id="1a90b-116">telecomExpenseManagementPartner の取得</span><span class="sxs-lookup"><span data-stu-id="1a90b-116">Get telecomExpenseManagementPartner</span></span>](../api/intune-tem-telecomexpensemanagementpartner-get.md)|[<span data-ttu-id="1a90b-117">telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="1a90b-117">telecomExpenseManagementPartner</span></span>](../resources/intune-tem-telecomexpensemanagementpartner.md)|<span data-ttu-id="1a90b-118">[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="1a90b-118">Read properties and relationships of the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>|
|[<span data-ttu-id="1a90b-119">telecomExpenseManagementPartner の作成</span><span class="sxs-lookup"><span data-stu-id="1a90b-119">Create telecomExpenseManagementPartner</span></span>](../api/intune-tem-telecomexpensemanagementpartner-create.md)|[<span data-ttu-id="1a90b-120">telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="1a90b-120">telecomExpenseManagementPartner</span></span>](../resources/intune-tem-telecomexpensemanagementpartner.md)|<span data-ttu-id="1a90b-121">新しい [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="1a90b-121">Create a new [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>|
|[<span data-ttu-id="1a90b-122">telecomExpenseManagementPartner の削除</span><span class="sxs-lookup"><span data-stu-id="1a90b-122">Delete telecomExpenseManagementPartner</span></span>](../api/intune-tem-telecomexpensemanagementpartner-delete.md)|<span data-ttu-id="1a90b-123">なし</span><span class="sxs-lookup"><span data-stu-id="1a90b-123">None</span></span>|<span data-ttu-id="1a90b-124">[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="1a90b-124">Deletes a [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span></span>|
|[<span data-ttu-id="1a90b-125">telecomExpenseManagementPartner の更新</span><span class="sxs-lookup"><span data-stu-id="1a90b-125">Update telecomExpenseManagementPartner</span></span>](../api/intune-tem-telecomexpensemanagementpartner-update.md)|[<span data-ttu-id="1a90b-126">telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="1a90b-126">telecomExpenseManagementPartner</span></span>](../resources/intune-tem-telecomexpensemanagementpartner.md)|<span data-ttu-id="1a90b-127">[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="1a90b-127">Update the properties of a [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1a90b-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1a90b-128">Properties</span></span>
|<span data-ttu-id="1a90b-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1a90b-129">Property</span></span>|<span data-ttu-id="1a90b-130">型</span><span class="sxs-lookup"><span data-stu-id="1a90b-130">Type</span></span>|<span data-ttu-id="1a90b-131">説明</span><span class="sxs-lookup"><span data-stu-id="1a90b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a90b-132">id</span><span class="sxs-lookup"><span data-stu-id="1a90b-132">id</span></span>|<span data-ttu-id="1a90b-133">文字列</span><span class="sxs-lookup"><span data-stu-id="1a90b-133">String</span></span>|<span data-ttu-id="1a90b-134">TEM パートナーの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="1a90b-134">Unique identifier of the TEM partner.</span></span>|
|<span data-ttu-id="1a90b-135">displayName</span><span class="sxs-lookup"><span data-stu-id="1a90b-135">displayName</span></span>|<span data-ttu-id="1a90b-136">String</span><span class="sxs-lookup"><span data-stu-id="1a90b-136">String</span></span>|<span data-ttu-id="1a90b-137">TEM パートナーの表示名。</span><span class="sxs-lookup"><span data-stu-id="1a90b-137">Display name of the TEM partner.</span></span>|
|<span data-ttu-id="1a90b-138">url</span><span class="sxs-lookup"><span data-stu-id="1a90b-138">url</span></span>|<span data-ttu-id="1a90b-139">String</span><span class="sxs-lookup"><span data-stu-id="1a90b-139">String</span></span>|<span data-ttu-id="1a90b-140">TEM パートナーの管理用コントロール パネルの URL。管理者は、このパネルで TEM サービスを構成できます。</span><span class="sxs-lookup"><span data-stu-id="1a90b-140">URL of the TEM partner's administrative control panel, where an administrator can configure their TEM service.</span></span>|
|<span data-ttu-id="1a90b-141">appAuthorized</span><span class="sxs-lookup"><span data-stu-id="1a90b-141">appAuthorized</span></span>|<span data-ttu-id="1a90b-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a90b-142">Boolean</span></span>|<span data-ttu-id="1a90b-143">パートナーの AAD アプリに Intune へのアクセスが承認されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1a90b-143">Whether the partner's AAD app has been authorized to access Intune.</span></span>|
|<span data-ttu-id="1a90b-144">enabled</span><span class="sxs-lookup"><span data-stu-id="1a90b-144">enabled</span></span>|<span data-ttu-id="1a90b-145">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="1a90b-145">Boolean</span></span>|<span data-ttu-id="1a90b-146">TEM サービスへの Intune の接続が現在有効であるか、無効であるかを示します。</span><span class="sxs-lookup"><span data-stu-id="1a90b-146">Whether Intune's connection to the TEM service is currently enabled or disabled.</span></span>|
|<span data-ttu-id="1a90b-147">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="1a90b-147">lastConnectionDateTime</span></span>|<span data-ttu-id="1a90b-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a90b-148">DateTimeOffset</span></span>|<span data-ttu-id="1a90b-149">TEM パートナーによって Intune に対して最後に送信された要求のタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="1a90b-149">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1a90b-150">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1a90b-150">Relationships</span></span>
<span data-ttu-id="1a90b-151">なし</span><span class="sxs-lookup"><span data-stu-id="1a90b-151">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1a90b-152">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1a90b-152">JSON Representation</span></span>
<span data-ttu-id="1a90b-153">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1a90b-153">Here is a JSON representation of the resource.</span></span>
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





