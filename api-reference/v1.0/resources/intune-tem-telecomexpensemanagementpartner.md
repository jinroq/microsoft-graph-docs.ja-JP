---
title: telecomExpenseManagementPartner リソースの種類
description: telecomExpenseManagementPartner リソースは、特定の TEM サービスのメタデータおよび状態を表します。 貴社がパートナーと協力関係を結ぶと、パートナーが TEM 機能をオンまたはオフに切り替える機能を有効または無効にできます。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: c515b21f5727bcb60588a6722cc3fd6b02719e36
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981799"
---
# <a name="telecomexpensemanagementpartner-resource-type"></a><span data-ttu-id="8e08c-104">telecomExpenseManagementPartner リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8e08c-104">telecomExpenseManagementPartner resource type</span></span>

> <span data-ttu-id="8e08c-105">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8e08c-105">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8e08c-106">telecomExpenseManagementPartner リソースは、特定の TEM サービスのメタデータおよび状態を表します。</span><span class="sxs-lookup"><span data-stu-id="8e08c-106">telecomExpenseManagementPartner resources represent the metadata and status of a given TEM service.</span></span> <span data-ttu-id="8e08c-107">貴社がパートナーと協力関係を結ぶと、パートナーが TEM 機能をオンまたはオフに切り替える機能を有効または無効にできます。</span><span class="sxs-lookup"><span data-stu-id="8e08c-107">Once your organization has onboarded with a partner, the partner can be enabled or disabled to switch TEM functionality on or off.</span></span>
## <a name="methods"></a><span data-ttu-id="8e08c-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="8e08c-108">Methods</span></span>
|<span data-ttu-id="8e08c-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="8e08c-109">Method</span></span>|<span data-ttu-id="8e08c-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="8e08c-110">Return Type</span></span>|<span data-ttu-id="8e08c-111">説明</span><span class="sxs-lookup"><span data-stu-id="8e08c-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8e08c-112">telecomExpenseManagementPartners のリスト</span><span class="sxs-lookup"><span data-stu-id="8e08c-112">List telecomExpenseManagementPartners</span></span>](../api/intune-tem-telecomexpensemanagementpartner-list.md)|<span data-ttu-id="8e08c-113">[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="8e08c-113">[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) collection</span></span>|<span data-ttu-id="8e08c-114">[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="8e08c-114">List properties and relationships of the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) objects.</span></span>|
|[<span data-ttu-id="8e08c-115">telecomExpenseManagementPartner の取得</span><span class="sxs-lookup"><span data-stu-id="8e08c-115">Get telecomExpenseManagementPartner</span></span>](../api/intune-tem-telecomexpensemanagementpartner-get.md)|[<span data-ttu-id="8e08c-116">telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="8e08c-116">telecomExpenseManagementPartner</span></span>](../resources/intune-tem-telecomexpensemanagementpartner.md)|<span data-ttu-id="8e08c-117">[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="8e08c-117">Read properties and relationships of the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>|
|[<span data-ttu-id="8e08c-118">telecomExpenseManagementPartner の作成</span><span class="sxs-lookup"><span data-stu-id="8e08c-118">Create telecomExpenseManagementPartner</span></span>](../api/intune-tem-telecomexpensemanagementpartner-create.md)|[<span data-ttu-id="8e08c-119">telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="8e08c-119">telecomExpenseManagementPartner</span></span>](../resources/intune-tem-telecomexpensemanagementpartner.md)|<span data-ttu-id="8e08c-120">新しい [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="8e08c-120">Create a new [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>|
|[<span data-ttu-id="8e08c-121">telecomExpenseManagementPartner の削除</span><span class="sxs-lookup"><span data-stu-id="8e08c-121">Delete telecomExpenseManagementPartner</span></span>](../api/intune-tem-telecomexpensemanagementpartner-delete.md)|<span data-ttu-id="8e08c-122">なし</span><span class="sxs-lookup"><span data-stu-id="8e08c-122">None</span></span>|<span data-ttu-id="8e08c-123">[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="8e08c-123">Deletes a [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span></span>|
|[<span data-ttu-id="8e08c-124">telecomExpenseManagementPartner の更新</span><span class="sxs-lookup"><span data-stu-id="8e08c-124">Update telecomExpenseManagementPartner</span></span>](../api/intune-tem-telecomexpensemanagementpartner-update.md)|[<span data-ttu-id="8e08c-125">telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="8e08c-125">telecomExpenseManagementPartner</span></span>](../resources/intune-tem-telecomexpensemanagementpartner.md)|<span data-ttu-id="8e08c-126">[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="8e08c-126">Update the properties of a [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8e08c-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8e08c-127">Properties</span></span>
|<span data-ttu-id="8e08c-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8e08c-128">Property</span></span>|<span data-ttu-id="8e08c-129">型</span><span class="sxs-lookup"><span data-stu-id="8e08c-129">Type</span></span>|<span data-ttu-id="8e08c-130">説明</span><span class="sxs-lookup"><span data-stu-id="8e08c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e08c-131">ID</span><span class="sxs-lookup"><span data-stu-id="8e08c-131">id</span></span>|<span data-ttu-id="8e08c-132">String</span><span class="sxs-lookup"><span data-stu-id="8e08c-132">String</span></span>|<span data-ttu-id="8e08c-133">TEM パートナーの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="8e08c-133">Unique identifier of the TEM partner.</span></span>|
|<span data-ttu-id="8e08c-134">displayName</span><span class="sxs-lookup"><span data-stu-id="8e08c-134">displayName</span></span>|<span data-ttu-id="8e08c-135">String</span><span class="sxs-lookup"><span data-stu-id="8e08c-135">String</span></span>|<span data-ttu-id="8e08c-136">TEM パートナーの表示名。</span><span class="sxs-lookup"><span data-stu-id="8e08c-136">Display name of the TEM partner.</span></span>|
|<span data-ttu-id="8e08c-137">url</span><span class="sxs-lookup"><span data-stu-id="8e08c-137">url</span></span>|<span data-ttu-id="8e08c-138">String</span><span class="sxs-lookup"><span data-stu-id="8e08c-138">String</span></span>|<span data-ttu-id="8e08c-139">TEM パートナーの管理用コントロール パネルの URL。管理者はここで TEM サービスを構成できます。</span><span class="sxs-lookup"><span data-stu-id="8e08c-139">URL of the TEM partner's administrative control panel, where an administrator can configure their TEM service.</span></span>|
|<span data-ttu-id="8e08c-140">appAuthorized</span><span class="sxs-lookup"><span data-stu-id="8e08c-140">appAuthorized</span></span>|<span data-ttu-id="8e08c-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="8e08c-141">Boolean</span></span>|<span data-ttu-id="8e08c-142">パートナーの AAD アプリに Intune へのアクセスが承認されているかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="8e08c-142">Whether the partner's AAD app has been authorized to access Intune.</span></span>|
|<span data-ttu-id="8e08c-143">enabled</span><span class="sxs-lookup"><span data-stu-id="8e08c-143">enabled</span></span>|<span data-ttu-id="8e08c-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="8e08c-144">Boolean</span></span>|<span data-ttu-id="8e08c-145">TEM サービスへの Intune の接続が現在有効であるか、無効であるかを指定します。</span><span class="sxs-lookup"><span data-stu-id="8e08c-145">Whether Intune's connection to the TEM service is currently enabled or disabled.</span></span>|
|<span data-ttu-id="8e08c-146">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="8e08c-146">lastConnectionDateTime</span></span>|<span data-ttu-id="8e08c-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e08c-147">DateTimeOffset</span></span>|<span data-ttu-id="8e08c-148">TEM パートナーによって Intune に対して最後に送信された要求のタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="8e08c-148">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8e08c-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8e08c-149">Relationships</span></span>
<span data-ttu-id="8e08c-150">なし</span><span class="sxs-lookup"><span data-stu-id="8e08c-150">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8e08c-151">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8e08c-151">JSON Representation</span></span>
<span data-ttu-id="8e08c-152">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8e08c-152">Here is a JSON representation of the resource.</span></span>
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



