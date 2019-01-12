---
title: telecomExpenseManagementPartner リソースの種類
description: telecomExpenseManagementPartner リソースは、特定の TEM サービスのメタデータおよび状態を表します。 貴社がパートナーと協力関係を結ぶと、パートナーが TEM 機能をオンまたはオフに切り替える機能を有効または無効にできます。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: f6bbb76a98e664f759f8e543eecafe2df6167515
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923020"
---
# <a name="telecomexpensemanagementpartner-resource-type"></a><span data-ttu-id="ddcbf-104">telecomExpenseManagementPartner リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ddcbf-104">telecomExpenseManagementPartner resource type</span></span>

> <span data-ttu-id="ddcbf-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ddcbf-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ddcbf-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ddcbf-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ddcbf-107">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ddcbf-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ddcbf-108">telecomExpenseManagementPartner リソースは、特定の TEM サービスのメタデータおよび状態を表します。</span><span class="sxs-lookup"><span data-stu-id="ddcbf-108">telecomExpenseManagementPartner resources represent the metadata and status of a given TEM service.</span></span> <span data-ttu-id="ddcbf-109">貴社がパートナーと協力関係を結ぶと、パートナーが TEM 機能をオンまたはオフに切り替える機能を有効または無効にできます。</span><span class="sxs-lookup"><span data-stu-id="ddcbf-109">Once your organization has onboarded with a partner, the partner can be enabled or disabled to switch TEM functionality on or off.</span></span>
## <a name="methods"></a><span data-ttu-id="ddcbf-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="ddcbf-110">Methods</span></span>
|<span data-ttu-id="ddcbf-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="ddcbf-111">Method</span></span>|<span data-ttu-id="ddcbf-112">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ddcbf-112">Return Type</span></span>|<span data-ttu-id="ddcbf-113">説明</span><span class="sxs-lookup"><span data-stu-id="ddcbf-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ddcbf-114">telecomExpenseManagementPartners のリスト</span><span class="sxs-lookup"><span data-stu-id="ddcbf-114">List telecomExpenseManagementPartners</span></span>](../api/intune-tem-telecomexpensemanagementpartner-list.md)|<span data-ttu-id="ddcbf-115">[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ddcbf-115">[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) collection</span></span>|<span data-ttu-id="ddcbf-116">[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="ddcbf-116">List properties and relationships of the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) objects.</span></span>|
|[<span data-ttu-id="ddcbf-117">telecomExpenseManagementPartner の取得</span><span class="sxs-lookup"><span data-stu-id="ddcbf-117">Get telecomExpenseManagementPartner</span></span>](../api/intune-tem-telecomexpensemanagementpartner-get.md)|[<span data-ttu-id="ddcbf-118">telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="ddcbf-118">telecomExpenseManagementPartner</span></span>](../resources/intune-tem-telecomexpensemanagementpartner.md)|<span data-ttu-id="ddcbf-119">[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="ddcbf-119">Read properties and relationships of the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>|
|[<span data-ttu-id="ddcbf-120">telecomExpenseManagementPartner の作成</span><span class="sxs-lookup"><span data-stu-id="ddcbf-120">Create telecomExpenseManagementPartner</span></span>](../api/intune-tem-telecomexpensemanagementpartner-create.md)|[<span data-ttu-id="ddcbf-121">telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="ddcbf-121">telecomExpenseManagementPartner</span></span>](../resources/intune-tem-telecomexpensemanagementpartner.md)|<span data-ttu-id="ddcbf-122">新しい [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="ddcbf-122">Create a new [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>|
|[<span data-ttu-id="ddcbf-123">telecomExpenseManagementPartner の削除</span><span class="sxs-lookup"><span data-stu-id="ddcbf-123">Delete telecomExpenseManagementPartner</span></span>](../api/intune-tem-telecomexpensemanagementpartner-delete.md)|<span data-ttu-id="ddcbf-124">なし</span><span class="sxs-lookup"><span data-stu-id="ddcbf-124">None</span></span>|<span data-ttu-id="ddcbf-125">[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="ddcbf-125">Deletes a [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span></span>|
|[<span data-ttu-id="ddcbf-126">telecomExpenseManagementPartner の更新</span><span class="sxs-lookup"><span data-stu-id="ddcbf-126">Update telecomExpenseManagementPartner</span></span>](../api/intune-tem-telecomexpensemanagementpartner-update.md)|[<span data-ttu-id="ddcbf-127">telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="ddcbf-127">telecomExpenseManagementPartner</span></span>](../resources/intune-tem-telecomexpensemanagementpartner.md)|<span data-ttu-id="ddcbf-128">[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ddcbf-128">Update the properties of a [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ddcbf-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ddcbf-129">Properties</span></span>
|<span data-ttu-id="ddcbf-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ddcbf-130">Property</span></span>|<span data-ttu-id="ddcbf-131">型</span><span class="sxs-lookup"><span data-stu-id="ddcbf-131">Type</span></span>|<span data-ttu-id="ddcbf-132">説明</span><span class="sxs-lookup"><span data-stu-id="ddcbf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ddcbf-133">ID</span><span class="sxs-lookup"><span data-stu-id="ddcbf-133">id</span></span>|<span data-ttu-id="ddcbf-134">String</span><span class="sxs-lookup"><span data-stu-id="ddcbf-134">String</span></span>|<span data-ttu-id="ddcbf-135">TEM パートナーの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="ddcbf-135">Unique identifier of the TEM partner.</span></span>|
|<span data-ttu-id="ddcbf-136">displayName</span><span class="sxs-lookup"><span data-stu-id="ddcbf-136">displayName</span></span>|<span data-ttu-id="ddcbf-137">String</span><span class="sxs-lookup"><span data-stu-id="ddcbf-137">String</span></span>|<span data-ttu-id="ddcbf-138">TEM パートナーの表示名。</span><span class="sxs-lookup"><span data-stu-id="ddcbf-138">Display name of the TEM partner.</span></span>|
|<span data-ttu-id="ddcbf-139">url</span><span class="sxs-lookup"><span data-stu-id="ddcbf-139">url</span></span>|<span data-ttu-id="ddcbf-140">String</span><span class="sxs-lookup"><span data-stu-id="ddcbf-140">String</span></span>|<span data-ttu-id="ddcbf-141">TEM パートナーの管理用コントロール パネルの URL。管理者はここで TEM サービスを構成できます。</span><span class="sxs-lookup"><span data-stu-id="ddcbf-141">URL of the TEM partner's administrative control panel, where an administrator can configure their TEM service.</span></span>|
|<span data-ttu-id="ddcbf-142">appAuthorized</span><span class="sxs-lookup"><span data-stu-id="ddcbf-142">appAuthorized</span></span>|<span data-ttu-id="ddcbf-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddcbf-143">Boolean</span></span>|<span data-ttu-id="ddcbf-144">パートナーの AAD アプリに Intune へのアクセスが承認されているかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="ddcbf-144">Whether the partner's AAD app has been authorized to access Intune.</span></span>|
|<span data-ttu-id="ddcbf-145">enabled</span><span class="sxs-lookup"><span data-stu-id="ddcbf-145">enabled</span></span>|<span data-ttu-id="ddcbf-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddcbf-146">Boolean</span></span>|<span data-ttu-id="ddcbf-147">TEM サービスへの Intune の接続が現在有効であるか、無効であるかを指定します。</span><span class="sxs-lookup"><span data-stu-id="ddcbf-147">Whether Intune's connection to the TEM service is currently enabled or disabled.</span></span>|
|<span data-ttu-id="ddcbf-148">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="ddcbf-148">lastConnectionDateTime</span></span>|<span data-ttu-id="ddcbf-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ddcbf-149">DateTimeOffset</span></span>|<span data-ttu-id="ddcbf-150">TEM パートナーによって Intune に対して最後に送信された要求のタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="ddcbf-150">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ddcbf-151">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ddcbf-151">Relationships</span></span>
<span data-ttu-id="ddcbf-152">なし</span><span class="sxs-lookup"><span data-stu-id="ddcbf-152">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ddcbf-153">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ddcbf-153">JSON Representation</span></span>
<span data-ttu-id="ddcbf-154">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ddcbf-154">Here is a JSON representation of the resource.</span></span>
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





